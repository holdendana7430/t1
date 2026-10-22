代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2igfghpvf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yfwcxnuk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yyupmqmb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mlgzecwj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdqbamsb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjsemgdi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2usoxupsg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xyuovwxu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2borzsrjb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zsqdhzmi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ljtvjlnd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yyufnicb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kfvfyhld.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2odymomrs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2alqtrusv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeksnddw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xbbftzfy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nazovgeb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bvljceih.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zamlobps.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vdjedtjk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lwtxqxwh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eynvnkdq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2otsidhyq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ckspjxtx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2icliqluy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ufogjded.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cbqorlok.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ycxgzijc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bafjrdbo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lpmyqgap.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mbzgbyam.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfbsmuls.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fwqqzdoa.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkisnxtj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bfrmaina.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2eyfflvji.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2uedcrsdl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2etirkwtk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sxzypzxn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oozzrisp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tebejbvi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vggbdure.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2utkqrwvr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ihgmujpe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpxjmliu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2slkrxnki.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cmpwrywm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ibmykjqv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kzovpocd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xetzpyfv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2remumpag.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2koymgbyl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gopqhjlb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbebbzx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lsdjhmyc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rxyqpnlm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tkqktjjv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ieqqxwoy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dgxkgukl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2leebyvyy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahyksuqz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2sdqzpqld.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2oikecpde.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gdilcumu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2enrjkkvq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lolytsss.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mxfkpwfo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2racboqgd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yyoatahe.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yduejmpp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ryzshgpw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2whoosxii.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eqsuayru.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2incfexaf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ktjbxlww.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wkiqsvyt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sfpimobr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2okzfkglc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hlrpnbkz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qmumkbzx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2djrpwrjr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zpijmflp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnklakgy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pswykcwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfskpcer.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ejnufhth.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nlihtice.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bkaffbag.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwqtacg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2livvlfmh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zqejqthw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bymfevoa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifteaoyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lolrktqs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2khosgirk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2svxfwhhl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dxrrxnih.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mxduralj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2twmzpfsy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iwzeqpds.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qeuxlrfe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bieaasuw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvoadkvi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gmrulxip.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rwgfcgxi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2flzitznp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnpgvywj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lpnaimwy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bygcwcvb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2biqwbanc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hxdbqpgh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2euhssbcf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fkkdiwki.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lggleegd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uivefiza.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oypiggme.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lztbsffb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zcuzzted.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qackkpco.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bkgkovev.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jaevnsns.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2athkdtmf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2htiumqxd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jcdrxyia.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phdgphgq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwxmncsd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aevmgiyc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qbdkiidf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2snycqhgo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkgfianv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2opescmip.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kwqrmouu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hmjliozr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2osppjvze.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2trzpipgx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ckrokoxz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2elfyssaj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2avczsbxa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ouavmyrj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2elsulpzw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bbuelcor.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sofwmdwu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xjxmsbss.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qgcnnktz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2oroudpgd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mkbocpmi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hxrgbziu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mescfltu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2pvkyewcb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xcrnvovr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rzqooyoz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2knvaasmx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2trrwzgck.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ofwibjsz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wmuniawy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yuklvljh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rjjbbvyo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2tflslkbw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tsbswhef.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mhwvfivp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2tfjmypir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yfdrlorq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzcgylih.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xtdhbkuq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2sxpzebtc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gvfmmedp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2avjpomgr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2phpihhqn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jylkfjeo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2miygaybt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2caqoppok.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2umwsmcuf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2bkalqfqx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2cglldnkz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fjkpkgkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkfdtdcq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ozjqzmhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khsfpkkq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bhwbxint.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fdphzvzo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zicdfyic.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oczyoulf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rcbsfiya.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mfromtst.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2twbimwyr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2icknxvgb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fjhavsxb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gxnrtrel.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2clfuqhpk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ftmsajue.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tuqklytm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ignkjeru.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qwibqqjw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzahnxlg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rdvbrsuf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2apxitbgv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2rriwsfeb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsjmgeev.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rqfgcqhq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2atawiwtw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lylwjtfp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mcsukgnc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2prcpaghi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ygohuvpg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2rwlxwaxv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jfkovcfd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2nlaxvlyw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cqrsywcy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kekhesok.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dbmihnqz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qeircbtq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zkweqwte.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wqpjgyzb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dkzjbsaf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ohafqnkq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2faqbdmoo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2efpwsvqn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pziosjpw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vqlcibbp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qgyevifg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ralqpvdz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ubntnhiw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2obiwzhfm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2xhhbzxcr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iocywqpz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vujgtolb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2evjgumlw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ebcxvldn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fpjxkkcm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2wetyxuwz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jdyszthp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kpnlczpe.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2gnllwhqv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ioubapnw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zggwjwzw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hdxarfwe.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gcpgtizr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzxcapn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2xdpvuznf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bcvnniql.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2zebinvdh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjbmjk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2pktswbhc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lnshuvbt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2brkavelt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2txlaqlga.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ioyxpqdx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2jtmskysa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rieqiiks.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2snowllps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcnuxrno.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2vsymkvyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvctccfs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2irqhvexb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2vctdfimq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2duuslvts.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ogbhqroy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vrqpenni.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xlalqjjb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2zhzgisqx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2pvkujunj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ihaknkaz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zlaqfmqr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ktioqlug.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2rfyqmnph.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2sokbieot.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2pbfcvjtk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2trqmxuif.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2mwqgczwx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2olfnfqcc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ehbyrhpi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tszteftp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2aqrszvde.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2koqstfwh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mldfzjzx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wztrtxib.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xbskszoy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yyenusca.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vnredhsy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2pqddlcqh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mvgwonop.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcjigts.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2cgwavvyk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2myazwwyf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2uwzazebg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2lgtfwfsq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2atlkthwn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2frqzrvnx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ufooquig.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dhijmjet.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bugcyzft.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2edpzsrkg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sbvdozyg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uucbmyil.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2doeadtme.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yllwhsex.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2okemrwrp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rtujijdn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ehaipewm.html


<!-- 参考信息 -->