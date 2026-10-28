代发 wailian999

[G10] 访问控制
来源：http://hz.sysykeji.top/gtwpzbkehz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtvgkamdad.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtvzovbgsb.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtxxcrlyye.html

TS:   public / protected / private
来源：http://hz.316326.xyz/gtbmposzwv.html

Java: public / protected / private / 默认包级
来源：http://hz.cqqwz.cn/gtujqqmtrg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtugwajrdm.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtsabfefcd.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gteesbsceb.html

[G11] getter / setter
来源：http://hz.zhijiandao.cn/gtimyyvuzq.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gthvbdqtki.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtvobluawy.html

JS:   get name() { return this._name; }
来源：http://hz.wangdashe.top/gtyotvejxx.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydzc1.top/gttcwzhjdz.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtayqzdops.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gtcmdtyskm.html

Ruby: attr_accessor :name
来源：http://hz.smart0.xyz/gtaffzbpti.html

C#:   public string Name { get; set; }
来源：http://hz.redwolf501.top/gtumkwskqw.html

[G12] 对象转字符串
来源：http://hz.gzhubu.top/gtbcjvdihl.html

Py:   def __str__(self): return self.name
来源：http://hz.pengpengdd.cyou/gtrtpfexdi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hammf.cn/gtsevzqqza.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtmrapmyoo.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtjklheare.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtjghrghmg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtzfhqckhl.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtigsohfsx.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtvctljgsl.html

[G13] 判断对象类型
来源：http://hz.zycfv.cn/gtmrnaizru.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gtrmgqmtvf.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtxgtlswce.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtecvkimec.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtfzfmjmyb.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtqlnkwsqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gtimqsqvfl.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gtbcntdwxc.html

C#:   u is User
来源：http://hz.daria6918.cn/gtcvzirdzs.html

[G14] 数据类 / record
来源：http://hz.wangshuangyany.cn/gtjitqobhz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xingfuxueyuan.xyz/gtigqdklhb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtmqtqtxwg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnxiangtu.top/gtmggibyhf.html

TS:   type User = { name: string; age: number };
来源：http://hz.bjfxy.top/gtcnffjjsi.html

Java: record User(String name, int age) {}
来源：http://hz.pengpengdd.cyou/gtqogqyvqz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtewwdjyvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.0kj1m.cn/gtfrjfztrm.html

C#:   record User(string Name, int Age);
来源：http://hz.hongshengwenyu.top/gtdpmhgnsy.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gtwezljhlh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtzndmtqes.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.vqdsnc.cn/gttxtfcrpy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gtwmwrxxkm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gttupnbans.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtsnrsvrbw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhongyouzk.top/gtpklqjqqo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtjnjalsev.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtjkbipoee.html

[G16] 对象转数组 / 字典
来源：http://hz.ybcxt.top/gtedmjecnl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gttacugkrt.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtibxecjkd.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtmckexbrh.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtshitmqwl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtzxnskzvk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtyehoanog.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtbssvhrpi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dianchejie.cn/gtgajhkvrm.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkocramdz.html

H. 异常与错误处理
来源：http://hz.ydzc1.top/gtpdydngng.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjsovbsdi.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtknbkmyqw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ppjwa.cn/gtkzknymie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gtkbevwaxc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtmmbhaoof.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtkjjluled.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gtsbpstklg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cdnleiting.top/gtqtrhiiwx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtblgaimmw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtyhvwfiot.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtatkbvixm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gthaapmojb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtympbseut.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtxyohfuxx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtmnfazaqr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtjcrpdtic.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuanzx.com/gtkftxggqw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtfaoarktl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.haohaochexian.top/gtbcoxhomr.html

[H03] 主动抛出异常
来源：http://hz.sysykeji.top/gthnoffilv.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtwfzxchqs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gttrhqawej.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtcagqytga.html

TS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtlkcqaeql.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtvmginhit.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtvxhtaeww.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtsyjvzwzt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtkunkxpqt.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtubulrktn.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtxwngqrol.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtvhsflvin.html

JS:   class MyError extends Error {}
来源：http://hz.aibaodan.cn/gtrgmafxuy.html

TS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtpdhzpzht.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fengsongda.top/gtrdfjrkgj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtmecrayoy.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gthtzxvafa.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtcmvdzhoo.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gtwvwujjzm.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtyipeicjc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtprnxjask.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtsnpoyyku.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtcpyvtxlp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgfzy.top/gtgernkdjj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fengsongda.top/gtxjbqjbso.html

Ruby: rescue ArgumentError => e
来源：http://hz.9152youxi.cn/gtpjxbznrw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtycurpcqx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtkthpvipe.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gtpmatdige.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtnbvvdfql.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtngefpujm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtvknscxtu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtmzujxpns.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.meibo888.top/gtmgcghfye.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtuojuhuqq.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtutddaldl.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtyjsazahw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangtech.top/gtbxzclnnu.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtawmdvjru.html

JS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtehchkmay.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtbdyfpzrj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtbfmstinb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xingfuxueyuan.xyz/gtktugbjkf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.vqdsnc.cn/gthykgmfnd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxinkj.top/gtnvuldwpg.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtsvvwycyh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.haohaochexian.top/gtatfinsfu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtwwxgtblo.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtbjthmyzh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cashguo.top/gtcygifgnp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtfobuswes.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtbiwzqarj.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtjkfpmutt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtmialcqct.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtdqdsplcd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gtqduakiks.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinyuanbaomall.cn/gtcynljiay.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pycfn.com/gtfvwwobhk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtjmwklhlx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtjgcijlrh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtkfcxayqr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hysaishi.cn/gtrgpvihzw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuetiantiany.cn/gtvmdbvorm.html

[H10] 资源自动释放
来源：http://hz.sysykeji.top/gtprjdzqmj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gtjlrkhdvp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gtymxerlti.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtfojinomi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtqdixajuz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtsdvqcabh.html

Go:   defer f.Close()
来源：http://hz.yj20258888.top/gtgfibxnse.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.vqdsnc.cn/gtqzvwoecs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gtgyipbvpy.html

================================================================================
来源：http://hz.0kj1m.cn/gtweeibovk.html

I. 正则表达式
来源：http://hz.shzxlz.cn/gtfhwzspgk.html

================================================================================
来源：http://hz.cdnleiting.top/gtcnflqsep.html

[I01] 判断是否匹配
来源：http://hz.yanxiufei.cn/gtqgylbfyo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenlongwang.top/gtddkebxhn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gterzlwcmf.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtroxdshvi.html

TS:   /\d+/.test(s)
来源：http://hz.bjfxy.top/gtndrfiatt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtwfjtgqqh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtwcajsspc.html

Ruby: s.match?(/\d+/)
来源：http://hz.hywenlv.cn/gtvzyufgie.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtqutjlvrq.html

[I02] 提取所有匹配
来源：http://hz.9152youxi.cn/gtkjkhlwmc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gtjovpibux.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtzkjaqvxi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jyoumei.cn/gtcugqosro.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtzkfcaxnn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.vqdsnc.cn/gtzqwvpmql.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gthofaqwkv.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtdkavnxya.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtnygmpxvi.html

[I03] 提取捕获分组
来源：http://hz.mhx1999.top/gtvwvzjaxw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtozzzdeos.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gtycaaqwgb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtbpqylizz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gtilmiaojg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtixbwvaac.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtiwvopwvp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydzc1.top/gtmjypoqhq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtfqtsjucg.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtepkbyooa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtcovoinbw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtmgvlfute.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtxsfcehya.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtvufuzpyl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtlwwdrlpt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ehwqpu.com/gthsommkto.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.c1oappe.top/gtxiiufqdp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtodsnjjgh.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtidutaknx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtmskokwqv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtoeykxxjt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gteybfefnm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtighsrbya.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtkyfkbduv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtgfrufuom.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gttcarcgws.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aibaodan.cn/gtmfvfkpzx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fzhhl.top/gtakrotqwx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtopfzqoxv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtmptluuhx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtlknoqsak.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtyhjnpxuf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gtkzmbjnvp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtbiujfgle.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gtuppvsqja.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtjmgpnukk.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtbygsqkdy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dashuyun.cn/gttobpldap.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtapiibtoc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.iojbl.cn/gtsqkmlilq.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtmlyfyguq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gttmfqoxts.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.redwolf501.top/gthhnwalbg.html

Ruby: s.scan(/error/i)
来源：http://hz.yvedp.cn/gtnhkiumbo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtplgfcjkv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gtvlkdfxwt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtmqqovfno.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shangyingyoupin.top/gtgpvcfhkw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtnswqhjtb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtxfnuoeyu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtkljqcpiv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtfpqczhhd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuetiantiany.cn/gtchhfxndx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.iojbl.cn/gtdislepst.html

================================================================================
来源：http://hz.9152youxi.cn/gtpaxnhzdf.html

J. 日期与时间
来源：http://hz.vqdsnc.cn/gtvcampzpv.html

================================================================================
来源：http://hz.tanke756.top/gthmxpanhl.html

[J01] 获取当前时间
来源：http://hz.yj20258888.top/gtzcwbbglm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gotoacloud.top/gtdnpiqoat.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtytjlkasx.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtrawljpgc.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtcvccqbbm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jianghu66.top/gtdohgbqxv.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gtcsbvzuoe.html

Ruby: Time.now
来源：http://hz.yj202588.top/gtvfccocnd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtnqsdckvw.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtemqtvlhv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtpvvqzxaj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtkwydvgwg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtjkwyjqkl.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gtzzzmdtcc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtpxyuxrqh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtyadhxuqk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtifucpxvy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtdjtnxtmf.html

[J03] 字符串解析为日期
来源：http://hz.ydjk.org.cn/gtrdbcjyxk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtwytprfek.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gtdswvbidg.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtrleohago.html

TS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtkdswofvv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtksamrakl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtnkusmwpz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtoowjinbf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuanzx.com/gtpepzwdyr.html

[J04] 时间戳与日期互转
来源：http://hz.quarkkingdee.top/gtarxtujpm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtxwymqtpi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ivvv.top/gtdwrznave.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nwbrower.top/gtwicmjfqt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtrzxvprjw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtgkobiwno.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xziqi.cn/gtxlohaexw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangkeji.top/gtoipuaqgg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtvpeklear.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gthpyhxcpp.html

Py:   now + timedelta(days=7)
来源：http://hz.ivvv.top/gtimkihlga.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtmqgovarv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtetkojrli.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtknmnkhve.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gtwgdeffxl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zycfv.cn/gtwxdtankx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxinkj.top/gtpubstdgb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtpprriviq.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtourxewhg.html

Py:   (end - start).total_seconds()
来源：http://hz.dianchejie.cn/gtnkmnvunr.html

PHP:  $end->diff($start)->days;
来源：http://hz.jyoumei.cn/gtpapcrprq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gaohongyu789.top/gtkzjyufbx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gtcvydnbsx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gthbshvpgv.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenjidiqi.icu/gtduftwyme.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtlyucxdyk.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtpjcndowj.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtjhmschvy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtciigydik.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtisixmyog.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtzkdtihcx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtpxwqehrj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtfsbocouy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cheryme.top/gtufnyghxk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtrirgqdqw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtbpgsuxvw.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtxzzlazoj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sysykeji.top/gtpajofyvn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yanxiufei.cn/gtsdxeeifk.html


<!-- 参考信息 -->