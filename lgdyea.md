代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.daria6918.cn/gtgtdwqtnh.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtnshsgwpn.html

Py:   super().greet()
来源：http://hz.shangyingyoupin.top/gtsaskqrud.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gtapmlxbbk.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtwlnsdgqn.html

TS:   super.greet();
来源：http://hz.jiagoushi.top/gtilxfdumu.html

Java: super.greet();
来源：http://hz.hongshengwenyu.top/gtnafcnavq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtxglepmqs.html

Ruby: super
来源：http://hz.fengsongda.top/gtwtetwosp.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtborjoodx.html

[G08] 静态方法与属性
来源：http://hz.hongshengwenyu.top/gtrnwwxqhc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinghuilouyu.cn/gtenoclnms.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gtucrfvias.html

JS:   static f() {}
来源：http://hz.ivvv.top/gtkaszclsh.html

TS:   static f(): void {}
来源：http://hz.cheryme.top/gtbyvydzbl.html

Java: static void f() {}
来源：http://hz.pengpengdd.cyou/gtgckykglb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuetiantiany.cn/gtvjspmher.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtrfyqzftj.html

C#:   public static void F() {}
来源：http://hz.yanxiufei.cn/gtbmagbjew.html

[G09] 接口 / 抽象类
来源：http://hz.gotoacloud.top/gtkehphryu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hywenlv.cn/gtaowrgphe.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtqoefxmxr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.havefunace.top/gtnrymmowj.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtgrbvnpmj.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtigdpfogc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ppjwa.cn/gtbdeeugqc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtpzxlgmtd.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gtoqzcvmlc.html

[G10] 访问控制
来源：http://hz.hammf.cn/gtryzfdyif.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangkeji.top/gtkcnxvqux.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtgsdxhasj.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gtypzmomkc.html

TS:   public / protected / private
来源：http://hz.yuxming.cn/gttaxgwdmq.html

Java: public / protected / private / 默认包级
来源：http://hz.cheryme.top/gtxyhmhwke.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtadhndhis.html

Ruby: public / protected / private
来源：http://hz.guowangkeji.top/gtisligzyi.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtygimydwi.html

[G11] getter / setter
来源：http://hz.xuanzx.com/gtfyrospja.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtsidfqtnd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtzjcqzuzv.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gtdrbajgdk.html

TS:   get name(): string { return this._name; }
来源：http://hz.meibo888.top/gtnjskqjmg.html

Java: public String getName() { return name; }
来源：http://hz.yj202588.top/gtvdueopqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aizwys.cn/gtvaoxzklh.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtmwandtab.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtthpbimpd.html

[G12] 对象转字符串
来源：http://hz.ydjk.org.cn/gtzfrfvzet.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtvyszmydu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtfqjjidpe.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gttpqphdsc.html

TS:   toString(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtopqyeihr.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtcstxmgdc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtjwmkwycd.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtsfpwqlbk.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtrxregeyj.html

[G13] 判断对象类型
来源：http://hz.zycfv.cn/gtvllceokt.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtoakvyogg.html

PHP:  $u instanceof User
来源：http://hz.hnqzz.top/gtcdsaoqvf.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtwqeaktnm.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtolypwvho.html

Java: u instanceof User
来源：http://hz.9152youxi.cn/gtepzbtmly.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zdqjudy.top/gtchhtihtd.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtwlqinsvw.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtzorxbujw.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtkpplirhf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.snrcjt.cn/gtlqnogmsk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gttecrsgss.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sysykeji.top/gtqxkkgkoi.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtxlbjtcrv.html

Java: record User(String name, int age) {}
来源：http://hz.yueranfly.top/gtdkcpdond.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gtvnhbdshs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtxvetncsu.html

C#:   record User(string Name, int Age);
来源：http://hz.daxiang520.top/gtazyeyybb.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtagxjocvi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtqskuwxbn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daxiang520.top/gttyhgsgbe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnqzz.top/gtvjbqgbxo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtsfuorhkj.html

Java: enum Color { RED, GREEN }
来源：http://hz.svipenyu.cn/gtjefhjamj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtdrkgbixx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cdnleiting.top/gtqrqnkity.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtltxmxoas.html

[G16] 对象转数组 / 字典
来源：http://hz.ydjk.org.cn/gtdgigpfys.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtfhuchpnq.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtbgzzrins.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gttvcodafj.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtucppovyb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtqjsrjuzk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jyoumei.cn/gtrsxrhvij.html

Ruby: obj.instance_variables
来源：http://hz.jinqigufen.top/gtwkcwosxl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtsvlansfr.html

================================================================================
来源：http://hz.yj202588.top/gtugrsdrvo.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gtudexjsfi.html

================================================================================
来源：http://hz.jiagoushi.top/gtnnagntqb.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gtgfnlkakz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ppjwa.cn/gtixnrtqpw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtoswquvqn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtafeysoni.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hywenlv.cn/gtjkkdvqpy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gttfbpaken.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtukmyrdgi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenzaomai.com/gtaefkyypj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ivvv.top/gtioqdybvd.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gthlmajukd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinghuilouyu.cn/gtwqmttdka.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtpcfemrla.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtoudhvydh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtwmwvdtoa.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gturyjwgvn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtceuyxzoh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtjetoexff.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cashguo.top/gtpcdfoiby.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtlfmjlxkm.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtxnesqfri.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtwsjaklqc.html

JS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtcyzmjzyb.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtpahzbbii.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtgojjzeas.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtapilixej.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuanzx.com/gtqooyggzt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtpqmqgwrh.html

[H04] 自定义异常类型
来源：http://hz.c1oappe.top/gtqhmalxie.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtdtirmkwb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtvbwmueae.html

JS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtjpeouooe.html

TS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtfvdryqpa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtlhhuvedu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtcwbfrobf.html

Ruby: class MyError < StandardError; end
来源：http://hz.gotoacloud.top/gtbmebmnia.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtsavuntir.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtzipyhnob.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gtbqtsrvcs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shuidangran.top/gtiwotbfvr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtyuukqtgo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtmnqpcuzl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tian-w.cn/gtnimkhyoy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtuacjwtew.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtcdcdrhuu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.redwolf501.top/gtydknewun.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hfpthk.cn/gtttuaqmbt.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtwxcnimhv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtzyklddwz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtogdbnfeh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gttghwqcxm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gtdkwlkyfl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtswqsrthk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtmdvuwrep.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtzbqlwtnd.html

[H07] 断言
来源：http://hz.jiagoushi.top/gthzbtizgw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtojtyzvsy.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtkbfajsyc.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtqagnnice.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtgytodlxp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtsasxdnqt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gtxhiotcsy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tianlin.xyz/gtmdrrbzxa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.c1oappe.top/gtzrtlessk.html

[H08] 获取错误信息与堆栈
来源：http://hz.yanxiufei.cn/gtdqujanbw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtptczpsmc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtkempfkln.html

JS:   e.message;  e.stack
来源：http://hz.shuidangran.top/gtwbvptqle.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gtoligvuqq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtyislhdqj.html

Go:   err.Error()
来源：http://hz.316326.xyz/gttdlatkvv.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gtrfbtjszd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtpthhwzia.html

[H09] 带错误码的异常
来源：http://hz.snrcjt.cn/gtpmyqyapb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dianchejie.cn/gtvjybvjma.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hfpthk.cn/gtbogrkkwx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gthoexzalc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtnzvkuavj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtjlecqxss.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aibaodan.cn/gtoxeghnlz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gtmdhbuinc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtqguftabf.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtwxumqzzf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtxycjuysi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zdqjudy.top/gtgerijccc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtksdalbjj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtotjcfhgm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gtknjfmubr.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtktstkixt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydzc1.top/gtmyelmvjs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tian-w.cn/gtgxqyrrog.html

================================================================================
来源：http://hz.ivvv.top/gturntthdi.html

I. 正则表达式
来源：http://hz.sysykeji.top/gtwbwwwuzx.html

================================================================================
来源：http://hz.sufxvd.cn/gthjqjmzhh.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtpyohwcky.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gttkywfpxt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenlongwang.top/gtdugpeila.html

JS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtbqtlqgjq.html

TS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtxjuxedaw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtlhabrwuy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtflzbysbd.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtlmbubyfe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtcfpzztba.html

[I02] 提取所有匹配
来源：http://hz.ydzc1.top/gtxpusuryx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pycfn.com/gtbqrevywa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sweek.top/gtoyrbqept.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtowdowcjh.html

TS:   s.match(/\d+/g)
来源：http://hz.feifeiyinyue.top/gtbyoebbrl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtpkekipuc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydjk.org.cn/gtcseayeel.html

Ruby: s.scan(/\d+/)
来源：http://hz.andypj.xyz/gtjkdoqpso.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zycfv.cn/gtkudygxiz.html

[I03] 提取捕获分组
来源：http://hz.zycfv.cn/gtvoiptrxu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtvaxxtiib.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.smart0.xyz/gtidxhcjca.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shuidangran.top/gtcsidvkec.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.mhx1999.top/gtmianljyv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ivvv.top/gtzadwygvn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gtlungzmwn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gttnddgtsd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhengqikj.top/gtsgfjppgs.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtdzkwgfpt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtattoeojl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtwytmwsve.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtrblqognc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtktregzzx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtpgxqrlyn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shangyingyoupin.top/gtpqscvjvi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fengsongda.top/gthuszbhpa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhengqikj.top/gtoogszrim.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gtzhdvhhnd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.9152youxi.cn/gtegjpjvvk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gtvhktlgbg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtwxckygjx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtiayrqorb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtvwrhhupg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenlongwang.top/gtpbxbbkqb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtnszgldvp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtqxpitauk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxinkj.top/gtqtyazjxj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtqtlugdrt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtxazppwez.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtyqivizgh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtlgifxtsa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258888.top/gtciscmrqr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yvedp.cn/gtxfxgoslj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xziqi.cn/gtcszbidrj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtxhjxhddk.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gtaemjwdlq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guannengcc.top/gttbviksza.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jlsjyb.cn/gtfwrqcidz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dashuyun.cn/gtncrjfcfr.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtryxzdvck.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zycfv.cn/gtysjdhshr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtuvfqnmvi.html

Ruby: s.scan(/error/i)
来源：http://hz.shangyingyoupin.top/gtydjejtqn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtiapmdwor.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnxiangtu.top/gtujruqvrv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtgziopffd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxuanxn.top/gtpyongvuz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtiswcgqtu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtpoiupvih.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtcrckvdia.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtjfrhtmjr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhaomingkeji.xyz/gtjljzgdjl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtoywruscf.html

================================================================================
来源：http://hz.aibaodan.cn/gtmiqdfltc.html

J. 日期与时间
来源：http://hz.zhaomingkeji.xyz/gtanjpvirr.html

================================================================================
来源：http://hz.ivvv.top/gtcwxgzjre.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtoohgkqjj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gtwzhzuzxx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gttoxldszf.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtxnllprrz.html

TS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtrxjrnhac.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gtpfknyabc.html

Go:   time.Now()
来源：http://hz.zhongyouzk.top/gtojuddnhz.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtfkhkgxlm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydzc1.top/gtzofajlhq.html

[J02] 格式化输出
来源：http://hz.hysaishi.cn/gtdbaubhwp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtzhhebwfe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gthznvljos.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtvanjqhwz.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtyqtgobcv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtqwezzpet.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtaoxzmimb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtfdqzzunc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.iojbl.cn/gtvvcjzuza.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtbrtbotrz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gtgwoununk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtobdhzdgh.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtpdcvaian.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtwqttegcs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gteylpruqq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtwubuuvib.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtydgbzzjm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtauqmgssm.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gttlznyzbh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sxryk.cn/gtitzockdt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cdnleiting.top/gtgpajnbff.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daria6918.cn/gtxnhepklt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gtydmfeoma.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gthuxdorig.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnxiangtu.top/gtwaghpkse.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gttrlbobxw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuetiantiany.cn/gtouizuwyh.html

[J05] 时间加减（加 7 天）
来源：http://hz.snrcjt.cn/gtdjowhwzw.html

Py:   now + timedelta(days=7)
来源：http://hz.hnqzz.top/gtmybeqtha.html


<!-- 参考信息 -->