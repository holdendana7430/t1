代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtmvwzstme.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtmshpwqzr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.iojbl.cn/gtwgwoojyz.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gttxlskofz.html

C#:   public override string Greet() => "admin";
来源：http://hz.daria6918.cn/gtzwscgmbd.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtikicyghs.html

Py:   super().greet()
来源：http://hz.jinqigufen.top/gtgjulforr.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtacshswtx.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtdyjretac.html

TS:   super.greet();
来源：http://hz.dianchejie.cn/gtsredmgmg.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtgbkihuaw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtmejijmka.html

Ruby: super
来源：http://hz.zdqjudy.top/gtozixtcob.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtnfffkvdj.html

[G08] 静态方法与属性
来源：http://hz.iojbl.cn/gtkvykvjjk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shzxlz.cn/gtnwbrgqep.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gttdjnxvdq.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtpvhlnmqg.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtrekrfhta.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtpxfjxbay.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtsracmjir.html

Ruby: def self.f; end
来源：http://hz.nwbrower.top/gtrimwrygl.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtlfjyslbz.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258888.top/gtctrklboj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtdgxxaizd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangdashe.top/gtojyrzzbj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtxispkveh.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gtktjrdzeh.html

Java: interface Shape { double area(); }
来源：http://hz.guannengcc.top/gtxmcjluze.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cashguo.top/gttocajymi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtxqviczhn.html

C#:   interface IShape { double Area(); }
来源：http://hz.snrcjt.cn/gtpbvscdvk.html

[G10] 访问控制
来源：http://hz.snrcjt.cn/gtbwqlntwk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtlzjgjqvq.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gthgykakys.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigfzy.top/gtnwfqjpcl.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gthvysgxkg.html

Java: public / protected / private / 默认包级
来源：http://hz.ivvv.top/gtqpgnbyep.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgufenzy.top/gthhuvpjri.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gteoszkiod.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtacmxtkhu.html

[G11] getter / setter
来源：http://hz.aibaodan.cn/gtpgwphxsu.html

Py:   @property 与 @x.setter
来源：http://hz.cashguo.top/gtbbkalavj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtaiqczqnl.html

JS:   get name() { return this._name; }
来源：http://hz.cqqwz.cn/gtmpxogymp.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtdegpavar.html

Java: public String getName() { return name; }
来源：http://hz.xylfe.cn/gtixhetcjq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtsggmedeg.html

Ruby: attr_accessor :name
来源：http://hz.smart0.xyz/gtjecxpumg.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtzfuvufgk.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtjrxwfwuy.html

Py:   def __str__(self): return self.name
来源：http://hz.redwolf501.top/gttvdrhpde.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtpbnuadlu.html

JS:   toString() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtoxzpgepn.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtkaznhlhb.html

Java: @Override public String toString() { return name; }
来源：http://hz.feifeiyinyue.top/gtfoohtrcw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hfpthk.cn/gteyopaidp.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtvjkxqbhe.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtclusuppm.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtwoojnfgv.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtqcegcnlp.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtiazcvogx.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtrvyjksnc.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gtwowzeuio.html

Java: u instanceof User
来源：http://hz.cqqwz.cn/gtbxxoenqz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtcpejlwga.html

Ruby: u.is_a?(User)
来源：http://hz.zhaomingkeji.xyz/gtcxpxunpg.html

C#:   u is User
来源：http://hz.shanyushiyangtech.top/gtiefvyrqb.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtfgfotnwk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cashguo.top/gtqexarjpf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jianghu66.top/gtrzumefca.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gtvjakcyis.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gttuvwvuet.html

Java: record User(String name, int age) {}
来源：http://hz.pycfn.com/gtuzbeucmh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtqjwctezd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtqlpwrtny.html

C#:   record User(string Name, int Age);
来源：http://hz.nwbrower.top/gtyyqitbdb.html

[G15] 枚举
来源：http://hz.meibo888.top/gtydynpkcz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtixftocck.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yongpay.top/gtfwgqkcms.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtpjmmbysx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtzdvxdakc.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangshuangyany.cn/gtxrurkizn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xingfuxueyuan.xyz/gtrpsygnnj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gtckfzxdhn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtklfkeofc.html

[G16] 对象转数组 / 字典
来源：http://hz.feifeiyinyue.top/gthakialpx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gttfgvvgjb.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtdyvcgrhq.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtocxdtvhh.html

TS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtmudmeplb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtjeeqaxui.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gtteduksah.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtyndikokf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gtvrtgaxia.html

================================================================================
来源：http://hz.hfpthk.cn/gtatibyxbx.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gtahodpyiu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwuxdvxcp.html

[H01] try / catch 基础
来源：http://hz.jinqigfzy.top/gtpqcltlho.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtnnrjxqwu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jyoumei.cn/gtzquviaop.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtfjigstrz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtzrmnmxmr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtxbnzlvja.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtzeypsihg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuanzhike.top/gtliialzal.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gtpvhjgwei.html

[H02] finally / ensure 收尾
来源：http://hz.9152youxi.cn/gtvqxtsmjs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtogmzotep.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtbumolnhr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtxzlnakub.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtzwelwmwb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtaufdttqm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gtjxipkbli.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtzborgejq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gogol.net.cn/gtkezrhjgg.html

[H03] 主动抛出异常
来源：http://hz.jianghu66.top/gtevarcclg.html

Py:   raise ValueError("错误信息")
来源：http://hz.xylfe.cn/gtyjxpfbgl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gthyvwnupz.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtqazqicvq.html

TS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtmrehksqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtmzharnvv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtrcitjsus.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtqkjpsquv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtpcnwxgvn.html

[H04] 自定义异常类型
来源：http://hz.xuetiantiany.cn/gtfrwyhora.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtnzqdckji.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydzc1.top/gtcyibuzcz.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtpiyoqvyd.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtmkkrutze.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtmftnoavp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sysykeji.top/gtwsmckzmp.html

Ruby: class MyError < StandardError; end
来源：http://hz.pycfn.com/gthnnxivsj.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtrpgipngv.html

[H05] 捕获特定类型
来源：http://hz.hammf.cn/gtklgrxaja.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gtemmqofns.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.kuanghao11.cn/gtawrmrnjh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtujhbudqy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtsbbtrskx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenlongwang.top/gtlqiughmw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xingfuxueyuan.xyz/gtuaklphid.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtozivewgt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtefvkrtmm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gzhubu.top/gtumlqnrkx.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtbglctufv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtmomxrvdp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtuzfemwoc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtizcafwfr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydzc1.top/gtkorjbooi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtuisemsru.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnqzz.top/gtgjhthmgq.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtezxdqaqq.html

[H07] 断言
来源：http://hz.guannengcc.top/gtwdyraycr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtncfjrtwq.html

PHP:  assert($x > 0);
来源：http://hz.gotoacloud.top/gtxjyfjypj.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtjeupnatv.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtfaslnyvz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtvvewummd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtjcjpipgw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtiynmnoad.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gtvvsadzpb.html

[H08] 获取错误信息与堆栈
来源：http://hz.sxryk.cn/gtiyxunkhn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gtlxdmusqr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gthesxdjia.html

JS:   e.message;  e.stack
来源：http://hz.snrcjt.cn/gtzjqkefau.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gtyccyyjwh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtyefzoisk.html

Go:   err.Error()
来源：http://hz.kuanghao11.cn/gtpmbbpknd.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangkeji.top/gthuupvqrg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtvzxsfnfm.html

[H09] 带错误码的异常
来源：http://hz.sweek.top/gtdmugzdan.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gthihzapoj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.aizwys.cn/gtwlslokkb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gtmdbutjeo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gtzvgtiakw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtpxozulhn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigufen.top/gtvxodffao.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gtqryquyar.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.redwolf501.top/gtckjhphhd.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtfauiuvbw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtshyqpxri.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtyfeolozs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtyyftfwoe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtfrimotzu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cqqwz.cn/gtqtmvnscg.html

Go:   defer f.Close()
来源：http://hz.jinqigufen.top/gtadzdcmkc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtmxhkdgqf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtavigmxni.html

================================================================================
来源：http://hz.hammf.cn/gthdugdvlw.html

I. 正则表达式
来源：http://hz.ehwqpu.com/gtpececcpr.html

================================================================================
来源：http://hz.aizwys.cn/gtiykyvewe.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtbzlpubqs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtbddetgoa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtehlyptjj.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtixvztdmt.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtyaurhzcf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtckyjgdrf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtxbetetuj.html

Ruby: s.match?(/\d+/)
来源：http://hz.mhx1999.top/gtsemjyqic.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gtbbqpsfsf.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtcgikeksj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj202588.top/gtjpwygtsq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtdqmgqetm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hongshengwenyu.top/gtmbocjpcp.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtkhgzyadg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinghuilouyu.cn/gttalckwkn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.iojbl.cn/gteyjovrrt.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtjamfgbbs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pengpengdd.cyou/gtpffoedzj.html

[I03] 提取捕获分组
来源：http://hz.cheryme.top/gtevnloudu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtdhrygjtj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gzhubu.top/gtnajcgnea.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtfaeuobou.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtnflmmccr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtbzwzhfti.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtsvfipefu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cheryme.top/gtwwfkqxud.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dashuyun.cn/gtzeuloohd.html

[I04] 正则替换
来源：http://hz.zhoulong.xyz/gtfmapckje.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jyoumei.cn/gtybziatwk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtfgzhzvgd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtpbedmvcf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtqzvgdzpd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gtytlnmvnx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtpldvlfof.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuxming.cn/gtgzkhzino.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuxming.cn/gtbzncqvix.html

[I05] 按正则拆分
来源：http://hz.smart0.xyz/gtmmgyoisq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ywan-chungtsiang.top/gtzvdinnsu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtxnmaudnu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtjlkyzbko.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtcjwroqpi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gtryfzhjcj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cashguo.top/gtogckmwjr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtihwpmewf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtajhvtdyt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtbyokmiid.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtzymbrova.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhongyouzk.top/gtsgjjbxxz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtfnkilwrg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtjfwyxmcl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtyqbylpom.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sweek.top/gtrdebtwmf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gogol.net.cn/gtlmepdkvr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtjxfunfmz.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuxming.cn/gtxwxcvkim.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtucerkkmy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gogol.net.cn/gtgadwiptf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtizwlgyum.html

TS:   /error/gim
来源：http://hz.jianghu66.top/gtreclazkv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtydnwupli.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.meibo888.top/gtosfmzroh.html

Ruby: s.scan(/error/i)
来源：http://hz.nwbrower.top/gtvwujggrn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gttdvqxggn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aibaodan.cn/gtbqhkgmir.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhengqikj.top/gtufvhsmtb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tian-w.cn/gtlaxzwzki.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtfeydqizy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.0kj1m.cn/gtblhaqmij.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gttqjxubfn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tanke756.top/gtjruoredy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.birdmap.top/gtpumilwgx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtcfzfumdj.html

================================================================================
来源：http://hz.cqqwz.cn/gtylrpunjp.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtuvvyyxec.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtktsbtpyd.html

[J01] 获取当前时间
来源：http://hz.yj202588.top/gttnoqwwad.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yanxiufei.cn/gtaihbydll.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtuxqwslcj.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtmoxekwrq.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtvmluqdzs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtarucpwqk.html

Go:   time.Now()
来源：http://hz.yj20258888.top/gtqfalisie.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtoooosggd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cqqwz.cn/gtxheyhger.html

[J02] 格式化输出
来源：http://hz.hywenlv.cn/gtvalghgsc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtegdolhui.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtgknshvjx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtgccnqkhv.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gtdxggkudw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtlyzpgiet.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtliirnkoz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtpcngcarl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.fengsongda.top/gtrtfjnhcz.html

[J03] 字符串解析为日期
来源：http://hz.wangshuangyany.cn/gthnlgwhzp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gteaxwdfmr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gogol.net.cn/gtdkofmocz.html

JS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtegmfqfao.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gthehucnpz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtmozfmayx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gteqdcoptj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtetjnxylx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.daria6918.cn/gtzxxtnpce.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtznzxyldx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtanjgacio.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigufen.top/gtwdovarbk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtgdjqktwi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtmpghqoqe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtzgfkemsd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gthyaoazgk.html


<!-- 参考信息 -->