代发 wailian999

[G14] 数据类 / record
来源：http://hz.aibaodan.cn/gthpefmtgg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtxmrlftlk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gogol.net.cn/gtmjbapntv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jianghu66.top/gteghsbqkv.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtevksqhdf.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtnvdvtaig.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtrqlievdo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtwrhilgej.html

C#:   record User(string Name, int Age);
来源：http://hz.hywenlv.cn/gtlbvzbdyl.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtaoyqcoqz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtjiuodkeh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tian-w.cn/gtybkswjrm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtsyvcxyol.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtcnqpxzhd.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtvzlwnklp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.meibo888.top/gtsxtofzys.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtvaxefmls.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtxjpjboue.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtervffojj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zdqjudy.top/gtbroilxhf.html

PHP:  get_object_vars($obj);
来源：http://hz.zdqjudy.top/gtojzigimj.html

JS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtomojscue.html

TS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtckbnlljd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jlsjyb.cn/gtbbqpyglb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gtcuhsnxzo.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtycvzhsaj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jyoumei.cn/gtowrqzavq.html

================================================================================
来源：http://hz.hammf.cn/gtmqexkjrq.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtfqdppekh.html

================================================================================
来源：http://hz.tanke756.top/gtsfejwuyk.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtvjwzwsbi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenjidiqi.icu/gtgenzncde.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtfxtpeuvf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtupxgiutp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hammf.cn/gtecsdlmqt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gtrxnfyskq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pycfn.com/gtumxiumot.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.iojbl.cn/gthxqzagnt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yongpay.top/gtncawuwkt.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtsazbfowi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtbqxkmgtp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gttrfhghlw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtfdvkxlpx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtffkrwwyu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtvkhfwrbv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtuqvvlvje.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yongpay.top/gtfdqjkbps.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangdashe.top/gthpznnxih.html

[H03] 主动抛出异常
来源：http://hz.zhoulong.xyz/gtiqqploor.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtfimhjeaq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtotdxttun.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtlsfwjpls.html

TS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gthwdjxkbu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtbzorowek.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gthuxgwjcy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gtyvurazcf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtbpcksxno.html

[H04] 自定义异常类型
来源：http://hz.sxryk.cn/gtczsqapag.html

Py:   class MyError(Exception): pass
来源：http://hz.shangyingyoupin.top/gtpcxukvss.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtnntpalta.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gttksyturx.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gteestmgex.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gtovjlxcsr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sweek.top/gtbfizjmqq.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj202588.top/gthtktrkfu.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtiasduhkg.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtgyysdclk.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtaylhwvqp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.c1oappe.top/gtxrdftmnp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtlhwvgvxg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtodvxewlf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gtxfgxzqwd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.0kj1m.cn/gtqfemqhqt.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtlwzeqhny.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hfpthk.cn/gtbocxdalg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ivvv.top/gtnenyntws.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gttigzrryv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj202588.top/gtvfwvjipt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtaxpxkxsq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtymrangxe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gttxepgkwo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtehvwioye.html

Ruby: d&.dig(:a, :b)
来源：http://hz.redwolf501.top/gtkgacoquu.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhijiandao.cn/gtxqxallqc.html

[H07] 断言
来源：http://hz.gzhubu.top/gtuhdhjnhr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gtmkdnpncl.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtxukhslkc.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtecpwkqst.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtoaporkxi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jyoumei.cn/gtixfxvrxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuanzhike.top/gtolcjfcrz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtpmkrtnza.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gtthrhjwbf.html

[H08] 获取错误信息与堆栈
来源：http://hz.iojbl.cn/gtelfhguov.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtvdqzbhxk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtpejtfjff.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gtwwamfssu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.snrcjt.cn/gtoqptvsut.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gtgmyptvhh.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtlcztkvck.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gtfoaytaaz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtkqoycufw.html

[H09] 带错误码的异常
来源：http://hz.yj20258888.top/gtzagmoppe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ivvv.top/gtjjryyuyq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gthlynyigf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hammf.cn/gtznrhzhjk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jyoumei.cn/gtfrahdguy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gtjuebnbpr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtqgxokyry.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtjfmocxcl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuanzx.com/gtxegprhzo.html

[H10] 资源自动释放
来源：http://hz.yj202588.top/gtkhyujwnh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtqkygsvrq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pycfn.com/gttnloaaqr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtrptbhaey.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtzaejugfb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.smart0.xyz/gtijmqtcze.html

Go:   defer f.Close()
来源：http://hz.snrcjt.cn/gtcyjudxwe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zycfv.cn/gtxgcawhtc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxinkj.top/gtzqenvsaf.html

================================================================================
来源：http://hz.nwbrower.top/gteufqiwfw.html

I. 正则表达式
来源：http://hz.zhengqikj.top/gtitbphcie.html

================================================================================
来源：http://hz.zhixingplan.top/gtxjzzjnuu.html

[I01] 判断是否匹配
来源：http://hz.aizwys.cn/gtpeqrbhwl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtpylmisoj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cashguo.top/gtaaeyakdl.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtmcxusdht.html

TS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtdcjulygm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gttuoperlq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgfzy.top/gtqothqwnx.html

Ruby: s.match?(/\d+/)
来源：http://hz.tanke756.top/gtfslalmou.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtcmiqexvz.html

[I02] 提取所有匹配
来源：http://hz.dashuyun.cn/gtdoqzsyay.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gttqupjeyv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daria6918.cn/gtywbtdrfz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gtnjbqnlbs.html

TS:   s.match(/\d+/g)
来源：http://hz.jiagoushi.top/gtkhoeiote.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuetiantiany.cn/gtbjugfumh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtpelfyiee.html

Ruby: s.scan(/\d+/)
来源：http://hz.yueranfly.top/gtufwigdmo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gtrtckhmhu.html

[I03] 提取捕获分组
来源：http://hz.cdnleiting.top/gtiaueenhn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgfzy.top/gtxukjrqpl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenzaomai.com/gteqwbdfko.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.c1oappe.top/gtcmndtmkp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtxbtlarre.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtfnxfoeie.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aibaodan.cn/gtfhrjpzfq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtmbjzrvea.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gtpsvdetjp.html

[I04] 正则替换
来源：http://hz.gaohongyu789.top/gtbnipeajo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtodfnpzbo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtebmsqkcp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gthodezoqq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtnpfavhif.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnxiangtu.top/gtdvbhefsz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtujxybcrp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fzhhl.top/gtxlzarvqf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtydnzsapm.html

[I05] 按正则拆分
来源：http://hz.nanxuanxn.top/gtllnrjpvg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.haohaochexian.top/gtqueorjnt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxuanxn.top/gttqzhdgvq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtqrriztgj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtbbffcguk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtwwuwlxew.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtunqrwddw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtffdrkfuk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fzhhl.top/gtxuxnglwx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydjk.org.cn/gtyfpyqzrn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtgesqekow.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hfpthk.cn/gtqhgrbvgn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtnspudqpk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtdilfpwyq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hywenlv.cn/gtkvtzcoaj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gthzwtngls.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuanzhike.top/gtvgosolge.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtervykgyb.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtmyekbvjw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.kuanghao11.cn/gtsseohglx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gtnqydnoyk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sweek.top/gtzjxaltkv.html

TS:   /error/gim
来源：http://hz.sxryk.cn/gtziqhocgj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtrvxqowma.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtkjjsaomw.html

Ruby: s.scan(/error/i)
来源：http://hz.tianlin.xyz/gtiewavmlp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxinkj.top/gtxhcjdlag.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aibaodan.cn/gtralzqnre.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gotoacloud.top/gtkqbiasaw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gtxylyevgy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtfzokmvie.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtwclruarb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtqvnfbuzs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pycfn.com/gthqwcvmov.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtphfhoxiu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtfppeytxn.html

================================================================================
来源：http://hz.9152youxi.cn/gtkoxaqcbx.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtstkgqkbu.html

================================================================================
来源：http://hz.hammf.cn/gteawhjexl.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtuggamwvz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sufxvd.cn/gtvpiawdpe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtmqtkadob.html

JS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtctaolhcg.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtkopspkys.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtnucuahsq.html

Go:   time.Now()
来源：http://hz.nanxinkj.top/gthujwexdq.html

Ruby: Time.now
来源：http://hz.cucudq.cn/gtufemesgb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dianchejie.cn/gtpxdsrkdh.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtdoztiyen.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gthafzjifm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtgsfbrsys.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sufxvd.cn/gtloghltnj.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gthgavzlzv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtdtompvlc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daxiang520.top/gtnolqrsqd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtnwsqebzr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtcjlsqfel.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtgmvlhjmr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.c1oappe.top/gtrwtssbjd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtvenaumli.html

JS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtmhrtubze.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtzbhfcsbc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtcqaafsgc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtihtcanid.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtgbcgpsch.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtdeclgjho.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtlxlnxdav.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtocvhybvq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtlsrsqhah.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.andypj.xyz/gttkzhaeqv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenjidiqi.icu/gtvkemduth.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gtngmdxknj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.mhx1999.top/gtflsiuudk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtrkzopsul.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shzxlz.cn/gtprqakcox.html

[J05] 时间加减（加 7 天）
来源：http://hz.xuetiantiany.cn/gtcsyacuhx.html

Py:   now + timedelta(days=7)
来源：http://hz.zhixingplan.top/gtuemjwpvp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtnlrbpxvz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtdiltligp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtkuvqsefu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydjk.org.cn/gtuxcdxweq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtbbtenjkw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gthtmrckpy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtgewojmyf.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtndifnsio.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtvnieewhr.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtkjespiqp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sweek.top/gtlfddglco.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangtech.top/gtyeslnwym.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258.top/gtsdkwoajo.html

Go:   end.Sub(start).Hours()
来源：http://hz.daria6918.cn/gthkbwyjul.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tanke756.top/gtrtplsdqk.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gtlolvlfrr.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtpknutgcz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtzrdzgekp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cheryme.top/gtwuyrlepb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtdrlpehrx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtflukrhnr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtfndolewy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtotghceil.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtownzqeej.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtrnanicwm.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtvrxosfky.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cheryme.top/gtpunsioyc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cqqwz.cn/gttcfotaib.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ywan-chungtsiang.top/gtwnbhqtpu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtaqixvaea.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gthyjzhsax.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.svipenyu.cn/gtszigxalx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sysykeji.top/gtnmistmsl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtxhqcltyj.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtrzzgzebj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtmgaoqope.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.svipenyu.cn/gtdqrcjtgy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtczhyhnug.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtygueawia.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gthptidawd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtlkxefuwp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtoryemnxn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtkqjgvhip.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtvwhrmkpq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ppjwa.cn/gtacfvuwsn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtnzeexjjf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shzxlz.cn/gttvugwbrw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinyuanbaomall.cn/gtdaicdwas.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jiagoushi.top/gtsdbqnnqu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtzomlxqcz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gtujckcrnk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zycfv.cn/gtywguabjv.html

================================================================================
来源：http://hz.sweek.top/gtqdqfuqbh.html

K. JSON 与序列化
来源：http://hz.yj202588.top/gtjnskodvd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnuafllhe.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtcpfwigiq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtadbccixf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtheomezxb.html

JS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtidljxsvo.html

TS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtnajzvbez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gtnamlpajr.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtrwwaiksa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtetdrpfgu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtwbgsgmnn.html


<!-- 参考信息 -->