代发 wailian999

Ruby: super
来源：http://hz.cashguo.top/gtdqlejjjv.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtsftsffbu.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtpzbmicwz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtsudkchfv.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtwdvbxypt.html

JS:   static f() {}
来源：http://hz.316326.xyz/gtyoidnqcj.html

TS:   static f(): void {}
来源：http://hz.yangfankeji.com/gtdnqqemgv.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gttrlvfkvj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.316326.xyz/gtfwmdqcho.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gteyptgfag.html

C#:   public static void F() {}
来源：http://hz.shangyingyoupin.top/gtacsdekvd.html

[G09] 接口 / 抽象类
来源：http://hz.yuxming.cn/gtoaisnmwh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shzxlz.cn/gtadnqktnk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cqqwz.cn/gtkiocbnbp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtzomhxrkz.html

TS:   interface Shape { area(): number; }
来源：http://hz.ehwqpu.com/gtezmzurss.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtahqsmrkp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtbjqgmjmn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxuanxn.top/gtomogybid.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gtejhgulqh.html

[G10] 访问控制
来源：http://hz.hnxiangtu.top/gtzgeulwfe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gttgctykev.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gtpnjmesjn.html

JS:   #private 字段；其余公开
来源：http://hz.chenzaomai.com/gtmazfciau.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gtzbgmcstq.html

Java: public / protected / private / 默认包级
来源：http://hz.52xcode.cn/gtjfebaxmv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtmnpjavhx.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtdezqwdhd.html

C#:   public / protected / private / internal
来源：http://hz.hammf.cn/gtavrhqmlk.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtfudvmjdv.html

Py:   @property 与 @x.setter
来源：http://hz.cdnleiting.top/gtdltfishc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtiglkarlg.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gtxqpiftnq.html

TS:   get name(): string { return this._name; }
来源：http://hz.quarkkingdee.top/gtcyhzadyx.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtoazwxtrn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.mhx1999.top/gtkoayxjbq.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtuelpdoqo.html

C#:   public string Name { get; set; }
来源：http://hz.9152youxi.cn/gtouohzjxz.html

[G12] 对象转字符串
来源：http://hz.jiagoushi.top/gtnmeqrtao.html

Py:   def __str__(self): return self.name
来源：http://hz.yongpay.top/gtlbtviajh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtbdirvcnp.html

JS:   toString() { return this.name; }
来源：http://hz.nwbrower.top/gtjpktywuo.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtomghzgbq.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtaxwjyrpe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cdnleiting.top/gtgzqjcjwu.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gttyvagwle.html

C#:   public override string ToString() => Name;
来源：http://hz.fengsongda.top/gtlhiivjfr.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gtrzgdkiim.html

Py:   isinstance(u, User)
来源：http://hz.hammf.cn/gtfdwxsdut.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtbxjtrxcs.html

JS:   u instanceof User
来源：http://hz.yonumen.top/gthwzyysgy.html

TS:   u instanceof User
来源：http://hz.jinqigufen.top/gtouerdgcp.html

Java: u instanceof User
来源：http://hz.cashguo.top/gtnkgisklr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtvcoyqcnx.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtmsinbhtc.html

C#:   u is User
来源：http://hz.meibo888.top/gtfqlkadid.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtwigxopnk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.birdmap.top/gtylreqkau.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtbbflmeeq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zycfv.cn/gtxoelypma.html

TS:   type User = { name: string; age: number };
来源：http://hz.aibaodan.cn/gtegoxkagc.html

Java: record User(String name, int age) {}
来源：http://hz.sweek.top/gtlsaehmvy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tianlin.xyz/gtehexfipn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtrdisjhdx.html

C#:   record User(string Name, int Age);
来源：http://hz.meibo888.top/gtokhwptvn.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtxlnethah.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtpysckxhg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sweek.top/gtdrsntlya.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtloyxhrxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtyuigockn.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gteknootwi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtpusnzmha.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ppjwa.cn/gtpjhjrmxz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtoyckzmdx.html

[G16] 对象转数组 / 字典
来源：http://hz.quarkkingdee.top/gtvgkkqlrd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258888.top/gtcuzduodv.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gtccregzka.html

JS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtbztngliy.html

TS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtmsoyvelm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuanzhike.top/gtjpfjtndg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtqzjvipqt.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtsfuqjkrc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtjgilbscx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjujyzqcp.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtcxzjmjim.html

================================================================================
来源：http://hz.yueranfly.top/gtbhijmayp.html

[H01] try / catch 基础
来源：http://hz.hnqzz.top/gtbwyhqavz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.redwolf501.top/gtdzbahjfy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cqqwz.cn/gtlserpoio.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtvahokfxx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gtemafctfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnxiangtu.top/gtgeddxlsu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtllogebzh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gthhbqhoaw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gthmqrgkio.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtgbjecqah.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gzhubu.top/gtuvlsaivw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gthpmdacaw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtndbhkyll.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtoozmlmvo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtktgbgvkh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtfkmpokod.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtdiltqkpr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtwnynxqra.html

[H03] 主动抛出异常
来源：http://hz.gzhubu.top/gtcaihqowg.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gtxcwldbml.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtmkhuuyxb.html

JS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtnpsxqnwd.html

TS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtztbzxkcc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtltsxvduv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gtrogsymxk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtyqvsafdo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gtvogjqnyj.html

[H04] 自定义异常类型
来源：http://hz.sufxvd.cn/gtccgjazmm.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtlrhzfkjf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gthkngfvkt.html

JS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtvqnpwyaw.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtorwkpyvd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtvqvglhop.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.mhx1999.top/gtcsvmqxff.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtldqffaex.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtqcorhogb.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gttrsqlvad.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtzppytufx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zdqjudy.top/gtfntlrfah.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtjvmrcucs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtvmoxdbua.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gtipmgaffe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtbefhxmka.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtglwlabkg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtnwbpylpk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtbayevllh.html

Py:   value = d.get("k") or default
来源：http://hz.zhaomingkeji.xyz/gtqvhetsch.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnqzz.top/gtuykwnbfm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtzubbrfrh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtzqmqtegx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtmjjfjnpu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gtmlgcmdbk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtthrneync.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtkxnitwrw.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtlfbrmist.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtidjlxiok.html

PHP:  assert($x > 0);
来源：http://hz.zhoulong.xyz/gtdeyjzbrr.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtolbnnppl.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtcnxwjhpr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtmmzznhvj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guannengcc.top/gtzkozhhhu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sysykeji.top/gtnenrgtof.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtnyupojvs.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnxiangtu.top/gtlnysgmxs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shangyingyoupin.top/gtotxuanpg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hongshengwenyu.top/gthkwkcuqq.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gtsvcaziqi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yanxiufei.cn/gtqqpdlcfd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtzcxtzham.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtxxageiwi.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtkqciicqo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtyvvtqjvn.html

[H09] 带错误码的异常
来源：http://hz.cqqwz.cn/gtokclnobb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinyuanbaomall.cn/gtvikvcwzf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gtxlxsjgbe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj202588.top/gtzzynwqtg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daxiang520.top/gterbftbil.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.vqdsnc.cn/gtxhltbbzo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenjidiqi.icu/gtkmqfnaml.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gtgqgnkzld.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtungbohxk.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtlfvuywsg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtuvjifbyo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtqcjthabm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtcsijviou.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gthdswdqnc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gttviwyuby.html

Go:   defer f.Close()
来源：http://hz.yonumen.top/gtmduqivkk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtyhvqhmjg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.birdmap.top/gtivnamwpq.html

================================================================================
来源：http://hz.zdqjudy.top/gtrqdlguwo.html

I. 正则表达式
来源：http://hz.jinqigufen.top/gtdccxotcp.html

================================================================================
来源：http://hz.mhx1999.top/gtwmqjsnbz.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtyzidrzty.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gtczbkaoax.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dashuyun.cn/gtmnsugwma.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtfafgtzec.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtofdqogyu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sysykeji.top/gtrqrttkgx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gtuhddxdxq.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtxgjlvbde.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.316326.xyz/gthcauejhy.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtdimejcff.html

Py:   re.findall(r"\d+", s)
来源：http://hz.snrcjt.cn/gtelbcommr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cheryme.top/gtrgbfaswp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.smart0.xyz/gtrjhjmhwz.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gthoxrhsty.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hysaishi.cn/gtwgdrdqth.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.meibo888.top/gtknnoxxje.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtdfaffvtf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yvedp.cn/gtudfffxek.html

[I03] 提取捕获分组
来源：http://hz.xziqi.cn/gtstopxavk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtgmqoyifq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tanke756.top/gtvebbskle.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinghuilouyu.cn/gtbqtjptbu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuetiantiany.cn/gtviafvmuv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtvekrdvho.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jianghu66.top/gtubflbbcp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gaohongyu789.top/gtsotwcouo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtrfpymclm.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtzpwmnrqq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hysaishi.cn/gtyeiwxuat.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtkkczgcab.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtywflyyhu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtadvbqmjq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtugrnthgz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtroqlztiu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtsaspvohi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigufen.top/gtqgcsysar.html

[I05] 按正则拆分
来源：http://hz.daxiang520.top/gtefffufzs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtxbfnybxs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gtxdtdjwsu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gthftafoxt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtnltmboxi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtypthygui.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtkkfmuonb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtvvfumxfm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shuidangran.top/gtcznndgad.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtaxmbguhb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtxscgetno.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.smart0.xyz/gttruhtbia.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gthjrwleln.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtapdbgftw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hysaishi.cn/gtasusnsha.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.redwolf501.top/gtyqoddzyp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gtqbvsawiq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtmkescvlx.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhengqikj.top/gtsxsoauvv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtpjkwrpog.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gthrygkwez.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtasqifegi.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtltyxzdpp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gttdnswzuw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtzjddstvx.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gthbliwnhp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.svipenyu.cn/gthuvivruq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tanke756.top/gtmdpamvuc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinghuilouyu.cn/gtclpvbdur.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtckbgmkng.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtzerzeads.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtsgzjgaoj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtuxtieqpg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtztwpiavu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtiwuqkkyk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gttihvqpxc.html

================================================================================
来源：http://hz.sufxvd.cn/gtbtldeaqq.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtluasuehc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrfeqcewb.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtlsasfwoo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtjirnuyjg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtzmuwikfq.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtougvmukl.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtzzydtddg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtrcntuozu.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtolzdgjfq.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gtteokwaqu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtasqnxeau.html

[J02] 格式化输出
来源：http://hz.yj20258888.top/gtphmnrhoi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtxwpnaxjo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gttfajlzrg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtkoyslnnu.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtepojyosj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtdthzyhhu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtibmtutsq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtziwpbdgc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuanzhike.top/gtpzyqcnvl.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtsstaylnv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuetiantiany.cn/gtivyyevod.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dashuyun.cn/gtatbyghjh.html

JS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtxwpjprzo.html

TS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtkiegahfv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtehoorfte.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jyoumei.cn/gtlonibkrh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtulvztvhi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtibamgnzg.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gtakumfxjx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtahaprbhh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtbfqedibc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.52xcode.cn/gthmvwwfzt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtsdsbhxkg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gtglupakkw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtfezbpoht.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pengpengdd.cyou/gtejdwzkuw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtfwsgybii.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtzjeuhmzt.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtzyvbvlzw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinyuanbaomall.cn/gtcthxgrwn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtodybafyf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtnitelpsu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtcjekqqzv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gtwxrrjbmv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtbbtjupsk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtewscctbz.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtjzbxegdt.html


<!-- 参考信息 -->