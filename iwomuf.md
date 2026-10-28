代发 wailian999

Java: u instanceof User
来源：http://hz.dianchejie.cn/gteldggzwa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtwutetezi.html

Ruby: u.is_a?(User)
来源：http://hz.kuanghao11.cn/gtlidsslum.html

C#:   u is User
来源：http://hz.ppjwa.cn/gtlomffryh.html

[G14] 数据类 / record
来源：http://hz.yanxiufei.cn/gtnyqjxqbd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtzpidvgfk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.52xcode.cn/gtvmtjvehe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtqxyhvbun.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gtucdjpeun.html

Java: record User(String name, int age) {}
来源：http://hz.yonumen.top/gtptcpwzyz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gtgdzkbsgt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sxryk.cn/gtrcgewkww.html

C#:   record User(string Name, int Age);
来源：http://hz.pengpengdd.cyou/gtitxbowxj.html

[G15] 枚举
来源：http://hz.ivvv.top/gtftvyadzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtiraxtsjh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dashuyun.cn/gtarcjucqp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtcpbwwnyw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtpixgebhv.html

Java: enum Color { RED, GREEN }
来源：http://hz.dianchejie.cn/gttemuehvx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj202588.top/gtdxxormsk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gtajqttyuv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtsnpamacb.html

[G16] 对象转数组 / 字典
来源：http://hz.hongshengwenyu.top/gtvlmikakn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.havefunace.top/gthucftkbd.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtewladatm.html

JS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtjkvawmki.html

TS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtqyqnutti.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gtfkvunqry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtgnxrcpuz.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtwmpxudwr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gthhfkgiyk.html

================================================================================
来源：http://hz.yvedp.cn/gtqhauoswz.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtgmpetnbe.html

================================================================================
来源：http://hz.sxryk.cn/gtdpzkawdx.html

[H01] try / catch 基础
来源：http://hz.yangfankeji.com/gtganirbmy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cucudq.cn/gtswcxbpch.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shangyingyoupin.top/gtectxhpac.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtrfjuymvk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtqijysxdt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtpbapupfc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gthsfhveou.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtkdpjybei.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtuhbovmgw.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtcinokihs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.vqdsnc.cn/gtlgvednhv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gttpnvsqhx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gthddgxyoi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtwfvfkvqx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtbeetyvnm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xinyue.icu/gtqckzwolc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gaohongyu789.top/gtjhhjnspb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtxyskanxn.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtxzlxykde.html

Py:   raise ValueError("错误信息")
来源：http://hz.gzhubu.top/gtppmzqvto.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtdszjmzwi.html

JS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtavgfolfr.html

TS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtfbmzokux.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtqiixfkky.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxuanxn.top/gtleactxqx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zdqjudy.top/gtpxlfwmqc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtpspjzrvh.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtqydvfrsd.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gtxznuwxus.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtqwrpknkl.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtzwuelikd.html

TS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtnzxoycie.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtdkfzfzme.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtgqtthtzo.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gtrhgpzqav.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtqchrtwiu.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gteprebnyv.html

Py:   except ValueError as e:
来源：http://hz.sxryk.cn/gtdxblnufu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jianghu66.top/gtvdcbqrvx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gteznpfejp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtjcpeqmqj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtjxkmlhig.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtjovumumu.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtakdpqqbh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pycfn.com/gttyrcruga.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtwcyqtpvk.html

Py:   value = d.get("k") or default
来源：http://hz.havefunace.top/gtcgnveuyw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtvxygwbiy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtuvxnfqkb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtcjtwautv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydzc1.top/gtmdmhtqsv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtrckvlaxx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xingfuxueyuan.xyz/gtdcukmrar.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtrprsowtg.html

[H07] 断言
来源：http://hz.kuanghao11.cn/gtyqesmakr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtpqvmxkss.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtoecnhroy.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gthcknrxdm.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtfhgigrzy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtimxkpmva.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xinyue.icu/gtgmzsqkri.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.9152youxi.cn/gtkybvvmia.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gthikhutdi.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhoulong.xyz/gtnoravfqr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtjfgqxlhp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gtyixujejh.html

JS:   e.message;  e.stack
来源：http://hz.cdnleiting.top/gtxzsaoqeo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtbanvfjqo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gthokwpdct.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtgzjuysoi.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtrfnwfqry.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtyqnabwpy.html

[H09] 带错误码的异常
来源：http://hz.gotoacloud.top/gtkgqglzhq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gttdurrrel.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuanzx.com/gtjswbmrwu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.iojbl.cn/gtlmlnogib.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtxzigoxve.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtrucrsydh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gthcukudnd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnxiangtu.top/gttphgwgzs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gttorzwstn.html

[H10] 资源自动释放
来源：http://hz.nanxinkj.top/gtbssmbjep.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.316326.xyz/gttqvavrgv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.svipenyu.cn/gtfmdsuyur.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtrzocnius.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtubzdkxqr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtgjsrrwhe.html

Go:   defer f.Close()
来源：http://hz.ydjk.org.cn/gteocyqnfk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jiagoushi.top/gtpsscxkzf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhengqikj.top/gtbhlgsepy.html

================================================================================
来源：http://hz.chenzaomai.com/gtnbahekho.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtvurtddll.html

================================================================================
来源：http://hz.aizwys.cn/gtdczglhmy.html

[I01] 判断是否匹配
来源：http://hz.xuanzx.com/gtffjujkff.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gttvnjgepa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtlpcpiydc.html

JS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtjofzckrd.html

TS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtgrinadfy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtvbmavlas.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zdqjudy.top/gtnorffjzq.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtemboadpd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtchasphkt.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtjvgchjcc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gttbwshbga.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gtmkvkautc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gthubipdow.html

TS:   s.match(/\d+/g)
来源：http://hz.birdmap.top/gtwwnccnhb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yonumen.top/gtoavaihdz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtldhucohr.html

Ruby: s.scan(/\d+/)
来源：http://hz.gotoacloud.top/gtpflyqwig.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sweek.top/gtahltifkg.html

[I03] 提取捕获分组
来源：http://hz.redwolf501.top/gtrlohnogw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daria6918.cn/gtbiwlrmwt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtdswitpzw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shuidangran.top/gthyquzyoz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtqzdmmefj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtefdlsxeb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinyuanbaomall.cn/gtinxofonj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jiagoushi.top/gtqslcidyv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jianghu66.top/gttcpyactm.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gttltgnzye.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtqrwzrboz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jlsjyb.cn/gtcbpypcac.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtlykioabl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtueyxgfos.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenzaomai.com/gtemresevr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtrwjmcolz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hongshengwenyu.top/gttjlyitcf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daxiang520.top/gtmjmanosk.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtxmhphsyh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guannengcc.top/gtsaswochh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shzxlz.cn/gtqsswkwiu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtcoytpilw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtzwgnxfzo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtwsdkxrdd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gttbqdbopq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtsttqhnnv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aizwys.cn/gtfmvckqix.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtoxjblgwe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gttyyucdzw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gttxwftksr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtndesvvan.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtxpfdgglu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gtttfaqrcn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.meibo888.top/gtuimjlmvp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gturtokriu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.quarkkingdee.top/gthjrneuxq.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gthilwvwmj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtiqgvxtwj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daxiang520.top/gtgjgkyfzp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnqzz.top/gtfhutwaow.html

TS:   /error/gim
来源：http://hz.dianchejie.cn/gtlvibmnaw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj20258888.top/gtcxtmqfdw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gtxttahpud.html

Ruby: s.scan(/error/i)
来源：http://hz.aibaodan.cn/gtvemtcqhk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhixingplan.top/gtshistsev.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtpcmkjjnh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gttqzjwzyi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhoulong.xyz/gtvwfhmpzj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtkjpdlxvw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtqdbaeucg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shuidangran.top/gtahyeehas.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.snrcjt.cn/gtqiwmkeqg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jianghu66.top/gtszsuprtw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtiiryzsbk.html

================================================================================
来源：http://hz.wangdashe.top/gtxzoqrswx.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtbkxffxdz.html

================================================================================
来源：http://hz.yuanzhike.top/gtneohnlda.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtvktabbzh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtczgfthkr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtqiwquifi.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gthtyguuyo.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtoxtbcdjj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtamyxqcfq.html

Go:   time.Now()
来源：http://hz.xuetiantiany.cn/gtdadhropt.html

Ruby: Time.now
来源：http://hz.andypj.xyz/gtwxcnodxp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ivvv.top/gtxwqjmzsl.html

[J02] 格式化输出
来源：http://hz.xuetiantiany.cn/gtrkzsngop.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtogtvpjlu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtzkexaszs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.bjfxy.top/gtcmnvydfe.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gttfmlgbgw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dashuyun.cn/gtzcoxprbc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yongpay.top/gttdmnagpj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtmgnbwmtl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtmfvnrshw.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtkcueeavk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ivvv.top/gtornujxmc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258.top/gthdafkdlo.html

JS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtepwgkgqm.html

TS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtopkicjlj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtxzylxzad.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.feifeiyinyue.top/gtnnlhybwp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtnxsiajxn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtnuoxyzsh.html

[J04] 时间戳与日期互转
来源：http://hz.shzxlz.cn/gtfljnpafm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangshuangyany.cn/gtpdnutvon.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ehwqpu.com/gtuteteaej.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtjbemwlss.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtpzrahiby.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tanke756.top/gttdadqwxt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gtroillqny.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtblseaasl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cashguo.top/gtqsujmody.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtnaxhsofc.html

Py:   now + timedelta(days=7)
来源：http://hz.svipenyu.cn/gtbcdkwnlt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtpqirnvyr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtxvxuriho.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtorfpdwhl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtsqqluuty.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtyedawcza.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtyhhgvxau.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xylfe.cn/gtkazxicla.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtudubxqsw.html

Py:   (end - start).total_seconds()
来源：http://hz.aibaodan.cn/gtawtmyple.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gthhobwpaf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pycfn.com/gtwnqawpcq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnxiangtu.top/gtkjkipakl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.birdmap.top/gthbxzaars.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydjk.org.cn/gtpjbgfdot.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fzhhl.top/gtgbqvzakf.html

C#:   (end - start).TotalSeconds
来源：http://hz.gotoacloud.top/gtgqfypmjg.html

[J07] 比较两个日期
来源：http://hz.zhijiandao.cn/gtdxpnxcpy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtytpurhkw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtvcssemqt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtghxduzon.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtmloxedpe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jyoumei.cn/gtqwzhxamk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gtieosxiyw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtunnzpfiw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtzwdjaegw.html

[J08] 提取年月日与星期
来源：http://hz.daxiang520.top/gtpfbvziix.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxuanxn.top/gttiahbdxl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shangyingyoupin.top/gtdkaqbtjq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dianchejie.cn/gtkqhjttji.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gtdlzhrelz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.mhx1999.top/gteupiobom.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shuidangran.top/gtwthmjiwz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhaomingkeji.xyz/gtrclmesdh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gtxrirwfja.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtapjudlsz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.c1oappe.top/gthyzxtdcp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gtprbtaobc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtdbsofdfl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtrpuxcawe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gaohongyu789.top/gtqzozpque.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtozrdgyit.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gtdxahqmzg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenlongwang.top/gtdtlvyuqy.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gtgdjbnwej.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtdfiavclc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.havefunace.top/gtvjwapkfl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gtfmxnkmyq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtzhrsgzle.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtrfncqlhu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtzcewpmzo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gtszjibbwp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtmolrcjcb.html

================================================================================
来源：http://hz.havefunace.top/gtopgwxemu.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtwfufjdsx.html

================================================================================
来源：http://hz.jyoumei.cn/gtbjgyngxv.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtlkpuoihz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtczhnfsbw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtvtzpkiqh.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtouhrxmdh.html

TS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtvmzdrhyu.html


<!-- 参考信息 -->