代发 wailian999

[G10] 访问控制
来源：http://hz.shanyushiyangtech.top/gtvhaaezmn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtjerwgupv.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtncybezhp.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtrrwbpsbb.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtyoogifnu.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtbopftiuy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tianlin.xyz/gtludujnde.html

Ruby: public / protected / private
来源：http://hz.gogol.net.cn/gtogodbprc.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtqjiukwds.html

[G11] getter / setter
来源：http://hz.ehwqpu.com/gtrrdrtsij.html

Py:   @property 与 @x.setter
来源：http://hz.xingfuxueyuan.xyz/gtklbeziep.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtjcxcwbza.html

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gtjtrgehzj.html

TS:   get name(): string { return this._name; }
来源：http://hz.tian-w.cn/gtcllpnwsb.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtviztlhvh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtjuthaeea.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtprxkwwwc.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtftwmarvc.html

[G12] 对象转字符串
来源：http://hz.wangshuangyany.cn/gtcxysluze.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtpmeokafb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtzteozeao.html

JS:   toString() { return this.name; }
来源：http://hz.ydzc1.top/gtuyfmczhb.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtnixdrzhn.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtrrnflopp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtyvnyxmqi.html

Ruby: def to_s; @name; end
来源：http://hz.fengsongda.top/gtifzlkpbt.html

C#:   public override string ToString() => Name;
来源：http://hz.pengpengdd.cyou/gtnqbgllnn.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gtkovuflxm.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gthjtjawvh.html

PHP:  $u instanceof User
来源：http://hz.cheryme.top/gtycwhjxsa.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtgewpydmo.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtiocopnzz.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtncbndxmu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtqytrjpir.html

Ruby: u.is_a?(User)
来源：http://hz.hammf.cn/gtursptwln.html

C#:   u is User
来源：http://hz.pycfn.com/gtyugseoax.html

[G14] 数据类 / record
来源：http://hz.sxryk.cn/gtlgkfsqpw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtgkobkubj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtbhmjqxkh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zycfv.cn/gtybldacgy.html

TS:   type User = { name: string; age: number };
来源：http://hz.xinyue.icu/gtvrchbvgj.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtqmtzrpkj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aibaodan.cn/gtvnexeomw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtjkjruffe.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtezdpqsnv.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtpnagquca.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ywan-chungtsiang.top/gtmisyntzk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtshpushin.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gteaqiggcm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtccbrncwx.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgfzy.top/gtzpfryqpk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtqauwmpsu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yvedp.cn/gttbdgucxc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtbayhdenc.html

[G16] 对象转数组 / 字典
来源：http://hz.9152youxi.cn/gtosxmedtp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fengsongda.top/gtygcknguz.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gttrnccujv.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtiueeolxy.html

TS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtuzmadikx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ywan-chungtsiang.top/gtqkgtlbek.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtzzljsifi.html

Ruby: obj.instance_variables
来源：http://hz.vqdsnc.cn/gtrtgmdpbi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daria6918.cn/gtawcsalzq.html

================================================================================
来源：http://hz.dianchejie.cn/gtyngsqwhf.html

H. 异常与错误处理
来源：http://hz.tian-w.cn/gtmsmxotko.html

================================================================================
来源：http://hz.zhoulong.xyz/gtlmnntosy.html

[H01] try / catch 基础
来源：http://hz.sweek.top/gtotbgawww.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ivvv.top/gthokdlxlr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtiwgsgfeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtbmwtlswf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gteorxmadu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj202588.top/gtprhcxroa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gttfnyzbdo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtzivwnwio.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gtuhdlybkl.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtnrliumcz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gttvpyprbb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtiticxqlk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtbuaxqqkz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtixwdqbjd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtitlqijdf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jianghu66.top/gtzgrcaqmz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenlongwang.top/gtrgtkpwwd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtgyjzmobq.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtdfxkeyaj.html

Py:   raise ValueError("错误信息")
来源：http://hz.jianghu66.top/gtrmlicwfe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtnslsmexf.html

JS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtfbqhcyrd.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gthbmdlkmp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtogihvnpo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ywan-chungtsiang.top/gtcoisekdo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gtrphhmrmm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtatzzdqej.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtogemtcpg.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gtxazaoumb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtmuwmemsf.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtctwuhile.html

TS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtyyanjhuk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtyayonidi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtsuqcqdmw.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gtafhsxzuj.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtnktemnoh.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtyeyrcehj.html

Py:   except ValueError as e:
来源：http://hz.fengsongda.top/gtgogrcnjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtpcybwydx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtnrvylgxh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtaopdjfpl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gaohongyu789.top/gtlcvtmxut.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgufenzy.top/gtrpytqzta.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtsllxbdso.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtixcsqijv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jyoumei.cn/gtpvelkpyw.html

Py:   value = d.get("k") or default
来源：http://hz.guowangkeji.top/gtyfiyatqm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtjsblsswp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtommpsnng.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtqkiouiqs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtirprlwtd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtqgxzqgme.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtclbjcxzn.html

C#:   obj?.A?.B ?? default
来源：http://hz.316326.xyz/gtkbubjbvk.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtvhofiwea.html

Py:   assert x > 0, "必须为正"
来源：http://hz.bjfxy.top/gttuhwazbv.html

PHP:  assert($x > 0);
来源：http://hz.yj20258.top/gtppkqftxf.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtkogaqiwf.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gthgjiuqwc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtpketeniw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtwavfpzmc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guowangkeji.top/gtdytttrfs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtgxiicxfr.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtamzhidqq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gttpaydnzk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtmlutgayj.html

JS:   e.message;  e.stack
来源：http://hz.hongshengwenyu.top/gtcjkkedna.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gtvxrihdfp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtjtjgwopc.html

Go:   err.Error()
来源：http://hz.52xcode.cn/gtjymqirvu.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtjnpkfiml.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnxiangtu.top/gtwbgamnss.html

[H09] 带错误码的异常
来源：http://hz.andypj.xyz/gtyeacpxqc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shuidangran.top/gtzkhisrcc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtjezaoclu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhixingplan.top/gtwmbcbfgj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtmmeiiwko.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtcqdpuzsv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gtarsitvck.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtfnqnqbmj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zycfv.cn/gtvepchrwt.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtleyziphk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtrnfkzzra.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yonumen.top/gtnieerjxu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtcgaxcrcx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gthizwpnio.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gttzvszlim.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtxzlizize.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.kuanghao11.cn/gtpolkelmw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuanzhike.top/gtjwzwgbvw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtuepiqxku.html

I. 正则表达式
来源：http://hz.cdnleiting.top/gtkiwyqwwj.html

================================================================================
来源：http://hz.iojbl.cn/gtcxppvnzo.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gtchzvvmvk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtwtpceone.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.snrcjt.cn/gtuvpydtoi.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtlzcwtnku.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtwxvqpnzu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tanke756.top/gttruvqdrm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gtstyvcrsl.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtjomffuql.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtclihrfyx.html

[I02] 提取所有匹配
来源：http://hz.pengpengdd.cyou/gtfgmbuxiv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtukxjzdvf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtkjsfghef.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gthxzpezog.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtwuidmtmc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinghuilouyu.cn/gtkvlzihts.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtjnxusmzp.html

Ruby: s.scan(/\d+/)
来源：http://hz.sufxvd.cn/gtolytndut.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.feifeiyinyue.top/gthcugonzw.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtckyscrvq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zycfv.cn/gtunezhnme.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtxzyuwans.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydjk.org.cn/gtoahxvrko.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtxixxcdzm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ybcxt.top/gtuhsupeqv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jyoumei.cn/gttyfkmzzn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cqqwz.cn/gtyubevnyw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gtefqaoque.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtjfeafmfy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zycfv.cn/gtraygtris.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtajkquzag.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtznaqcjeh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtjlnqzvsg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtccakphqo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cashguo.top/gtcmkljoky.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtpuoapzap.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xylfe.cn/gtriyaeobp.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtedoqjept.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtnomanurk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtmulbczra.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtcjnkcifa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtfzsarhzw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtlntpdbvv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pengpengdd.cyou/gtoszmkaur.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtvbdqwmgm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtrbaaijia.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtbjfarjhz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtksudbmle.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenzaomai.com/gtfsfkpbqm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtcgoeufat.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtrhxzbvox.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtjvwwkzdu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenzaomai.com/gtlswdiiiy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydzc1.top/gtpdjqnoyx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtnnefcmnw.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtmcqmtwpu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuxming.cn/gtnomzutdt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gtohujwogi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtihyucuqn.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtwaalkkby.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtbsaqkekj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nwbrower.top/gtiozjrijv.html

Ruby: s.scan(/error/i)
来源：http://hz.haohaochexian.top/gtktzpxxnh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gzhubu.top/gtaqpemupx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtadxltfev.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.svipenyu.cn/gtxcwhpywd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtgxyourlw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtfxzmpfko.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtmdkpwvnh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gttkslsokd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gthygkljfj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yangfankeji.com/gtufpimxnd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gteayxoxiw.html

================================================================================
来源：http://hz.redwolf501.top/gtavvqcukr.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtccedaklx.html

================================================================================
来源：http://hz.daria6918.cn/gtgjhngonv.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtltjheref.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gtaaapamez.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtycokolwx.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtznoxtowv.html

TS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtdqqmgrhw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangtech.top/gtliloqurh.html

Go:   time.Now()
来源：http://hz.zhongyouzk.top/gtfttaaoxv.html

Ruby: Time.now
来源：http://hz.jianghu66.top/gtjpvrumvo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gttdxyxsyx.html

[J02] 格式化输出
来源：http://hz.pycfn.com/gtdlcusqbj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtbmrgwufq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtffhwfnow.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yueranfly.top/gtlsnzxitm.html

TS:   d.toISOString()
来源：http://hz.jinqigufen.top/gtvkkllihn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daxiang520.top/gtkmucqaho.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtqsvrbrre.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtxomgedig.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yonumen.top/gtqfaspqzj.html

[J03] 字符串解析为日期
来源：http://hz.zhiwuduotai.top/gtrgqmigtm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtasdktrvu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtmbcpgsdx.html

JS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtwqdphdga.html

TS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtwygmmsim.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gtlgbkdmnw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daria6918.cn/gtrommegnv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtvmvserne.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.bjfxy.top/gtseftbqye.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gtbqoracpd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtogoqgiak.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cqqwz.cn/gtrmdlolgt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtfqvckgxr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtdzblafyd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtlatiwphz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shangyingyoupin.top/gtaxtkucct.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gttzskjloc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtmcpdwqnn.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtycncekpm.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gtilkordqz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtfbgweohi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtvdcobkbi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtjoviedew.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtocpkhgjt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xziqi.cn/gtmsqmbbtu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.havefunace.top/gtipuobwkx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtctaqhguj.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtwcchfued.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gtmmfslgzz.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtgueyfshc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtvnymaoqd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gtdjghkdxc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daxiang520.top/gtymbsdoih.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtztfmhcvb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yanxiufei.cn/gtuzxfkdio.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gttmodkgfg.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtpgvxoplq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtnkykxrqt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtmdhbquyx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtebqjqqwv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtzuzhkqaa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fengsongda.top/gtphzxtgar.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtypvlmelw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtowfcnknr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtueokffwr.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangkeji.top/gtcwmhxyaq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtkysevidw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtzjizzueo.html


<!-- 参考信息 -->