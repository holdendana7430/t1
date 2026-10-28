代发 wailian999

PHP:  public static function f() {}
来源：http://hz.yvedp.cn/gtucylhaog.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gtfptuiupa.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtivnrnsew.html

Java: static void f() {}
来源：http://hz.sufxvd.cn/gtreqprvto.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtbydmtejp.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtoprvikre.html

C#:   public static void F() {}
来源：http://hz.sxryk.cn/gtlmuyzgzp.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtrwslckto.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtqctuowyb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gturckhvxf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tianlin.xyz/gtpnyrzmsz.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtkabilvgs.html

Java: interface Shape { double area(); }
来源：http://hz.yj202588.top/gtqdfmiezj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtabzyeefy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtclanwgif.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gtolvqvxve.html

[G10] 访问控制
来源：http://hz.svipenyu.cn/gtvyaqitpa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gtzkedxegr.html

PHP:  public / protected / private
来源：http://hz.xuanzx.com/gthetgddrn.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtcvrgqamm.html

TS:   public / protected / private
来源：http://hz.iojbl.cn/gtbaurywmy.html

Java: public / protected / private / 默认包级
来源：http://hz.tian-w.cn/gtwnaohyqd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtcxolcten.html

Ruby: public / protected / private
来源：http://hz.chenjidiqi.icu/gtaljhlvfk.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtrbcqgrwi.html

[G11] getter / setter
来源：http://hz.chenlongwang.top/gtnsfmgrmm.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtaaxqocqk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gthfdkcemd.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtpnypbneh.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtglonaujw.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gtckyhtufk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gttbcswucw.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtmdughxzm.html

C#:   public string Name { get; set; }
来源：http://hz.ppjwa.cn/gtoksmlrsg.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtbvizmlxj.html

Py:   def __str__(self): return self.name
来源：http://hz.bjfxy.top/gtlonyvsso.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtozsktpjz.html

JS:   toString() { return this.name; }
来源：http://hz.sweek.top/gtcbweoskx.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuanzx.com/gtesftnazs.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhengqikj.top/gtpfzoaang.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnqzz.top/gttnbillac.html

Ruby: def to_s; @name; end
来源：http://hz.smart0.xyz/gtaijvbwhf.html

C#:   public override string ToString() => Name;
来源：http://hz.daxiang520.top/gtjfuusfso.html

[G13] 判断对象类型
来源：http://hz.nwbrower.top/gtggjshvtd.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtyctvehdp.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtsqlprthn.html

JS:   u instanceof User
来源：http://hz.jianghu66.top/gttflaxrwe.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gthhsmaokt.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gtwubqrexh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ywan-chungtsiang.top/gtkoklnyvc.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gtzfzateie.html

C#:   u is User
来源：http://hz.fzhhl.top/gtmkxbbymr.html

[G14] 数据类 / record
来源：http://hz.sxryk.cn/gtqewekfle.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtyrogcxlq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtsotzsper.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuanzx.com/gtdfmyikfq.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtsxzkznhb.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtaumaqthi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zdqjudy.top/gtoripayvp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenzaomai.com/gtamvahzjy.html

C#:   record User(string Name, int Age);
来源：http://hz.daria6918.cn/gteoxoybjq.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtcfclteih.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtzdnnesxp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtesyhuski.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ppjwa.cn/gtjxvuivjb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtxclnpjdc.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtpwgibyom.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shzxlz.cn/gthptriblb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtqcvffcpx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtkqllmjpj.html

[G16] 对象转数组 / 字典
来源：http://hz.9152youxi.cn/gtamljwcyr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtshkvnttb.html

PHP:  get_object_vars($obj);
来源：http://hz.havefunace.top/gtimtdotyo.html

JS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gthkowojhj.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtrqanywep.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xinyue.icu/gtbpkqdzjx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ybcxt.top/gtkbbjucoi.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtnzzjkwiv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxuanxn.top/gtddxxiahu.html

================================================================================
来源：http://hz.316326.xyz/gtyaudgrvw.html

H. 异常与错误处理
来源：http://hz.quarkkingdee.top/gtnaieslky.html

================================================================================
来源：http://hz.bjfxy.top/gtbjpumqiz.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtnszjgdds.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtidlkoplr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gtizrearls.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtpbdosrbc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.guowangkeji.top/gtxflasdkv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gtfamhpmqs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xinyue.icu/gtfkycfgvh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.c1oappe.top/gttwlakxiw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtnsnvbjdh.html

[H02] finally / ensure 收尾
来源：http://hz.zhixingplan.top/gtogejllge.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtqaipvmdt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtkqtwjcmx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtpnfobycp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtmbjyuxpy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gteqnqicbf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtgtsmjjhz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtukfrtezk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gttcxupuhh.html

[H03] 主动抛出异常
来源：http://hz.zdqjudy.top/gtcievceeu.html

Py:   raise ValueError("错误信息")
来源：http://hz.andypj.xyz/gtucgwpquu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtjzlqwjye.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtfqpelyfh.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtqkizlaeu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtzgfpxsbx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtjllxzrcp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxinkj.top/gtcvnpgwxn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gthkffijok.html

[H04] 自定义异常类型
来源：http://hz.daria6918.cn/gtwmvbeddq.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtzrotqlyn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gtteuxblzw.html

JS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtxtuyimzp.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtntlsucyz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtwufkwtbl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtlfpjpevs.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtaxnoalsw.html

C#:   class MyException : Exception {}
来源：http://hz.wangshuangyany.cn/gtncpgfxla.html

[H05] 捕获特定类型
来源：http://hz.ydzc1.top/gtyeskfwlz.html

Py:   except ValueError as e:
来源：http://hz.pycfn.com/gtirzvdysq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gtvaooanip.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtogcfmdtm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtevmceygd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnqzz.top/gtzzkrnuco.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gtlsfpfmij.html

Ruby: rescue ArgumentError => e
来源：http://hz.cheryme.top/gthmowqsgy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ppjwa.cn/gtadwzlbhe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tian-w.cn/gtyhdexcsa.html

Py:   value = d.get("k") or default
来源：http://hz.ydjk.org.cn/gtvhrzccda.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtkqaryksi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gthqxbpuyv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gturmhyluf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtzetvbrdb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinyuanbaomall.cn/gthezsbdqh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zycfv.cn/gtydahnvmp.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtwrrqdtap.html

[H07] 断言
来源：http://hz.yongpay.top/gtryuteslg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtkwsebgge.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtavxlofgp.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtpkbpwgqn.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gteugenqwn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gtfncyylku.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtrkxyqgnf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtcqbhoxvn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yangfankeji.com/gtbzxzyykb.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtdsjbrqgd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtmspdzzzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtjvmmzirp.html

JS:   e.message;  e.stack
来源：http://hz.jinyuanbaomall.cn/gtiamxkbtc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtlbqtiutl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtiiyiukjp.html

Go:   err.Error()
来源：http://hz.gotoacloud.top/gtehcfjvla.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtqhbxgssx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtfsovlgxy.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtoxsgdqhh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gtcbdccnxz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gturxbwgmo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.andypj.xyz/gtdhffjghq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cheryme.top/gtkftqozqg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shangyingyoupin.top/gtctqetjrm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydzc1.top/gtndujqxpz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtdldzfxdt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gogol.net.cn/gtyjellohr.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtrheepyyj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtbxwdamuk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhiwuduotai.top/gtxvezbqpq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtfiuagddb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtpoumegob.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtcctpsevl.html

Go:   defer f.Close()
来源：http://hz.meibo888.top/gtlidslfue.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuanzhike.top/gtzbdptekg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cucudq.cn/gtiytwedqc.html

================================================================================
来源：http://hz.xziqi.cn/gtrzplhlrv.html

I. 正则表达式
来源：http://hz.hfpthk.cn/gtsyiekpzr.html

================================================================================
来源：http://hz.fzhhl.top/gtemeiwuwp.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtdgqhwqui.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zdqjudy.top/gtxdullsga.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtzomghqvn.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtzwnjngvt.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtmetkineb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtgdpcswzp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gteiyygohi.html

Ruby: s.match?(/\d+/)
来源：http://hz.hysaishi.cn/gtylwvfpdx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtrjadiwyz.html

[I02] 提取所有匹配
来源：http://hz.ehwqpu.com/gtptozhxkc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtegcihzzd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtltirgmab.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuxming.cn/gtgjyhuqzo.html

TS:   s.match(/\d+/g)
来源：http://hz.yanxiufei.cn/gtmxucslfm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtwyaliegs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtivqalmnz.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gthdlsduoj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtablflcqr.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtelgpdsno.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtbwloxsaw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shzxlz.cn/gtbdprgpmi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtkylhvbab.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gtkxsmoedj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhoulong.xyz/gtyplqvymn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shzxlz.cn/gtvbwxfedj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtgvxadobu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gzhubu.top/gtuptakvqj.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtvkvbvvsu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gthepbgtmw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtahzvrzan.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtmxfeabtv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gttjcibove.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtsqgcypug.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gttxhtfbgl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtvkprzeiv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtufutfdgn.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtodhkricn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtlvkfavqi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.52xcode.cn/gtodsmagro.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtxqfmxhce.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtwlrnkuew.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sysykeji.top/gtbkekuezk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtirtggfhf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gttiokdxqo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtmyiavasy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gaohongyu789.top/gtnlyezgvr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtsqxigodh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtpdqozqic.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gteipifdpc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtpfujrtev.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shzxlz.cn/gtshesxdxo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtccqxumqx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenzaomai.com/gtdnavldax.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtrieuiyaf.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtsfrezznb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinyuanbaomall.cn/gttzchyfhl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gttvlbhkxk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtghthaubi.html

TS:   /error/gim
来源：http://hz.yueranfly.top/gtuufonywm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydjk.org.cn/gtjkpndoxd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gtbntdxlmq.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gtjjgohjvz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangkeji.top/gtbvtuckey.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtcyotyrlb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtbqpxoxzg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtelbkwhbh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtbbuqtqwr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtwwnynfhy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtccomlgxh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtmozekulh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhaomingkeji.xyz/gtesclkmze.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtgadhtdgi.html

================================================================================
来源：http://hz.tian-w.cn/gtyzydrxgi.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtrbkflcxm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtauxjirvg.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtyvkmjnnx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gtudjjlgaz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtuppzewls.html

JS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtqftpsvvp.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtgmfsmarv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtxuhgbqrp.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gttnyjnxra.html

Ruby: Time.now
来源：http://hz.hywenlv.cn/gtacvakyew.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtiycmmync.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gtaefxvipj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtgijlmxeo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gteefxwlcg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtebvibhuv.html

TS:   d.toISOString()
来源：http://hz.redwolf501.top/gtzplaxgkd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sweek.top/gttabbzlqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtqqbgigpp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtqcndeila.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gtjucauclt.html

[J03] 字符串解析为日期
来源：http://hz.cheryme.top/gtnopftosg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hammf.cn/gtawtpcqaj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gttxhjgyub.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtxqswzgfh.html

TS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gthhyuwndb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtckdrlucb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gogol.net.cn/gtwuitzgso.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtluojhlow.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gthggftqzm.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gthrmbdmvg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cucudq.cn/gtycuvkate.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.feifeiyinyue.top/gtvyqzdrao.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtnxaahzvn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtrqaephpo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jianghu66.top/gtazksokqk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtroffmyfk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gaohongyu789.top/gtjybucpvs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jlsjyb.cn/gtimoxtfcn.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtqhtsnyzz.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtzaccfovh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtrymdzhki.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtnrdfarjc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtlbpidtoq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.mhx1999.top/gtuusnxpwb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtzynrzyoc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.9152youxi.cn/gtskaonill.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinyuanbaomall.cn/gtzrromhiw.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gtkndqggdn.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtwguholaa.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtonwlxhsf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gtybjsllbo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guowangkeji.top/gtfodxxniv.html


<!-- 参考信息 -->