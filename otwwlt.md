代发 wailian999

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtibhsmsfb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtqtrhlrac.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtqcxhwofr.html

C#:   class Admin : User {}
来源：http://hz.aizwys.cn/gtkypggijj.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gtlrxdneoj.html

Py:   def greet(self): return "admin"
来源：http://hz.wangshuangyany.cn/gtmemildkg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtmvdytezc.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtnesgqhqr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtjnitquxb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtrcstlhvf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtydwttgsc.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtkwdkroiu.html

C#:   public override string Greet() => "admin";
来源：http://hz.shangyingyoupin.top/gtnzvjunbt.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtybbmkune.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtvtshrfpq.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtizanzord.html

JS:   super.greet();
来源：http://hz.daria6918.cn/gtnnipiads.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtfghllqat.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtdabzgtsn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cashguo.top/gtrmmltykh.html

Ruby: super
来源：http://hz.guannengcc.top/gtvwssxgrg.html

C#:   base.Greet();
来源：http://hz.xingfuxueyuan.xyz/gtkrwjsecp.html

[G08] 静态方法与属性
来源：http://hz.yvedp.cn/gtojrzhyyn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ivvv.top/gtdvbfswfp.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtwgkjshpx.html

JS:   static f() {}
来源：http://hz.shzxlz.cn/gthwprmkux.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtlycmqmuu.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtwcciwxnr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtoenryckf.html

Ruby: def self.f; end
来源：http://hz.yongpay.top/gtvsomhedr.html

C#:   public static void F() {}
来源：http://hz.ivvv.top/gtnndmsblp.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtjiqukxyh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgufenzy.top/gtneftxkxc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jiagoushi.top/gtezhlsuel.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hysaishi.cn/gtbcjjsbdf.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangkeji.top/gtoinbcwis.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gtkritfdcl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gttsrezesz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gotoacloud.top/gtvyvqhivj.html

C#:   interface IShape { double Area(); }
来源：http://hz.bjfxy.top/gtwlaxexvb.html

[G10] 访问控制
来源：http://hz.zycfv.cn/gthajdzpol.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtkevrnlsg.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gtigbukgad.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtozrwtxqs.html

TS:   public / protected / private
来源：http://hz.zhaomingkeji.xyz/gteezubjkh.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtyvdzqkxo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtkmzdqlvl.html

Ruby: public / protected / private
来源：http://hz.cheryme.top/gthhnrovmm.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtzidbrtiy.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gthfdmgqlk.html

Py:   @property 与 @x.setter
来源：http://hz.tian-w.cn/gtogruxyfg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.birdmap.top/gtfrloermb.html

JS:   get name() { return this._name; }
来源：http://hz.hammf.cn/gtoytfkeyq.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtmqctkhpx.html

Java: public String getName() { return name; }
来源：http://hz.xylfe.cn/gtswcihhev.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yvedp.cn/gtclwqhwrj.html

Ruby: attr_accessor :name
来源：http://hz.feifeiyinyue.top/gtzrhbfmej.html

C#:   public string Name { get; set; }
来源：http://hz.jiagoushi.top/gtegdklkmg.html

[G12] 对象转字符串
来源：http://hz.hnxiangtu.top/gtymoiehal.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtpjbyuwxu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuxming.cn/gturdaensh.html

JS:   toString() { return this.name; }
来源：http://hz.nanxuanxn.top/gtfjfkqgyf.html

TS:   toString(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtqespgfcf.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtwahcdozw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtwisuniio.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gtolraujza.html

C#:   public override string ToString() => Name;
来源：http://hz.iojbl.cn/gthumgdlim.html

[G13] 判断对象类型
来源：http://hz.birdmap.top/gtxrlxultj.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtmbmuqpve.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtfpfxocvj.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gtkpuxvksa.html

TS:   u instanceof User
来源：http://hz.tianlin.xyz/gtbswkietq.html

Java: u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtcjacbmcx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hammf.cn/gtfnzemnru.html

Ruby: u.is_a?(User)
来源：http://hz.jqgfzy.top/gtnueaeyws.html

C#:   u is User
来源：http://hz.iojbl.cn/gtcondfdcl.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtglwyzswx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gtvyabpjyc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtyviskkxz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtgfhzsxxi.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtbzjdwruf.html

Java: record User(String name, int age) {}
来源：http://hz.haohaochexian.top/gtnjlrbtpd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtieyzmjrg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dianchejie.cn/gtcfdawcbi.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtmoulozva.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtmyiyswik.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtqmlaqqdb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenlongwang.top/gtexwisugl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jyoumei.cn/gtydcdibvb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtynfizyfz.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtbvhwvfqh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtpmnzmlbk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ehwqpu.com/gtsahpfypt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtqycmmbnh.html

[G16] 对象转数组 / 字典
来源：http://hz.redwolf501.top/gtfxdfupiy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gttzrpkijz.html

PHP:  get_object_vars($obj);
来源：http://hz.zhijiandao.cn/gtzgrqrmbb.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtlqzytnla.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtozxjxeqd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtqfqvyvdg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dashuyun.cn/gtortmofvu.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtksxmsikn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtpgrrkawp.html

================================================================================
来源：http://hz.316326.xyz/gtmxoqjcnb.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtfxtjpflk.html

================================================================================
来源：http://hz.316326.xyz/gtgatnrpmw.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtipejgjfb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gtjxxhlnwf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.0kj1m.cn/gtpxpwdvyd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtijqobgwj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtyejjaakt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtslozwyfg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gthsarnxtw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangdashe.top/gtipbvlbdc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fengsongda.top/gtkbegupko.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtfwrynzxd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtvkyruuyv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtuqjluhfa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtjxlgdcdo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gthplszizk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtihvxjbvz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtrbwbouak.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtqmhhthpt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daxiang520.top/gttbvcglkd.html

[H03] 主动抛出异常
来源：http://hz.gzhubu.top/gtkjnfeixk.html

Py:   raise ValueError("错误信息")
来源：http://hz.havefunace.top/gtpcdbdcmy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtebppmcqc.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtkaxqksqh.html

TS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtknfmbcjn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtybtrgkzq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtiwzzqmqp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj202588.top/gtpmcyeyyy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtzilogbvf.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtteensihd.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtdhotibdf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtmhczorzs.html

JS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtygispdgs.html

TS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtuzumggkz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtzphgajiq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gttsrfkedi.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtcfyspnkd.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtvppvetho.html

[H05] 捕获特定类型
来源：http://hz.smart0.xyz/gtegyctiso.html

Py:   except ValueError as e:
来源：http://hz.hysaishi.cn/gthczattrn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.0kj1m.cn/gtegswhyit.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtqtnjemyc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtfsynicdj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xziqi.cn/gtperqoxns.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gtvfalcbhp.html

Ruby: rescue ArgumentError => e
来源：http://hz.iojbl.cn/gtnrcfthek.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gttrctcztc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ivvv.top/gtogxoowix.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gttnwgtdhg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daria6918.cn/gtvacipxdm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtaxhrykte.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtnvajwcvi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yanxiufei.cn/gtznhztagm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gtgswxsixh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ywan-chungtsiang.top/gtluzwuupy.html

C#:   obj?.A?.B ?? default
来源：http://hz.c1oappe.top/gtfcqhnvjk.html

[H07] 断言
来源：http://hz.yvedp.cn/gtjezbqtpe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gtkjalrybt.html

PHP:  assert($x > 0);
来源：http://hz.iojbl.cn/gtxbomhfjl.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtrxyjmebf.html

TS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtkriudkki.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gtvusywwfc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtjiuehwws.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gtpefwkyau.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtjcvqkrtq.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gttbvwprwg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhijiandao.cn/gtaiywevye.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangtech.top/gtxsibnowy.html

JS:   e.message;  e.stack
来源：http://hz.tianlin.xyz/gtpwympmmj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtcynhodww.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shangyingyoupin.top/gtblshpbob.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtzhthikjb.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtqldiwhom.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtoveufahb.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtinqftabw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtqgygfnzp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pengpengdd.cyou/gtzayjwask.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gtfsvziqoc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtusfxcabp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnqzz.top/gtmrbwqibm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gthrpybdly.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yongpay.top/gtiagzmpka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hammf.cn/gtabiswpdj.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtaxmgbpfc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhoulong.xyz/gthrjbzstb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhaomingkeji.xyz/gtlekxwzug.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtlvqaeokx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtvlbugzsk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtphekrevs.html

Go:   defer f.Close()
来源：http://hz.jlsjyb.cn/gtcdecvsws.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenjidiqi.icu/gtadxbwlen.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xziqi.cn/gtwjrhyrfe.html

================================================================================
来源：http://hz.jqgfzy.top/gtmclqewvd.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtwtrnfqgw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvbrqnhio.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gtiryzyleh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtxjswwbjt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yanxiufei.cn/gtrolpyptp.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtdsdysrmk.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtctxzibsc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gthubfbnzf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtepqcfsbd.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtgcgwvlzf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenlongwang.top/gtrpajxwnc.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtwuwrozov.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtmvhzzdgy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtbssunyby.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinyuanbaomall.cn/gtkdphkqrv.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtbkdnolmw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.316326.xyz/gtuumyziss.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhixingplan.top/gthppoxfvh.html

Ruby: s.scan(/\d+/)
来源：http://hz.meibo888.top/gtvwyvqsel.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtkprglwyf.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtblngjabd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gteiflnmek.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtvtenwcgo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtdkkdprma.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jiagoushi.top/gtyynregve.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtnfdulnxc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtmtxvopsq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtrsylaaua.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jyoumei.cn/gtfztzhdaz.html

[I04] 正则替换
来源：http://hz.feifeiyinyue.top/gttfezimic.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtlgxqopkj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtbrmjffoh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtrnbmgvib.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtsuuwpkzi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gtmjngpxbl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtnesttfcw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.feifeiyinyue.top/gtvcmxiyid.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuxming.cn/gtmlhgtpdq.html

[I05] 按正则拆分
来源：http://hz.bjfxy.top/gtijbhteha.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtcvqybese.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yueranfly.top/gtlbajqubq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtrktlsafc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtcfyddxti.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtkkckoerj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gttjavkean.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtclzdwenb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gtkcrtylvi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cdnleiting.top/gtkrvunoqp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gthzydxryf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtmlfyawrr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtbqypfixj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gtjhqtumdh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.c1oappe.top/gtilbmgosx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258.top/gtuepvhhlq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtpdwsfkqh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtiouzhutt.html

[I07] 忽略大小写与多行模式
来源：http://hz.smart0.xyz/gteixhfryk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cdnleiting.top/gtxxilxzpj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cdnleiting.top/gtycbgxicj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtsgprzqyf.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtoupwaxqz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinghuilouyu.cn/gtjalieulo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtalpnwpmu.html

Ruby: s.scan(/error/i)
来源：http://hz.kuanghao11.cn/gtfwycrltj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtzroezzzx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gtyfulqcfe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtawmhqsgv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtvregitxd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtmmzwlvuk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtasujavtr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cheryme.top/gtpdxacnpx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtcflkezna.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yanxiufei.cn/gtghtwyrqd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtouhvlxwv.html

================================================================================
来源：http://hz.yj20258888.top/gtaqylgbxj.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtsfgvpzog.html

================================================================================
来源：http://hz.chenzaomai.com/gtvxnkncsj.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtcjluzrtz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sweek.top/gtddrqaygh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtznajpiec.html

JS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtzlosfole.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtmyjbtcje.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hysaishi.cn/gtcabbhiza.html

Go:   time.Now()
来源：http://hz.cqqwz.cn/gtussmgfte.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtktvxpfqx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.316326.xyz/gtipsgwuxa.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtkfxuoduy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtiqimegxr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtogsvrykc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxinkj.top/gtvfoeglbl.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtzvhrijqt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtwalwpdcd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.andypj.xyz/gtzbgwdxmc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtfbzihcrk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nwbrower.top/gtyfzmrrgg.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtfsrkllzq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cqqwz.cn/gtwdjpazun.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtkmeuooxy.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtvwnqancd.html

TS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtvpxzujag.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtkiavrunc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuanzhike.top/gtlyacmcfi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtbqtkszra.html


<!-- 参考信息 -->