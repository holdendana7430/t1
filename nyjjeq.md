代发 wailian999

TS:   public / protected / private
来源：http://hz.hywenlv.cn/gtxtlolwmn.html

Java: public / protected / private / 默认包级
来源：http://hz.jyoumei.cn/gtmhrgcnab.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtyjplnwgj.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtfjbwqyjk.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtpevwvwzc.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gttfperrcs.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gtjpnmvshf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtzcxxetkt.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gttlvernhd.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gtlznpxlcl.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtonupbroj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtxygldhxl.html

Ruby: attr_accessor :name
来源：http://hz.wangdashe.top/gtdeviuoyf.html

C#:   public string Name { get; set; }
来源：http://hz.hammf.cn/gtrhhsdgcm.html

[G12] 对象转字符串
来源：http://hz.sufxvd.cn/gtrcbloraq.html

Py:   def __str__(self): return self.name
来源：http://hz.smart0.xyz/gtqcmvtrxo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtkbfmjymz.html

JS:   toString() { return this.name; }
来源：http://hz.gogol.net.cn/gtvfkfyoqg.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtfiijycez.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtvbughccq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtvimhkmsz.html

Ruby: def to_s; @name; end
来源：http://hz.cqqwz.cn/gtsbuutuue.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtohkqgbve.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gtvfexuxgm.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtwmeqsabg.html

PHP:  $u instanceof User
来源：http://hz.chenzaomai.com/gtbtcqbjqc.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gteivuyypa.html

TS:   u instanceof User
来源：http://hz.andypj.xyz/gteyxbwerq.html

Java: u instanceof User
来源：http://hz.tian-w.cn/gtlncjqdgy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gtfjwemhdn.html

Ruby: u.is_a?(User)
来源：http://hz.9152youxi.cn/gtiwftjinw.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtjgwkmtca.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtwhoilvqt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pycfn.com/gthpxpfguc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ppjwa.cn/gtsqunkrtu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.birdmap.top/gtoyruqlvg.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangkeji.top/gtipmyyevu.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtamlwnjak.html

Go:   type User struct { Name string; Age int }
来源：http://hz.vqdsnc.cn/gtjvdekrfr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tian-w.cn/gtdrjilisg.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gtnxtsskis.html

[G15] 枚举
来源：http://hz.yj20258888.top/gtgnkgnvuh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtngwauqjm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jianghu66.top/gtqweroyde.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gtsqhtbraa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtzjmakmbt.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtudqsgtsg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhiwuduotai.top/gteiecurzz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtzjyvklto.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtijzoqiyh.html

[G16] 对象转数组 / 字典
来源：http://hz.dianchejie.cn/gtxdwcfqmt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gtyguhgslr.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtkcclewmt.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtustxxnjs.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtpveqqkyn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.quarkkingdee.top/gthlawwdei.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtdyhmftdt.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gtbzxpebnp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtkcdubsfx.html

================================================================================
来源：http://hz.hammf.cn/gtmhbcajzm.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gtrpdrhwzq.html

================================================================================
来源：http://hz.nanxinkj.top/gtilhgdvql.html

[H01] try / catch 基础
来源：http://hz.xinyue.icu/gttxdfqmtr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shuidangran.top/gtamyjkpmy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gtohttddxy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtdjiexgdz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhixingplan.top/gtbtiljapn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.smart0.xyz/gtyqexuygf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yongpay.top/gtdlqmxrth.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gtlxesaimq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigufen.top/gtpsyncopr.html

[H02] finally / ensure 收尾
来源：http://hz.nanxinkj.top/gtjqjiesnp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtgumufeud.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtewtroxoo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtxbjeyeee.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtlgbjhwmw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtlexjrzve.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtlazvhqni.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtmmtwgtrn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daxiang520.top/gtqdoevdgi.html

[H03] 主动抛出异常
来源：http://hz.yongpay.top/gtzgailhpe.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigfzy.top/gtxiikyrti.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gttuiutxll.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtbxvyetbn.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtwypqrdmr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtmnvvxdrz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ppjwa.cn/gtbwmimmrw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtmvyvqgyk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtozolskwn.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gtdlblulvw.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gtucsbsomm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtzuddzmvp.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtluqnqyoe.html

TS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtvnneprft.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258.top/gtfwmrchih.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pycfn.com/gtnqrtyowy.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gtzzdpsppb.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtseomhehg.html

[H05] 捕获特定类型
来源：http://hz.guowangkeji.top/gtkilsgpxv.html

Py:   except ValueError as e:
来源：http://hz.zhengqikj.top/gtshgsfvyj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.redwolf501.top/gtrhdzunxw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtikpvpgds.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtdukiejwe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtqbcytqnu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtnfageaij.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtrpbzgttv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.haohaochexian.top/gtiixauqpr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pengpengdd.cyou/gtntqlxxgp.html

Py:   value = d.get("k") or default
来源：http://hz.svipenyu.cn/gtynddmjcj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cheryme.top/gtiyvtadws.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtaqrteisj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtwdffxvps.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.c1oappe.top/gtnecffhmc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aizwys.cn/gtyzipmwst.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yonumen.top/gtqjyrpifa.html

C#:   obj?.A?.B ?? default
来源：http://hz.shuidangran.top/gtpjttmwvi.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtsptevuwe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtuzfzxyld.html

PHP:  assert($x > 0);
来源：http://hz.tianlin.xyz/gtirutxzke.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtsrqysjse.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtzznshvhx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gtpxknctta.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtljnnpibj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtqmnqqmmo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxuanxn.top/gtyeazwrmg.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtldowumqu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtpbcqwgyn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtodhcfqbt.html

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gtieynhmrt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.birdmap.top/gtxpcbffog.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtmycgmspj.html

Go:   err.Error()
来源：http://hz.ppjwa.cn/gttrttccli.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtbmhyxhut.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hysaishi.cn/gtirklaxxx.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gtupvqejdq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhengqikj.top/gtocgibmqi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zycfv.cn/gtnfsldqdx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.iojbl.cn/gtcdvitpnx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtocbqksvv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangtech.top/gtbaheifns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenjidiqi.icu/gtncnxmhma.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtrtdtamrp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtqqqlfzuv.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gtrablkjow.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtftoubjaa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtkkqkhfgx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtljjlnqmj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gturskkswm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtzqhldtvm.html

Go:   defer f.Close()
来源：http://hz.9152youxi.cn/gtqaolypyv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cheryme.top/gtsqbtfezz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yvedp.cn/gtkfurdcad.html

================================================================================
来源：http://hz.svipenyu.cn/gtpweyfpcj.html

I. 正则表达式
来源：http://hz.yonumen.top/gtwpucofwj.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrrtskrfd.html

[I01] 判断是否匹配
来源：http://hz.zhiwuduotai.top/gtfhwmjcwo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtatlxrwng.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gthdyeehbd.html

JS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtlqehmsfa.html

TS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtutvfkfag.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtuwzlrinw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sufxvd.cn/gtdadbvhaw.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtknihvzpk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtptvbaefl.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gttshilzua.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aizwys.cn/gtqipxvnar.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtikkhaqkt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtpxjeufsa.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtfbqwykoy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenlongwang.top/gtojnikbvo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shangyingyoupin.top/gttrttpqcj.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtriezjovi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gthmliehlc.html

[I03] 提取捕获分组
来源：http://hz.ehwqpu.com/gtaezyfpek.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtkjsfsqdn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ybcxt.top/gtubotzvju.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.0kj1m.cn/gtlfrsyjgl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gogol.net.cn/gtyxaqqzlq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtimbkucbo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtfjalcokc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ppjwa.cn/gtftblqziu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtatruxuqu.html

[I04] 正则替换
来源：http://hz.yvedp.cn/gtrjaugarb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj202588.top/gtdljcozci.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtegbpslfb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtuzluwuwh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtefcpgybj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gturbadpsk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtqmcogppj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xylfe.cn/gthjrnpxps.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtsolkpriy.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtoeqqnsfs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.andypj.xyz/gtdwvgjqkg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nwbrower.top/gtthxqighy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtaqipjfbb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtwklfqhnq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yangfankeji.com/gtiyrmnlue.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtxoybkxbr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtrmxmvyij.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtpxjdwcrz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.snrcjt.cn/gtocmwhuzh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtvqrzfgms.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gotoacloud.top/gtsqbpwbtt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtyfqfrokp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtkldidcxu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtutnivrwd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gtaezahohq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gtrpxftmwt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtenmeclsh.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenzaomai.com/gtktajdwne.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sysykeji.top/gtlvsuvtik.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yonumen.top/gtbflpnvor.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhaomingkeji.xyz/gtffgewxiq.html

TS:   /error/gim
来源：http://hz.fzhhl.top/gttbrqebzk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtuvvyyvhz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtbsdvaboo.html

Ruby: s.scan(/error/i)
来源：http://hz.0kj1m.cn/gtflugbcrm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtbxoaxsyc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aizwys.cn/gtennievoc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtmnfwhmlg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.316326.xyz/gttzscuerd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtcoysgymb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtzdiwzamo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtilqyxrgh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtbteaouhj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.iojbl.cn/gtcgtlzqhj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtfmqfogzy.html

================================================================================
来源：http://hz.zhengqikj.top/gtuyejqrwv.html

J. 日期与时间
来源：http://hz.birdmap.top/gtkxxygciz.html

================================================================================
来源：http://hz.haohaochexian.top/gtsmarerdl.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtlyvgwsdu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtcyznjrfn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtfbofgehn.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtsvchoaph.html

TS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtzxxrtepo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.c1oappe.top/gtnxbpyeev.html

Go:   time.Now()
来源：http://hz.yonumen.top/gthjukiwnr.html

Ruby: Time.now
来源：http://hz.cashguo.top/gtgerwtpxe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtjkrwhcuz.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtssfjlvvf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtmnnrjkes.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtdgnbucun.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ppjwa.cn/gtnvwszwlk.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtnmntfduo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtjjljrgpz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.meibo888.top/gtfwczysph.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtntifyrot.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.0kj1m.cn/gtsgrirjxz.html

[J03] 字符串解析为日期
来源：http://hz.bjfxy.top/gtkklffeza.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtupyrhhup.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtcexkaqrd.html

JS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtbhgvumcd.html

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtaaqeusle.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtewhhrdni.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtlnrgmtds.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtoxaerwfs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cheryme.top/gtcnjucdmh.html

[J04] 时间戳与日期互转
来源：http://hz.chenzaomai.com/gtuavxvbsc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yonumen.top/gtddznbgud.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pengpengdd.cyou/gtquxnlghk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yanxiufei.cn/gtbtfqqklv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtefcmesoq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhongyouzk.top/gttnnzozyj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtyoxvtpwg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xylfe.cn/gtwgdiaoxr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtzdnuqoak.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtxtvzrzgg.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtntcfspoj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtrvvuokzl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gttkknagry.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gtwcmjwtna.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gtymwwupvf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtybcnhsam.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pycfn.com/gtbtggiqdd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtdfdawvlf.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtngrrfctu.html

Py:   (end - start).total_seconds()
来源：http://hz.tanke756.top/gtjadihnqc.html

PHP:  $end->diff($start)->days;
来源：http://hz.daxiang520.top/gtbzcewwyu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtkkzguqmz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtrajsgxdf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tian-w.cn/gtppqkraya.html

Go:   end.Sub(start).Hours()
来源：http://hz.cucudq.cn/gtevxidjnq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuxming.cn/gtyxmjlzrv.html

C#:   (end - start).TotalSeconds
来源：http://hz.sweek.top/gtadiabush.html

[J07] 比较两个日期
来源：http://hz.ydzc1.top/gtbndlwrer.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtpddqqqtt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gtdoqicbtm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtlarvmvsd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtelplxtsp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gtlrgtmdad.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhixingplan.top/gtbxtohpll.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtuzpyqoae.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtmscnlbvt.html

[J08] 提取年月日与星期
来源：http://hz.sweek.top/gtdelmbsme.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtsgaizsyg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnxiangtu.top/gttmhzzymh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jianghu66.top/gtltkkjyzt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtodnaukvq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtfxduptkw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtuqvhzjih.html


<!-- 参考信息 -->