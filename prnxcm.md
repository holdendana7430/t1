代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.havefunace.top/gtxsypubov.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtpnwrruev.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtwmzsyvhp.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtjnwksszt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fengsongda.top/gtemunovjt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.kuanghao11.cn/gtgdictjpi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cheryme.top/gtzfkszdtx.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtkiirnjqv.html

Java: interface Shape { double area(); }
来源：http://hz.zhijiandao.cn/gtgpnplfgx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtgqyouner.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtrwvuclwh.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtsvzlhklk.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtpnaqghkf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gtnzqosqis.html

PHP:  public / protected / private
来源：http://hz.zhiwuduotai.top/gtdpjtzrlm.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtlzxszawr.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtvrkxuiiw.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtrrfipran.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fengsongda.top/gtunkfyxro.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gttpibsdam.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtfaxngbde.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gtxnprpkrv.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtvpqewaud.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtxiucjwmn.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtkvwmvwgt.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gtakfxnmau.html

Java: public String getName() { return name; }
来源：http://hz.zhiwuduotai.top/gtlwsbxdoy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtynrlysbj.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtltejvysy.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtmrwxyvev.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtnomaalnm.html

Py:   def __str__(self): return self.name
来源：http://hz.aizwys.cn/gtibgmtoev.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtlrvgtfah.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtwbqzmaet.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtbzcqyugu.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtaorceuvd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtoapgnqlt.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gttlswegkn.html

C#:   public override string ToString() => Name;
来源：http://hz.xuetiantiany.cn/gthsxjukza.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtkediimey.html

Py:   isinstance(u, User)
来源：http://hz.pengpengdd.cyou/gttpxleyco.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gtwgcmmsvl.html

JS:   u instanceof User
来源：http://hz.daxiang520.top/gtapjfhylw.html

TS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtsnndlshm.html

Java: u instanceof User
来源：http://hz.daria6918.cn/gtruekytde.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtiheuxomq.html

Ruby: u.is_a?(User)
来源：http://hz.yangfankeji.com/gtmvwyznnz.html

C#:   u is User
来源：http://hz.jianghu66.top/gtplvnybhx.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtsryrgbbi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gtbjirlvnj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.havefunace.top/gteyggydys.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtrwecfzgf.html

TS:   type User = { name: string; age: number };
来源：http://hz.cheryme.top/gthcmzlbce.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtrysprilk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj202588.top/gtfmlbjoqk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cdnleiting.top/gttbdawzqy.html

C#:   record User(string Name, int Age);
来源：http://hz.jinghuilouyu.cn/gtjrkbnasl.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtjuhncpcy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.0kj1m.cn/gtzybonctv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuanzx.com/gtlyiasubx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ybcxt.top/gtkdvlnmvm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtyyizcobh.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtigmqvpej.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtfomexuyh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.9152youxi.cn/gttnadabyf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtmcgtioqr.html

[G16] 对象转数组 / 字典
来源：http://hz.bjfxy.top/gtctfchtjp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gtjymirvsh.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtvdyfqbkx.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gteuqgzdmv.html

TS:   Object.entries(obj)
来源：http://hz.sweek.top/gtxlqofgnn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtyjvuodjd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtncylamfk.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gtfppvwcob.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtjltqhojp.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcinisixm.html

H. 异常与错误处理
来源：http://hz.yj20258.top/gtwxkkbpey.html

================================================================================
来源：http://hz.mhx1999.top/gttbdkktkp.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtmodywysk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtoyfgrdzn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.0kj1m.cn/gtzomscdmy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtxxplhsuy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtaamhuzyl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenjidiqi.icu/gtdjlkboha.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.havefunace.top/gtjhcmpkds.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydjk.org.cn/gteonecndb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gtcxmlsnqa.html

[H02] finally / ensure 收尾
来源：http://hz.zycfv.cn/gthxvfrnrv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtgtdjdkze.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtawcrciqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtivsafyal.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gthwpetmge.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtjtdymlhl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtkcjsmjyd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shangyingyoupin.top/gtztncpasb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shangyingyoupin.top/gtorttioog.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtkmpalusk.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtjahcjacw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtyauevkhg.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtlsoprmpw.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtnrhrqlhp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtnvcxebcd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtkveitolp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtyfghlolp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtnaynqvko.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gtkenjvyjn.html

Py:   class MyError(Exception): pass
来源：http://hz.daxiang520.top/gteqtbmfjm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtdovrpyka.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtxrzdlozj.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtqlmhthex.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gtyhsrzvac.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tian-w.cn/gtmwghkgha.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtffqgcafh.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangkeji.top/gtwuldlsuf.html

[H05] 捕获特定类型
来源：http://hz.xuanzx.com/gtjauyavvg.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtgxyexmcb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gthgfcgtif.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gterotqhkt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtltxigjod.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtmkotdjef.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtzcfrtejw.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangshuangyany.cn/gtazbotggg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gtfnphbpzm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gtmzhwprko.html

Py:   value = d.get("k") or default
来源：http://hz.pengpengdd.cyou/gtzmuobrvt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.kuanghao11.cn/gtwqqyjgzg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtfgkbibkt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gthnftdbov.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gtlgwiudng.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.quarkkingdee.top/gtfkcrnqve.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtztokzfne.html

C#:   obj?.A?.B ?? default
来源：http://hz.guowangkeji.top/gtxpvantff.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtaonlhioa.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtfcaivgam.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtpuoxetow.html

JS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtbfpojazv.html

TS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtcespgyku.html

Java: assert x > 0 : "必须为正";
来源：http://hz.quarkkingdee.top/gtlrvklkmn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangshuangyany.cn/gtqrdxvfdt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtwkcvhlnb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gtlrwzznrn.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhixingplan.top/gtxnborjfl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ppjwa.cn/gtfnaboagg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gtirrkrais.html

JS:   e.message;  e.stack
来源：http://hz.zhijiandao.cn/gtayxmpnac.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shzxlz.cn/gtxrqkmzra.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtrgfvoleb.html

Go:   err.Error()
来源：http://hz.chenjidiqi.icu/gtptovufym.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj202588.top/gtjowapulb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtwqihgjvr.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtuwfjagwy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuxming.cn/gtpndhyjbo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xinyue.icu/gthwjpqsif.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.feifeiyinyue.top/gtefattabt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yongpay.top/gtisfoqgsh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gtfygvhofp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.feifeiyinyue.top/gtlfhhxxbc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhiwuduotai.top/gtmgaynftg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zycfv.cn/gtlqkxakfp.html

[H10] 资源自动释放
来源：http://hz.nanxinkj.top/gtfrxeiusm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtyxjinoga.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhongyouzk.top/gtdfdzisak.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtysurvwok.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtkfywgtdn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gotoacloud.top/gtxxcssvpk.html

Go:   defer f.Close()
来源：http://hz.wangshuangyany.cn/gtprlhrbtw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gtedakpsqh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.0kj1m.cn/gtanzabvvu.html

================================================================================
来源：http://hz.shzxlz.cn/gtutygcewr.html

I. 正则表达式
来源：http://hz.zhongyouzk.top/gtkctratqa.html

================================================================================
来源：http://hz.dianchejie.cn/gtsjuavmzw.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtkqmbkpzr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258.top/gthukwuenx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnxiangtu.top/gtvegnfyyz.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtiwsbmeab.html

TS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtffvyojro.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgfzy.top/gtpoglyykd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtidrrgzkz.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtjncdsfdj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtbqkjizja.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gthyqxjddq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.wangdashe.top/gtqfqpnluf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtpqgfbpar.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtqzwjwaas.html

TS:   s.match(/\d+/g)
来源：http://hz.xuanzx.com/gtqonqkifv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtgfsgbwgj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtwpaseyds.html

Ruby: s.scan(/\d+/)
来源：http://hz.yongpay.top/gttrfjifke.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tanke756.top/gtpteijqjl.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtneqcyqhr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shzxlz.cn/gtthqowivs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gtgntocmma.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cdnleiting.top/gtpkbyeflc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhijiandao.cn/gtridrvake.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtjdmbikmh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnqzz.top/gtxkernklm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jyoumei.cn/gtbsaewsng.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtvwayegnf.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtokhcwucx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xinyue.icu/gtwybzxqhm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gthqyancqz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gttxwylmnt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtrjshzqrz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gtyjfhdgyb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xinyue.icu/gtubwnrmjm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtuiwhtznn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xziqi.cn/gtkqusctjj.html

[I05] 按正则拆分
来源：http://hz.tianlin.xyz/gtpjeyymbn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtcecqkgkh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ppjwa.cn/gtanpiasrn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtvamsqgxx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtzjzeiurw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtayvbopaj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtawdoxjju.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtjsphcqrb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gtwihvpjhr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtlpfgluyy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtoqwbedpv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtdjpuxqeg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtmlpppfhr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtqbakyvaz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yueranfly.top/gtxbflpszh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hongshengwenyu.top/gtwwsxmamu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258888.top/gtyodkxwgq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtxdsppeze.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtaxubmsyb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xylfe.cn/gtnhvkqwzw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtudpgisns.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtfzmuaasq.html

TS:   /error/gim
来源：http://hz.zdqjudy.top/gtvbqsatvc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtbfmtafhu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtdzjpeumg.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gttazaaqbo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gtxczaqyzj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtqmapblmq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtivznqvaf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yanxiufei.cn/gtidrkzmdq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtkifhvqwg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtjyxlzzsg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtfkzatfvg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnxiangtu.top/gthcycegre.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.c1oappe.top/gtnedztvby.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sysykeji.top/gtknfbydez.html

================================================================================
来源：http://hz.mhx1999.top/gtpxwfufae.html

J. 日期与时间
来源：http://hz.yongpay.top/gtqieczsdd.html

================================================================================
来源：http://hz.guannengcc.top/gtpjiwufsc.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangkeji.top/gtcqwkpncs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtmuivzyus.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtpwnzqirj.html

JS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gttnvsegpy.html

TS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtkobtqyyu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtxgxibuyr.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtgqezmlsb.html

Ruby: Time.now
来源：http://hz.guowangkeji.top/gtwcmwarfk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtcqaincqj.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtpwoovpjj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtubdkzdwa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtuilyaqhp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtzjeeogmu.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtxiysxrkl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtouelhrsv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gtkspnuyqg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtxrknthyu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gthoxxzble.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtcxgzmkxm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gtjmmeojdi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ppjwa.cn/gttikrshzf.html

JS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtjifablhx.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtwsovxivm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtenebeydh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sweek.top/gtbcrpplcv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gthfjzdjik.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aizwys.cn/gtrmvtugvl.html

[J04] 时间戳与日期互转
来源：http://hz.dianchejie.cn/gtxyfrhswb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtmqzlkspw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtxlnraclj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtwsovznxy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtdqxwfzzo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtxjyiauno.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gtfinundbn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtouhpbvxv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gzhubu.top/gtrvwzmyga.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtiqeqxrgr.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gtgpklktwp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtuglotfld.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtxpztzflg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtnqzmdxxk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gtxcalorhn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtthcwdlge.html

Ruby: Time.now + 7 * 86400
来源：http://hz.smart0.xyz/gtwxoqakgu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangkeji.top/gtzqadzriy.html

[J06] 计算两时间之差
来源：http://hz.ehwqpu.com/gtdckrxqpt.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gtixjawdon.html

PHP:  $end->diff($start)->days;
来源：http://hz.guowangkeji.top/gtxomomkdq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtbchgngsk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhongyouzk.top/gtkcqgcevj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtgmsharor.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtiooryqkh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtmvtangxe.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtcbewlmat.html


<!-- 参考信息 -->