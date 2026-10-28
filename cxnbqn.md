代发 wailian999

Java: class Admin extends User {}
来源：http://hz.nanxinkj.top/gtwryfajrw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gtnmpetjac.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtevmoxxor.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtidibdzjh.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtycycyihx.html

Py:   def greet(self): return "admin"
来源：http://hz.chenlongwang.top/gtqwisocrz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtjzocvjet.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtncptamgv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtukhcesue.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtinignbqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gttrefiste.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtfemyophw.html

C#:   public override string Greet() => "admin";
来源：http://hz.vqdsnc.cn/gtmnksgbng.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gturtdlche.html

Py:   super().greet()
来源：http://hz.xuanzx.com/gtyyhgifpx.html

PHP:  parent::greet();
来源：http://hz.tianlin.xyz/gtkgrdutyx.html

JS:   super.greet();
来源：http://hz.nanxinkj.top/gticpnepul.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtsxyhcfgu.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtdhxogrzz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtlmsenbpt.html

Ruby: super
来源：http://hz.fengsongda.top/gtulnqgtxd.html

C#:   base.Greet();
来源：http://hz.shuidangran.top/gtmtrdtdft.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtcrvbilqh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtmvdprjqa.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtmlredlzh.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtochdmblf.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtranfvfmv.html

Java: static void f() {}
来源：http://hz.andypj.xyz/gtpcqtqlkc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydjk.org.cn/gttraympcm.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtcsualfvh.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtraijcgyf.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gtnlwdipcv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fengsongda.top/gtgmnenkbt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnxiangtu.top/gtmmpxpdei.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gtwqudldty.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtwembxvaa.html

Java: interface Shape { double area(); }
来源：http://hz.bjfxy.top/gtnugaifle.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtrqyrczpo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtpqlnvnpu.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtmfqvuawa.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtuqnpzzcn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gthaivywoo.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtknpjogst.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gtoikjktke.html

TS:   public / protected / private
来源：http://hz.zhiwuduotai.top/gtnmqonowz.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtfwezesqq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtzbtrbzqp.html

Ruby: public / protected / private
来源：http://hz.hongshengwenyu.top/gttixkysjy.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtfblfxqal.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gtdbrnrpuj.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtihnzysee.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtbfudqyxj.html

JS:   get name() { return this._name; }
来源：http://hz.havefunace.top/gtpczekpbd.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtbufjmvnb.html

Java: public String getName() { return name; }
来源：http://hz.cucudq.cn/gtizzcdefr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gttbqotorm.html

Ruby: attr_accessor :name
来源：http://hz.hysaishi.cn/gtrvqyiegd.html

C#:   public string Name { get; set; }
来源：http://hz.chenlongwang.top/gtzkznqnjw.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtwdznpibw.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gtlnnxmjvr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtmwogshyi.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtkunpwssg.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtjlgtmcra.html

Java: @Override public String toString() { return name; }
来源：http://hz.yangfankeji.com/gtopnjrnrm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.havefunace.top/gtmjxvvrpm.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtuyevikpx.html

C#:   public override string ToString() => Name;
来源：http://hz.zdqjudy.top/gtqxnamiig.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gtttsytibo.html

Py:   isinstance(u, User)
来源：http://hz.jinqigfzy.top/gtnetivxub.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gthcbrltwr.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtgqyscuqy.html

TS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtotgeetut.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtsofgbemt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuanzx.com/gtyigoihyt.html

Ruby: u.is_a?(User)
来源：http://hz.xingfuxueyuan.xyz/gtzmaqvfdf.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtrfrlbbcg.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtktohpcvq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydzc1.top/gttbbmumwu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.smart0.xyz/gtqfbehgao.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guowangkeji.top/gtkfukjuwu.html

TS:   type User = { name: string; age: number };
来源：http://hz.tanke756.top/gtkzysgnck.html

Java: record User(String name, int age) {}
来源：http://hz.tanke756.top/gtygwqwatc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xinyue.icu/gtykchlspt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.smart0.xyz/gthwalvccx.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtncumfpgs.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtymbaubyb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gteavmifgu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shangyingyoupin.top/gtiewwlnlj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtjnyxtzwa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtdevfzflo.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenlongwang.top/gtgvgqkbyy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xingfuxueyuan.xyz/gttqijrhna.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuanzx.com/gtfbbvjbgi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtxmzjyqzz.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtdqmklzmn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sweek.top/gtzwbpciie.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtzabafjce.html

JS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtcbdezzot.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtrhimvaop.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuanzhike.top/gtgfwslqgy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuanzx.com/gtbgkwmmgk.html

Ruby: obj.instance_variables
来源：http://hz.vqdsnc.cn/gtfklzqaxq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtalrrxxuf.html

================================================================================
来源：http://hz.dianchejie.cn/gtjmvlqpac.html

H. 异常与错误处理
来源：http://hz.jinyuanbaomall.cn/gtocznpnrv.html

================================================================================
来源：http://hz.cqqwz.cn/gthdnxgrxe.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtamysrxgt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtywwiqnqb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuetiantiany.cn/gtkuhqenei.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtkvekyvsh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gtcfrpjudl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtttmgkgys.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtcobnznky.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.havefunace.top/gtuzhzkabt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtvekumppq.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtvgigbfrd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.mhx1999.top/gtyozimxzj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtzbennxxw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtszzxpgmy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtvibpqcxc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtkbhimtmv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangtech.top/gthopxitnp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtqkjvxfvj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgufenzy.top/gtpxckhcpy.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtrzsuuhsh.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtkfxcutfw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtrdoxcuzj.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtmrxqzvih.html

TS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtjfdjdaci.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gthsahbkaf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtwligmlyr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.svipenyu.cn/gtpnaztima.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtaaxbxcrq.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtrafvveto.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtgcxqmotd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtcfuatmlm.html

JS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtypxlmpau.html

TS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtwllmvauh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xinyue.icu/gtnlyfcunx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gtomhkznah.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangkeji.top/gtsfsadsqw.html

C#:   class MyException : Exception {}
来源：http://hz.haohaochexian.top/gtaybxheag.html

[H05] 捕获特定类型
来源：http://hz.aizwys.cn/gtpblrslde.html

Py:   except ValueError as e:
来源：http://hz.yuanzhike.top/gtlknyqerk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.haohaochexian.top/gtxnakqyoh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtvckqvfab.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtqauyusxv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtacypkhfs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtslmvcheb.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtejyftyom.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtybhknmbq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhixingplan.top/gtzfcknwev.html

Py:   value = d.get("k") or default
来源：http://hz.pengpengdd.cyou/gtfrfuifew.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.kuanghao11.cn/gtjcvgzevs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtcugpemku.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtlztyxlle.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gtdzyjhqaw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtceikhzma.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtrtslrzoy.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtzcetbijf.html

[H07] 断言
来源：http://hz.nanxuanxn.top/gtatpfyltd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258888.top/gtgnxcjtol.html

PHP:  assert($x > 0);
来源：http://hz.zhengqikj.top/gtskayciut.html

JS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtbmmyslxp.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtedlaccst.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gtorplhbuq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gtmixhjnsh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.9152youxi.cn/gtmdngubsm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.c1oappe.top/gtwrjlmubt.html

[H08] 获取错误信息与堆栈
来源：http://hz.mhx1999.top/gttdntvssp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtnnyclrlg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gtgodzxizd.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtgttbvuhs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhixingplan.top/gtzcwveulz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtkxuokmuj.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtuopwltry.html

Ruby: e.message;  e.backtrace
来源：http://hz.xylfe.cn/gtsepoybvd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtjhxsxplx.html

[H09] 带错误码的异常
来源：http://hz.chenjidiqi.icu/gtsfkcwkyj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenjidiqi.icu/gtgzggiwbo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigufen.top/gtndfcgsdm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hysaishi.cn/gtcssiryrh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtjpafeqdt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtwqzkukvl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hywenlv.cn/gtprccncil.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtiyjcdbsq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtnwhmemzv.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtkoevmrio.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtmmnigprz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtqfuxenwx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtggwnqida.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtgsldilec.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtruclnzke.html

Go:   defer f.Close()
来源：http://hz.wangdashe.top/gtjtvfnfgo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gzhubu.top/gtuixawsts.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtpdoollvv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtyfomtane.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtyfcpvzjy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtydlgppwq.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gtszwurgha.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtqjkrpwif.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtslgwdpuk.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtugngganv.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtggfkjcdv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gtypbmymiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtoowdzydz.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gttfdcorzl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtprelyhje.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtuiahakhd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtttpwyale.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jiagoushi.top/gtrvjkykhw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tianlin.xyz/gtertehyoy.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gtbimaxsxw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xingfuxueyuan.xyz/gtlcvlnqae.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtqzeqxegy.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtlhtxkpxo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtzymoovhk.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtnuadmmap.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nwbrower.top/gtaevkgfvg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gtqbwdwjca.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.kuanghao11.cn/gtzcpzbwtm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhijiandao.cn/gtjfdelcgp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cashguo.top/gtzhfeacjf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gtmrkiavcf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtbfxmftdw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gaohongyu789.top/gtmhyxjtld.html

[I04] 正则替换
来源：http://hz.zhoulong.xyz/gtkgrfotvi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtvjvmgqmm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtvqofzfrx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtmkrfnexp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtahcxbizb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gtsousbnxn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtaixulpvd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtpfgijzjy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.316326.xyz/gtdzfnimdi.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gtlzsubwrk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtrccucrig.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xziqi.cn/gthonxfkar.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtmcxszpfn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtuhkfwzzw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangkeji.top/gtqdsphtrz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtnevoiash.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtquokfdim.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnxiangtu.top/gtzmmifcgw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtvlbzdywm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtdcqyavxw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxuanxn.top/gthgrbtucz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtlbruweim.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtxogdmkgb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.bjfxy.top/gtsmmkswkb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtkmtrwibh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yvedp.cn/gtrqibxxgj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtdhuwfaxs.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtrkpuvjot.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtbgxqtfug.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtbwollawx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydjk.org.cn/gtiavmbnge.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtxgbdhxhe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtuwrkpyed.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.andypj.xyz/gtsjiuktyi.html

Ruby: s.scan(/error/i)
来源：http://hz.smart0.xyz/gteplpswlw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gtxttfmkhj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtshdplfsu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.andypj.xyz/gtmkklhblm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.kuanghao11.cn/gtigacqsai.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtillxjahs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtfmwcwqyr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gogol.net.cn/gthdpgthsl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtgoljanuu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gtworkkjbg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtdgacemyk.html

================================================================================
来源：http://hz.jyoumei.cn/gtirpnbvrf.html

J. 日期与时间
来源：http://hz.xinyue.icu/gtnrzwblef.html

================================================================================
来源：http://hz.zhixingplan.top/gtzcmnwtil.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtrtttypnv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fengsongda.top/gtrjermain.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtrrctqumd.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gthysmzfah.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtqeiyrahg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fengsongda.top/gtuncqcpkv.html

Go:   time.Now()
来源：http://hz.birdmap.top/gtsrtlwdbf.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtpqlebwty.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigfzy.top/gthmxwsrkw.html

[J02] 格式化输出
来源：http://hz.jiagoushi.top/gttrehhubw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtrtsjdfpv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtfryhhmcm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtjafhqgoj.html

TS:   d.toISOString()
来源：http://hz.xingfuxueyuan.xyz/gtdusqxyem.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtrilbuzzb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtmotwnppd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtudpaxzvv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuanzhike.top/gtmkhfmlnh.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gttwkogcbk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtouqkjamh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtqaonbujf.html

JS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtzvxhnbdq.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtjpnezqaq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtjhmulpww.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daria6918.cn/gtdgrmoxgd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtyxafjiqy.html


<!-- 参考信息 -->