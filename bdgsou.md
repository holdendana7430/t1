代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtgbfwkeby.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtlmaykavj.html

C#:   public string Greet() => Name;
来源：http://hz.shuidangran.top/gtnuglcspi.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtcodoseoc.html

Py:   class Admin(User): pass
来源：http://hz.hywenlv.cn/gtybcjfpvz.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtqhplxrkh.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtsallxkts.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtdyqbaqhz.html

Java: class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtnijmgizf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtsooqsnyf.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtmuyycnxj.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtgawfabmz.html

[G06] 重写方法
来源：http://hz.shzxlz.cn/gtivmtzmtc.html

Py:   def greet(self): return "admin"
来源：http://hz.zhaomingkeji.xyz/gtkpoavlyv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtzjtoayhx.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtwspalyuc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtbwudypdu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtshdcqamg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtnoozumbk.html

Ruby: def greet; "admin"; end
来源：http://hz.tanke756.top/gtfnyolzml.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtdgmuounp.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtrjhzgdhh.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtleesryld.html

PHP:  parent::greet();
来源：http://hz.xuanzx.com/gtdhwrrqqc.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtbsiunpqr.html

TS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtuwmhjrin.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gtaigwbklc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtxtftvabe.html

Ruby: super
来源：http://hz.xinyue.icu/gtjmrmbkme.html

C#:   base.Greet();
来源：http://hz.daria6918.cn/gtjuqvjdee.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gtytbruchi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtfaitzafu.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gtsliprgsm.html

JS:   static f() {}
来源：http://hz.jinghuilouyu.cn/gtvvwmsyjs.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gtokcincwy.html

Java: static void f() {}
来源：http://hz.daxiang520.top/gtqibtcdep.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangtech.top/gtifkuwvan.html

Ruby: def self.f; end
来源：http://hz.tanke756.top/gtvzdqooqh.html

C#:   public static void F() {}
来源：http://hz.cheryme.top/gtoneeteqv.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gttjpuzwvz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gttbzfvchc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zycfv.cn/gtdbuwkera.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yonumen.top/gtrbdxwegh.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtodtxusjh.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtgrbpxrwg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtgczgyhtz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.316326.xyz/gtskkqbvnr.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gttxqujure.html

[G10] 访问控制
来源：http://hz.sweek.top/gthsyppgpp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinghuilouyu.cn/gtbwltdelf.html

PHP:  public / protected / private
来源：http://hz.guannengcc.top/gtvkelmllw.html

JS:   #private 字段；其余公开
来源：http://hz.chenlongwang.top/gtzdthqqiu.html

TS:   public / protected / private
来源：http://hz.yvedp.cn/gtrazlsgpe.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gthkzdvqrw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangtech.top/gtzpwcvtcf.html

Ruby: public / protected / private
来源：http://hz.sweek.top/gtsoysutdd.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtmmxjerds.html

[G11] getter / setter
来源：http://hz.yvedp.cn/gtikpumemm.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gtktcydyqd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pycfn.com/gtwblgekyo.html

JS:   get name() { return this._name; }
来源：http://hz.cqqwz.cn/gtbvtvcejy.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtzjxphqad.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gtbgoqkzxn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cdnleiting.top/gtkparhuqw.html

Ruby: attr_accessor :name
来源：http://hz.zhengqikj.top/gtbybwusut.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtlhsnwllw.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtgcsbkhck.html

Py:   def __str__(self): return self.name
来源：http://hz.yj202588.top/gtqbcmgvwp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtxzfyodej.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtmsaufodj.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtfesejuuk.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtohvbslvg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gtiseoorcj.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtmalzdmen.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtudcmtdkg.html

[G13] 判断对象类型
来源：http://hz.svipenyu.cn/gtjlndpoki.html

Py:   isinstance(u, User)
来源：http://hz.cashguo.top/gtbzjldgyq.html

PHP:  $u instanceof User
来源：http://hz.yj20258.top/gtqurujcec.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtzxafqjye.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gtyprdpzev.html

Java: u instanceof User
来源：http://hz.gogol.net.cn/gtzlfxtopg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtylqcdean.html

Ruby: u.is_a?(User)
来源：http://hz.yueranfly.top/gtamwmmhxd.html

C#:   u is User
来源：http://hz.nwbrower.top/gthgsbbfyh.html

[G14] 数据类 / record
来源：http://hz.zhiwuduotai.top/gtvraikvrm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tian-w.cn/gtnykvroyn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtlsxwjtiu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtgbtjwixc.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtfubxfjkz.html

Java: record User(String name, int age) {}
来源：http://hz.gotoacloud.top/gtsdvyvspb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cashguo.top/gtfgnmllzd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtvtuxfxiy.html

C#:   record User(string Name, int Age);
来源：http://hz.pycfn.com/gtetwbrthp.html

[G15] 枚举
来源：http://hz.ywan-chungtsiang.top/gtvcgyltnr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hammf.cn/gtntmgbtex.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtvkpgqymf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinghuilouyu.cn/gtzvnumskx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtgcfmjhhv.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtyctmgvof.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hongshengwenyu.top/gtjtfqpkrv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.c1oappe.top/gtltvjfvgw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtbbkxjrwk.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtirunvwcf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.quarkkingdee.top/gtfcyoomli.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtlfftdenn.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtyilvqxts.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtoonnfnzk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.andypj.xyz/gtiudckdvl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hywenlv.cn/gtzevyztvw.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtslgzglmu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ppjwa.cn/gtmbyaojug.html

================================================================================
来源：http://hz.hammf.cn/gtmeofsche.html

H. 异常与错误处理
来源：http://hz.jinqigfzy.top/gtsmmwxrlb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtpedrouob.html

[H01] try / catch 基础
来源：http://hz.9152youxi.cn/gtnpykykgy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gtawwzumih.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtelgbvotb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtpaxzkzam.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtqdshsuai.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tian-w.cn/gtinfgmwlr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtygdixaow.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtqegfgvvj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yueranfly.top/gthobwndcs.html

[H02] finally / ensure 收尾
来源：http://hz.chenjidiqi.icu/gtvgoccgcr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtyurkiiup.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gthzobpumg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtmbsrsdvc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtjwovudvj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtuvbagbmh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuanzx.com/gtldncyeuc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtezvqpayf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtnwffhdfz.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtszepxhkw.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtoridykhl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.316326.xyz/gtmqyvdxnl.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtopzqpdql.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtxzygymkd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtnvsobflo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gogol.net.cn/gtjpvqroca.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.9152youxi.cn/gtrobsornh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gttvvcskzh.html

[H04] 自定义异常类型
来源：http://hz.nanxuanxn.top/gtwnxpzkup.html

Py:   class MyError(Exception): pass
来源：http://hz.yj202588.top/gtcyetfjzi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtmxlomvvb.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtcvgzutjc.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtkjjconzy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gtrbjtgkqs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtdbpdfhcw.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gthwhwlspz.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtecgooqww.html

[H05] 捕获特定类型
来源：http://hz.vqdsnc.cn/gtmsnxzdap.html

Py:   except ValueError as e:
来源：http://hz.ivvv.top/gteindsmsa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtwuqoafrb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtbpfjscng.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtpvelnnza.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtwzthaqkg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtzjhrusog.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtvzpdaebu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtttxxohtd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtdpwelvbs.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangtech.top/gtwuwqiynz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jianghu66.top/gtzddjvqlb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gttmgcsiwg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtmxzvzvnt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtfvlfgmft.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gtpuqfygxc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangshuangyany.cn/gtnhcvfuwj.html

C#:   obj?.A?.B ?? default
来源：http://hz.cqqwz.cn/gteltpxvjl.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtdbxawuvb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gtxvqyhyxj.html

PHP:  assert($x > 0);
来源：http://hz.yanxiufei.cn/gtckikgnzn.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtjlrnemfw.html

TS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtdcfixnqa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtggwulldv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gtimtpfhkf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtbmimgbgu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zycfv.cn/gtgwqduzjo.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtxmuhecxs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtqnnitbtf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxuanxn.top/gtlhhheqaa.html

JS:   e.message;  e.stack
来源：http://hz.ywan-chungtsiang.top/gtlppccaof.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.birdmap.top/gtftxujbkc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.birdmap.top/gttpnnwgxd.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtuzinegdz.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gthmyiwyhh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shzxlz.cn/gtgmqvtauw.html

[H09] 带错误码的异常
来源：http://hz.dashuyun.cn/gtibphlzbv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtbbkpsubz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtpqiishrg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtpqkrdqgb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.snrcjt.cn/gtaufignyl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtypdmvdev.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtwwtrafry.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtzbyiquuw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtiuloactb.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtazljxiwv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtrcsrhcwr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtesurokrx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtbhohdphr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtspyflmre.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtsgfmcgpg.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtlnuxhril.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtvoxzzfqy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sysykeji.top/gtjnvneiyk.html

================================================================================
来源：http://hz.gogol.net.cn/gtgingxglx.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gthlavaizh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmajsqluq.html

[I01] 判断是否匹配
来源：http://hz.guowangkeji.top/gtglkzknnr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtznffjzyv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fzhhl.top/gtzwgpminb.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtvtycqpgq.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtpjtozaup.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtwaixywzc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jiagoushi.top/gtlixaswks.html

Ruby: s.match?(/\d+/)
来源：http://hz.redwolf501.top/gtrsagqiwz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.0kj1m.cn/gtjryqlbft.html

[I02] 提取所有匹配
来源：http://hz.jqgufenzy.top/gtqjcsqhly.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gtlxuigidd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xylfe.cn/gttavnfrfi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhaomingkeji.xyz/gtmcvgnvuv.html

TS:   s.match(/\d+/g)
来源：http://hz.yj202588.top/gtdnuyztwd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtdfzncucd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yanxiufei.cn/gtdvcbkdzl.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtkyzuxsav.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtmklhicsm.html

[I03] 提取捕获分组
来源：http://hz.zycfv.cn/gtwefltlof.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gtupdcsrwd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cashguo.top/gtmogfvfqs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtfnjafimw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigufen.top/gtbsulyrfx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtibxqppkb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtytphkbqe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtzfvvgsew.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gttxsbwjpr.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtgrjrjzzg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gttbwuynvg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.vqdsnc.cn/gtqmsxmwmy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtsmohnxmk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtmfmerzbu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtqiuogozb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.vqdsnc.cn/gtspwrvzbw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenzaomai.com/gtebhdsbmn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtylecfhdz.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gttpdbtxud.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yongpay.top/gtgzpzfuph.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtywxquziz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtuobsqeew.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtceochxko.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fengsongda.top/gtdjvnhtku.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtdnnilrcw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtspyqrjwe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gteucyzpls.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtjrwjlbqn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtrwjrdsrr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtymuoryhn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtljhfauao.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtxwvqverb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtohlbaslb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.meibo888.top/gttiwjigti.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hysaishi.cn/gtxfuzqdch.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtzpcawswn.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydjk.org.cn/gtdndszsvm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinyuanbaomall.cn/gtiqlgnbwt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cheryme.top/gtukcspdrt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhaomingkeji.xyz/gtbpuaqxtu.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtcevkfcfx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gtrbcvkynd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gtqqxzstnr.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtrrcfefuj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydzc1.top/gtzneuaoov.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtjbfedxfa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtirmjffgy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.redwolf501.top/gttiksxvbq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtxhmgnldk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtjtofyzri.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtywpafswa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtzskmeyeg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daria6918.cn/gtkghpqqne.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtaxtvrujw.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtesospawf.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gtabgnimww.html

================================================================================
来源：http://hz.jqgufenzy.top/gtggnatjqw.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtpfzmerdj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtarfslfwd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtcdlnhaoe.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtrtptidsa.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtchrtpwlx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yongpay.top/gtnpfqnduu.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtczfiwntj.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gteofywftz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yangfankeji.com/gtdqmurqjz.html

[J02] 格式化输出
来源：http://hz.jinyuanbaomall.cn/gtsqsnobkv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtsbqjgxcu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gteejgpiqo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtivlwsswh.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtxdwspplf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yongpay.top/gtyenuunwl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cqqwz.cn/gtxpayxlse.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtglsklord.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gttzadwxry.html


<!-- 参考信息 -->