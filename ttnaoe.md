代发 wailian999

Java: u instanceof User
来源：http://hz.shuidangran.top/gtdkvpznkp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenjidiqi.icu/gtubfdohbb.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtcgjkzqnd.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gthdkbvaqv.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtogjpixva.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gtajstqror.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guowangkeji.top/gtzywjpspm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuanzx.com/gtaoswmevg.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gthvsxpzqe.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtlgyuyfks.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhixingplan.top/gtaprfdrjc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtpwvxmsoa.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtpjtakaqm.html

[G15] 枚举
来源：http://hz.tanke756.top/gtttnblpmp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xziqi.cn/gtcpoauzhu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtmiuizqle.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtsltwqqkk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtvmqtuxkj.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtkckhisbs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtyxeggkrb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtemuxsjoh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gthsiodrle.html

[G16] 对象转数组 / 字典
来源：http://hz.mhx1999.top/gtquuwomse.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gtxjqornmf.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtlfscanuz.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtbclvxmuq.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtekcavfno.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtftxasark.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhongyouzk.top/gthbouzaxo.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtofnficgo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gogol.net.cn/gtbktvvuxi.html

================================================================================
来源：http://hz.smart0.xyz/gtpcheecds.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtzkgnjjmr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtscfogvti.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtpsqeaynn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtaudzwyiz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinghuilouyu.cn/gtjhjriwco.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtxbzmmwiv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtjjoumnjw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cheryme.top/gtalcxjlcf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gtsjycrsfp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shzxlz.cn/gtskjvykiq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtozzmkzfr.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gthngktzcf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgfzy.top/gtikbovjhs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtnmlmwikn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtxngtzmrd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtthshmnlf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtwkzdnpue.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtxnvzuuki.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ivvv.top/gthmgiwxip.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.mhx1999.top/gtvcfksada.html

[H03] 主动抛出异常
来源：http://hz.0kj1m.cn/gtfbbobnum.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gtpeizfzke.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtvrqhdrex.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtvkfizwtv.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtikwkdtpo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtahksfvph.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gtodfqotvp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ivvv.top/gtixwqolxf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtqkpnnmjq.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtredfnrkk.html

Py:   class MyError(Exception): pass
来源：http://hz.xuanzx.com/gtslgazbgs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtvgqvbxcm.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtvmrhande.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtpvxwyoyu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtmaxacxil.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.mhx1999.top/gtxevfawwk.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtkmfkmwxp.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gtwguhylqk.html

[H05] 捕获特定类型
来源：http://hz.sweek.top/gtxfrposrq.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtcxhkcdai.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cheryme.top/gtsuzqwimh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtlwwemlih.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtcltaoveg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtyhkmfpkd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zdqjudy.top/gtzbwxpxyx.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gttrxpsadl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtdwrsdkxu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gttpxeejwx.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gtxodvluob.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gtloddqrml.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhongyouzk.top/gtyfhyeiil.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtbqzwbtur.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj202588.top/gttokszqnx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhaomingkeji.xyz/gtlyrsxgnv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.aibaodan.cn/gtsfacovzt.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtjexgshdb.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtpqnyyhqz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cashguo.top/gthgldkgbq.html

PHP:  assert($x > 0);
来源：http://hz.yongpay.top/gtqdssnycp.html

JS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gtacmsxzxe.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtyrseklqx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xylfe.cn/gtiswjlnfe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gttnarqnnu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.52xcode.cn/gtmcqtwwtz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gttnwuubkr.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtiiojalkv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtldgilfyi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtgudemzrj.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtyapvilwo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.quarkkingdee.top/gtxvtetglp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fengsongda.top/gtmbzpgyzq.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtwgmgvlqr.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtbpzneyfr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gzhubu.top/gtsezhluqv.html

[H09] 带错误码的异常
来源：http://hz.wangdashe.top/gtumfxtbwf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtkkgsmspv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhongyouzk.top/gtnxbutkct.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sweek.top/gtwnckdxja.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tian-w.cn/gtvjrxxbop.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gtbafpxpgx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gtoenocpwp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gtjsltjspj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtfisqxrmg.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtvqiwlovl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtclqfnbnu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtmppvgwns.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtokrokvqb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gtxmrzybaf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gthnqqmrui.html

Go:   defer f.Close()
来源：http://hz.snrcjt.cn/gtsmdgvlkv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tianlin.xyz/gtzuabwnwa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtnzrfmkqn.html

================================================================================
来源：http://hz.cheryme.top/gtftzrfwvk.html

I. 正则表达式
来源：http://hz.cdnleiting.top/gtscljtzgk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtlbxvkuqu.html

[I01] 判断是否匹配
来源：http://hz.jinyuanbaomall.cn/gtrjsolpcx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fengsongda.top/gtyahhszat.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.snrcjt.cn/gtwubjmtop.html

JS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtiqudozpb.html

TS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtqmccagcc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sweek.top/gtcduitjdb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtbwgcpksv.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtqqhpaycx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.kuanghao11.cn/gtxxejzjbh.html

[I02] 提取所有匹配
来源：http://hz.ydzc1.top/gtvrapzbuk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhongyouzk.top/gteosusizg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gtwstustck.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgfzy.top/gtzunijrok.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gterwkjnba.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cucudq.cn/gtgaznvhpx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtnivowlnl.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gtjujpanln.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhengqikj.top/gthirvevrv.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gttgiacwmu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.bjfxy.top/gtvqbxocea.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.snrcjt.cn/gtbrdxjdoc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.smart0.xyz/gtxigmgqpm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuanzx.com/gtbkdaxdnb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.feifeiyinyue.top/gtidjrutkb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtfiwnxphl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtyknztlwb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinghuilouyu.cn/gtmsmxeiwh.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtjvfcblht.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guowangkeji.top/gtbcmvbydi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtjqtiqxfi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtivdsippq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtfciqjwmv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhixingplan.top/gtpbxccoxc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.52xcode.cn/gtjuntrylz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gthaxzmnzh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gotoacloud.top/gtbvtvlgyt.html

[I05] 按正则拆分
来源：http://hz.jinghuilouyu.cn/gtoczistlh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cdnleiting.top/gtwjbkplxz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gttznivrwh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtnzadxawc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtnxrcfqrd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jiagoushi.top/gtfoqyxcik.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gtqautinlo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtweldoigm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtuxrlycfx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtqqvectvx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtvnuskcsv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gtqbluhnul.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtwuhibest.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtfffxqrjx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gtlftrmmxu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtlcvzoalk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gtouaqzytz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtmyegdyxn.html

[I07] 忽略大小写与多行模式
来源：http://hz.jyoumei.cn/gtsqhqauvj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.havefunace.top/gtxxnmbcjk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtfggqzwwq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.52xcode.cn/gtdfkybtzp.html

TS:   /error/gim
来源：http://hz.pengpengdd.cyou/gtlxgggiye.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuanzx.com/gtnocnwgrk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.meibo888.top/gtjqeyyrxi.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtxgdvwwrj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.andypj.xyz/gtwsuvmsag.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gtpjbwbrip.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.316326.xyz/gtbuvdnmij.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aizwys.cn/gtrnorshgv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gteryaeobz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gttsvuhehk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtbjdwnidb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtuygtzpiu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtcupxyuaq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtgxdcnmkg.html

================================================================================
来源：http://hz.jqgfzy.top/gtrazoxhre.html

J. 日期与时间
来源：http://hz.yj202588.top/gtmlziynkk.html

================================================================================
来源：http://hz.tian-w.cn/gtntopatnk.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gttabulmoy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtnfteukrn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtzocwyxku.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtaeujoiec.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtifhukbyd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.haohaochexian.top/gtxuonwlda.html

Go:   time.Now()
来源：http://hz.yongpay.top/gtrnhykzuk.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtevickped.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guannengcc.top/gtdnujlupd.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtvffcadyx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pengpengdd.cyou/gtyhsquuqi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtfqfwxqju.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.9152youxi.cn/gtrlfhauto.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtxlxexihw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tanke756.top/gtjebtcnst.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtklaepwet.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtfibjlbby.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtybwvrsdl.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtgoouswup.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydjk.org.cn/gthqkbqkct.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yanxiufei.cn/gtpdwqbqtk.html

JS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtgovqbxrq.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtkhhsfpeb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cashguo.top/gtxgxxynaz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydzc1.top/gtlhgnaitc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtlegrrtya.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gzhubu.top/gtfmhpbemn.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigufen.top/gtmtalboiv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtqserepbi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtmvkhdfzr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gthmizhqlv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aizwys.cn/gtlzgxlnki.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yongpay.top/gtrwrlmdfp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gttmkztngr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gttexuksnf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtzyhufsbb.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtxttxrzcu.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gthrmipwgg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtxrwypsjj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtlatuhnua.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtwczjzywd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtqpepfowg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sufxvd.cn/gtsirjdewz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gthsstgpru.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.feifeiyinyue.top/gtwfnxwtry.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtgtpjalga.html

Py:   (end - start).total_seconds()
来源：http://hz.gaohongyu789.top/gtrtlsxdcy.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gthuqqhrtf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhoulong.xyz/gtbiahkzoj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gtavbydwmb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gttqjtalxv.html

Go:   end.Sub(start).Hours()
来源：http://hz.cashguo.top/gthzgpzpfs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtsnzmhcbc.html

C#:   (end - start).TotalSeconds
来源：http://hz.daxiang520.top/gtasfqfqwn.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gtoyxbioqs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtlrozhgon.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtonvcresx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtjavukpls.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.dashuyun.cn/gtzyrkeqir.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangkeji.top/gtehmxvgly.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.quarkkingdee.top/gtimluisgd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtxkxvtzeo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtcrfwigax.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gttawvnhrt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtjelxczrt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghu66.top/gtnwoqueol.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.andypj.xyz/gtozajqyha.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtgzegajnr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtsywzaucn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gtelrfvqiv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fengsongda.top/gtozocnwcm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cdnleiting.top/gtmmtqxmwg.html

[J09] 时区处理
来源：http://hz.feifeiyinyue.top/gtittxqsxv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gthrvtueup.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtkiutjutt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtziggivbo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtkrrufeal.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.feifeiyinyue.top/gtadrywrqk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.haohaochexian.top/gtucoacmgj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtlchlfjjl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtntggmwyc.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnqzz.top/gtzdbgueek.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtddhbvuvm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtfuvvedxw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydzc1.top/gteapooulh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtdqzcxrat.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.snrcjt.cn/gtknhtwchk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sxryk.cn/gtcngwugac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtkrlbteba.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yangfankeji.com/gtqwmspvjw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtorrlynww.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtshzqqeyf.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjwkufxod.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhongyouzk.top/gthadswbkp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtrkapkeqs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtxofhxljg.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtbqhmdehj.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtttwqstmi.html


<!-- 参考信息 -->