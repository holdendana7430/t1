代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gtwioieklm.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtldsmqtzr.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtkedcchkw.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtrfcrcanp.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtewmfsfiw.html

PHP:  class Admin extends User {}
来源：http://hz.shuidangran.top/gticzdsliz.html

JS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtkmfftsgn.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtftzpwnhf.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtdaqzydhl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtwdyjpzwg.html

Ruby: class Admin < User; end
来源：http://hz.jinqigufen.top/gtzwdzppkq.html

C#:   class Admin : User {}
来源：http://hz.wangdashe.top/gtbjokmdnd.html

[G06] 重写方法
来源：http://hz.wangshuangyany.cn/gtazkeicxp.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gtafvpazcy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtzquvwjvp.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtezkiitzo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtgoskwumj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtikttuucm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tanke756.top/gtkixsbpwv.html

Ruby: def greet; "admin"; end
来源：http://hz.tianlin.xyz/gtmquxwjaz.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gtdjgzmaaw.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtuwusmbyh.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtrkkbjajz.html

PHP:  parent::greet();
来源：http://hz.gogol.net.cn/gtrnuchmyc.html

JS:   super.greet();
来源：http://hz.ivvv.top/gtmvxzysub.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtmtclqdej.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtoqcdqizu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtlitrmusx.html

Ruby: super
来源：http://hz.ywan-chungtsiang.top/gttjlfeiyt.html

C#:   base.Greet();
来源：http://hz.jyoumei.cn/gtitvnendp.html

[G08] 静态方法与属性
来源：http://hz.chenzaomai.com/gtghhufhbt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtjjxrjite.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtptfwyfhi.html

JS:   static f() {}
来源：http://hz.c1oappe.top/gttozalevh.html

TS:   static f(): void {}
来源：http://hz.hammf.cn/gtithsnxlh.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtcuwjwnec.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtxrmklaka.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtcgnhvpou.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gtzgppibnd.html

[G09] 接口 / 抽象类
来源：http://hz.daxiang520.top/gtotmwocfv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pycfn.com/gtbabpnqre.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gtknkuhoya.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.redwolf501.top/gtcpayddpw.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj20258.top/gtfzhhpztv.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtgyhnayrk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yonumen.top/gtggqbibjq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.c1oappe.top/gtsmzwmxty.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gtxrbnjljk.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gtvmyisrxs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtslprwewx.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gtkjfsjpyq.html

JS:   #private 字段；其余公开
来源：http://hz.ivvv.top/gtpshkdhfs.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtgbmvimrh.html

Java: public / protected / private / 默认包级
来源：http://hz.ehwqpu.com/gtyvllpzpu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daria6918.cn/gthgeouiyp.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtmgmnsnqz.html

C#:   public / protected / private / internal
来源：http://hz.svipenyu.cn/gtsxoflcgz.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtdonjhken.html

Py:   @property 与 @x.setter
来源：http://hz.meibo888.top/gtrvjtkixt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtbwvybskk.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gtpqozondb.html

TS:   get name(): string { return this._name; }
来源：http://hz.9152youxi.cn/gtcdsdxgun.html

Java: public String getName() { return name; }
来源：http://hz.bjfxy.top/gtgjwamula.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtfqjtjnxy.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtbnsomutk.html

C#:   public string Name { get; set; }
来源：http://hz.ivvv.top/gtmnsjdvzo.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtwodeoejr.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gttendsdcp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gthciwubfm.html

JS:   toString() { return this.name; }
来源：http://hz.cucudq.cn/gtmfrmyuuo.html

TS:   toString(): string { return this.name; }
来源：http://hz.sweek.top/gtinmjbvdz.html

Java: @Override public String toString() { return name; }
来源：http://hz.sufxvd.cn/gtksxswrgc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gtmdhsktvs.html

Ruby: def to_s; @name; end
来源：http://hz.9152youxi.cn/gtfiknenwv.html

C#:   public override string ToString() => Name;
来源：http://hz.zycfv.cn/gtcgersndy.html

[G13] 判断对象类型
来源：http://hz.dianchejie.cn/gtusapmntk.html

Py:   isinstance(u, User)
来源：http://hz.hnqzz.top/gtsafslsfs.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtlgvdshek.html

JS:   u instanceof User
来源：http://hz.hywenlv.cn/gtktxknevi.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gtumclpmxm.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtitnvneoi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gtortpirjl.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtojauerzo.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtgurcfsga.html

[G14] 数据类 / record
来源：http://hz.316326.xyz/gtmoyharcq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtyzryugpj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cucudq.cn/gtkfloewyo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtklygbjtl.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtzudybove.html

Java: record User(String name, int age) {}
来源：http://hz.nanxinkj.top/gtgwfoyzmj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtarqwlreu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gtfcjtqbwj.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gtzecfztgt.html

[G15] 枚举
来源：http://hz.andypj.xyz/gtwcwzmmtt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtaldcktze.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dianchejie.cn/gtaipqaqzm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.316326.xyz/gtwzrfsmsg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtzrredvny.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gthoizkjof.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenjidiqi.icu/gtkzebfocv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtqmpcsngb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtohwaxmxb.html

[G16] 对象转数组 / 字典
来源：http://hz.pycfn.com/gtcnapnwyi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtzxknvgfo.html

PHP:  get_object_vars($obj);
来源：http://hz.cashguo.top/gtxzpuhmss.html

JS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtipalnwyr.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtwufamqzv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gthzjidofm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hywenlv.cn/gtxdcozbxl.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gtwohshppx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gthhxwjciv.html

================================================================================
来源：http://hz.hnqzz.top/gttlmunhkc.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtloircyby.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcnqqkxnk.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gtlkuuvcbg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cheryme.top/gtqfezdeij.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gtmpkjhhpe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtkcupstbq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtbcbslsmh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtgqemjnre.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gtksnepnld.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydjk.org.cn/gtgavcxmlk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.havefunace.top/gteuwextys.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtjgywvmcq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtqdodcbzg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtpygefjsp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtzblufbcg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtevotypgs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtsvjpikbx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gtcwrpfyxr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangtech.top/gttcsqmnlp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtwymmpaeg.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtqecwhaim.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinghuilouyu.cn/gtsyhaesgi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtssgfwtar.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtzlyroiuk.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtpsyhuyob.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gthjnmemjt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gthdajpxzy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtslcinwpe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtkekhudjk.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtdotxcevx.html

Py:   class MyError(Exception): pass
来源：http://hz.hysaishi.cn/gtxojpvtpz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtlnrulbwt.html

JS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtkvopjmlf.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtikvyrivx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtsuyrmhet.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtryecbooz.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinyuanbaomall.cn/gtefsaxwld.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtlmokxodu.html

[H05] 捕获特定类型
来源：http://hz.sysykeji.top/gtvcbpalxt.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtfdzfeyiw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sweek.top/gtdyggecfr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gtquksllne.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtfscfjbcq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangkeji.top/gtrhcahuba.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jyoumei.cn/gtqswqxsst.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gtzkipgduv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtksgdameo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtsqlnmnes.html

Py:   value = d.get("k") or default
来源：http://hz.jianghu66.top/gtsicryumr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtuyvitaan.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtpqkwykcz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gttxqqmhjj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258.top/gtagfryvqd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gtqzikuuyt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtqimqoatb.html

C#:   obj?.A?.B ?? default
来源：http://hz.yvedp.cn/gtykgswlth.html

[H07] 断言
来源：http://hz.zycfv.cn/gtsgksakji.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gtgjblhgwf.html

PHP:  assert($x > 0);
来源：http://hz.feifeiyinyue.top/gtahozgigv.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtoqjqszen.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtynpytiey.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj202588.top/gtuhjnfpel.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtzuytyrxb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj202588.top/gtajjjbgjo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtuwmbjgrh.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtzkhyagwp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtexxdrhxk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.9152youxi.cn/gtufsbfwhp.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gtzsfkdaaw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yvedp.cn/gtmrpnyups.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtqxhadiix.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtpuqlcauk.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtbnrvhxzf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sysykeji.top/gtmnxgiaxs.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtkbzrejwl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtlqtpkazl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zycfv.cn/gtbpufhgbk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ybcxt.top/gtzcdlprws.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtkkhrphqw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.redwolf501.top/gtecnbvqip.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtwofdegdz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cqqwz.cn/gtxaeuoevy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtxdsfbmdo.html

[H10] 资源自动释放
来源：http://hz.jianghu66.top/gttvbjpwum.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtgsuwvuam.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtohorznzw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtriurwxmx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ybcxt.top/gtlblnvixr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gttbmutesf.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtihhbbhmo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtynricrjt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtkhsmyobb.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbsapfmtg.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtchnpoype.html

================================================================================
来源：http://hz.jqgfzy.top/gtxdbjgkui.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gttjqnbodd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtnfposcpf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtesqcrwsl.html

JS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtqmqnrtql.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtoratnikw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtggcaqtne.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtavltyjsv.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtjxjhozjz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtmcfdjmzb.html

[I02] 提取所有匹配
来源：http://hz.gotoacloud.top/gtzixyxlwe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtvyoehusr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtkdiwekvi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.c1oappe.top/gtjdztxbnb.html

TS:   s.match(/\d+/g)
来源：http://hz.bjfxy.top/gtzbedaubt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fzhhl.top/gtzxpckwoy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtzeddnzle.html

Ruby: s.scan(/\d+/)
来源：http://hz.xziqi.cn/gtkonqbdxf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtdsaqhghb.html

[I03] 提取捕获分组
来源：http://hz.cheryme.top/gtzqeyyhlz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtqtcvjwxz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtunyudrnh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gttwaoobqm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtxdmqpmbt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gtlhwcarpj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtqlrshill.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jyoumei.cn/gtlslzftoq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigfzy.top/gtwhqbrdoh.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtllxmqsks.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinyuanbaomall.cn/gtbposvabv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtdweszsva.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtxrlwahsu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtzjtaymdn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gthnayancz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sweek.top/gtsfaqnimh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangshuangyany.cn/gtfoqppofb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gtaoerfplm.html

[I05] 按正则拆分
来源：http://hz.ydzc1.top/gtlxjwntar.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtxmmnigqz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zycfv.cn/gtjsciijow.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtckhacqks.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtmxtzicjh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gtnetsaxmv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtwgecmisf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtutyibarh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.vqdsnc.cn/gtyvtfpeeg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtcebbkcwf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtmeniicwc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtxhvzvrnm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtccvuyqfd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtsrbdijee.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtlarzycur.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhijiandao.cn/gtrcmyofxz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cqqwz.cn/gtvwsoifbh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtjusojlyn.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuetiantiany.cn/gthiwblsod.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangtech.top/gtrwnpfwml.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtrsvuandn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtwwsssetg.html

TS:   /error/gim
来源：http://hz.nanxuanxn.top/gtprmnfsyw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gogol.net.cn/gtfteumypt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gthylhtecn.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtdtrtkmvy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhoulong.xyz/gtlxgexxas.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sufxvd.cn/gtpqacivea.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gtazahqcwy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cheryme.top/gtbejcccrz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtmyzzobqy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtstghlhtv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtoddceaee.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258.top/gtwyymrnrf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhiwuduotai.top/gtrbtoiqib.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtoowthuil.html

================================================================================
来源：http://hz.yonumen.top/gtmwbmvbdk.html

J. 日期与时间
来源：http://hz.yvedp.cn/gtlmebykzc.html

================================================================================
来源：http://hz.nanxuanxn.top/gthnprcmii.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtyahhqqgj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtqruugjph.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtdyphywdw.html

JS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtjplgqjth.html

TS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtowyubgbe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guowangkeji.top/gtwuwnjrsi.html

Go:   time.Now()
来源：http://hz.daxiang520.top/gtltbdwskd.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtcoceqedu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtieridwzb.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtjxznoxsa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtyyqkmjle.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtgpuvexbv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtfbcjrbfw.html

TS:   d.toISOString()
来源：http://hz.0kj1m.cn/gtudfcswua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtbosylnkf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangdashe.top/gtthkadbrb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtmufrsmxa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtjunheusn.html


<!-- 参考信息 -->