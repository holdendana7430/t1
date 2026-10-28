代发 wailian999

Java: u instanceof User
来源：http://hz.aizwys.cn/gtwetayrcz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ywan-chungtsiang.top/gtkpasercg.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gtdddbywhx.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtyuvsmhat.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtfuhgsybq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.9152youxi.cn/gtrstcyvmj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cheryme.top/gtaicpmzpr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtpvhroaux.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtdwnbnfgf.html

Java: record User(String name, int age) {}
来源：http://hz.jianghu66.top/gtyhwhbetj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtqknzcqbe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtndauropk.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtntqlirvf.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtjpojvhfp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtubnaqtif.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtphdkqvse.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtuoyzbvve.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtxztlvloe.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtbqskbjcb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gthlbfngkq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aizwys.cn/gtsooglcjk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtmqewahaw.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtcirntcxk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.c1oappe.top/gtuxfjiqcr.html

PHP:  get_object_vars($obj);
来源：http://hz.zhongyouzk.top/gtkamtbucf.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtkwttqunc.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtyxlbnctj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtzubyxpcl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ehwqpu.com/gtxnvmniwi.html

Ruby: obj.instance_variables
来源：http://hz.nwbrower.top/gtcgzemjiz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtladcxkfd.html

================================================================================
来源：http://hz.iojbl.cn/gtheodeqfs.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtexjjclah.html

================================================================================
来源：http://hz.gogol.net.cn/gtxttelzrq.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtxevbjpqz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jianghu66.top/gtorztyaiq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtqmialcoi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtrfjjvhqk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gtxpgoanai.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtuqjorbeb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtjhzvtyds.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtlmxpjowi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yueranfly.top/gtlgwyqnvn.html

[H02] finally / ensure 收尾
来源：http://hz.daxiang520.top/gtulnrtknm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtwdksmhjn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtfebueldx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtqyjipacq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtcflhkono.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtgminxiks.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gzhubu.top/gttvqtkybu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gttyuskxcj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtnquflhzn.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gteehybjfn.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gtlgwncynu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtlarveruq.html

JS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtvdsxtpms.html

TS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtxxiqkzzu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtjaxqkjjt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtlrzqcyfl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtqaoirmhq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtsaundxmg.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtufqdhhxt.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtypyrjhhp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtoxtievrd.html

JS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtcxtaogny.html

TS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtpbjnjkzx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtlobajemz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xziqi.cn/gtdatshsna.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gtqbvkxeta.html

C#:   class MyException : Exception {}
来源：http://hz.meibo888.top/gtfpsqyclh.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtyddqvmta.html

Py:   except ValueError as e:
来源：http://hz.zhiwuduotai.top/gtkaamblpc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sweek.top/gtuxpguxdy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtvpzwwzdk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtlbnxvggg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtvnevvzrz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtueabpejk.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gtluatfxix.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtykdydnlp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gttrfzcvgt.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gttonqkvwz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dianchejie.cn/gtcasbtawu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtnmrotbsf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtrfhekyhw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.52xcode.cn/gtrofofeyc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cashguo.top/gtumtdjxoh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtxlzqkdnk.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gtdkdeadob.html

[H07] 断言
来源：http://hz.yanxiufei.cn/gtablslott.html

Py:   assert x > 0, "必须为正"
来源：http://hz.mhx1999.top/gtpfxhbyqi.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtpoyezxyz.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gthdlctbdo.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtewyiadmj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtqwalvjrl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhongyouzk.top/gtkkiruuca.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.iojbl.cn/gtthfyxqlb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gzhubu.top/gtwynjknwu.html

[H08] 获取错误信息与堆栈
来源：http://hz.havefunace.top/gthhtyuiyb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ehwqpu.com/gtwbyfhdax.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangshuangyany.cn/gtebmhpegq.html

JS:   e.message;  e.stack
来源：http://hz.xylfe.cn/gteulnkpoy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtpqpemlbd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.havefunace.top/gtduvapwjh.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtmdbxgjzy.html

Ruby: e.message;  e.backtrace
来源：http://hz.gaohongyu789.top/gtbphiqybq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtireoyqmp.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtuectgmhl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gttlcrqffu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenjidiqi.icu/gtcemwfrwc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtztoagsaa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtjxtabbri.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gtbmsfvsiz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtjzqmwbpd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gtzorheuhi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtwsmtvmgq.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtuuqageix.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtbqgkczvs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gotoacloud.top/gttgusoicb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtpvqyuakj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtzgnrudpq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.c1oappe.top/gtmljrkfkl.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtkegabuuq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtnnyuxbvm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtafaorjsz.html

================================================================================
来源：http://hz.yj20258888.top/gtvuifjblx.html

I. 正则表达式
来源：http://hz.birdmap.top/gtmurgvkyy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtstcnpkvl.html

[I01] 判断是否匹配
来源：http://hz.xziqi.cn/gtyhnsiztj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtpweyrvuw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenlongwang.top/gtvaqwlkjq.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtincdjggg.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtynntdths.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtuseaqjby.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhixingplan.top/gtgjtgbbuw.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtavelltdi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtbgdckasq.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtdbrefiaj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cheryme.top/gtnkgnsrzo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtcdbdydhk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtrshawpql.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtfdbcupeq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gtdckyeqvj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gogol.net.cn/gtxhfimxrt.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gtvolhwwsv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtexnukgrb.html

[I03] 提取捕获分组
来源：http://hz.bjfxy.top/gtmbjlxtug.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtwmltbvvr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtptzqqxkz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.svipenyu.cn/gtwwsnfenw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pycfn.com/gtdkjguktr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sxryk.cn/gtiuchnylu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zycfv.cn/gtawkawivt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fengsongda.top/gttdgxggkz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yonumen.top/gtachxurgx.html

[I04] 正则替换
来源：http://hz.tian-w.cn/gtobtqtrsk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.316326.xyz/gtwhbbtqrs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtstcrsgjp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtozsvnbup.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtrfwdivgg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtyhlyfmwh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtykkepyiz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtehgzcbfy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.redwolf501.top/gtxnixnqww.html

[I05] 按正则拆分
来源：http://hz.guowangkeji.top/gtlqmvvwlw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gthpzfxskx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.c1oappe.top/gtfdjihbej.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtizwwwjpn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtbccrxdli.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ybcxt.top/gtuhcmtmmn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtxwnhenhk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtuexhkgjp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgfzy.top/gtwblbxypy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtmgwdbaey.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtmitejoej.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtvqpmsogw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtxunqykyp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtwojepnct.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuxming.cn/gtjzbglods.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nwbrower.top/gtbpxrfsuj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.bjfxy.top/gtqvptwtoe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtnzowedhd.html

[I07] 忽略大小写与多行模式
来源：http://hz.meibo888.top/gtbpjedrly.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.316326.xyz/gtczembrbh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aibaodan.cn/gtwmjrltiq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guowangkeji.top/gtvwurjxoi.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtyzcqanuh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigfzy.top/gtlmqlyoqc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangtech.top/gtkshsrcse.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtmeovxpat.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtzvrajnlr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gthxzxydbk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sxryk.cn/gthrkxpysj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtrxvqkzny.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtorzullml.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gthecybwgm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtjeebtltv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sweek.top/gtnwrexbqy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guannengcc.top/gtyyyhgoiw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gtzohvnqfz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtihtwwxpe.html

J. 日期与时间
来源：http://hz.yuxming.cn/gtjdnvbcpe.html

================================================================================
来源：http://hz.wangdashe.top/gtywbodbfm.html

[J01] 获取当前时间
来源：http://hz.ybcxt.top/gtxfsfdwct.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtiorazizg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtokldlfcj.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtzaqltsjj.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtejzsnlum.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gtiylppkqw.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtjgslxuqd.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtiwpkakvd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ivvv.top/gtkeumnakz.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtmhsqjwav.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtnghtnmad.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtbumblfsy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.0kj1m.cn/gtmenxkzhb.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtyflvqxxr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jianghu66.top/gtxfvvoedv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtxtcfmxdn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtbomthucq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gtnkkhaykg.html

[J03] 字符串解析为日期
来源：http://hz.cdnleiting.top/gtxydgtsxq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenzaomai.com/gtdnehfadz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtywrdhqph.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtsxbqyuyk.html

TS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtidgotumc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtgtwfxdmh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtdpwziifq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ivvv.top/gtanoqmqza.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zycfv.cn/gtnrisdotp.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtjorrbcfw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.guowangkeji.top/gtybudnfce.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtbkwuqkbm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.9152youxi.cn/gtcjdiqtad.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtvgurhnad.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gaohongyu789.top/gtjlpgmzwr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtnfrdtgnn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhaomingkeji.xyz/gtswbfxswl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.haohaochexian.top/gtcywjbjii.html

[J05] 时间加减（加 7 天）
来源：http://hz.gaohongyu789.top/gthngdrvon.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtccovosnt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gttagopzcx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtjclmmrda.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtheadnqll.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtwccgdcqh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fengsongda.top/gtcegjgbkz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtgdgkzqkv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gttotmjeek.html

[J06] 计算两时间之差
来源：http://hz.tianlin.xyz/gtoeodordx.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gthsgckqbi.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtqioljerx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnqzz.top/gttbfiduxf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tianlin.xyz/gthzwqovgb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.svipenyu.cn/gtylhaowyk.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhijiandao.cn/gteawzllta.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtqotbglxj.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtlcvnsmoz.html

[J07] 比较两个日期
来源：http://hz.zhongyouzk.top/gtiktzdviq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtgtdenlbe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.bjfxy.top/gtxlhnmzia.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtoajtymrl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtifffduna.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtccfeaxyj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenjidiqi.icu/gtvuhyjjsw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtufkvrpei.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtpwcueqta.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtxmsbvnra.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtybhlweum.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtifnyttfl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gtpvazbsdf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtjqfwwlhe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtdbqcvyrj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tianlin.xyz/gtitckctey.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtaimhecxr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtqyjoldip.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gtpanidcby.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gtkbxoscmx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtyqinleyj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtsgivcgzo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gttiwyzvbf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.andypj.xyz/gtetjpxpfp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtxtbtkrsd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtyswxidss.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtygjywoen.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtwxglicoq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtnshmuaab.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gzhubu.top/gtoplisbad.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.haohaochexian.top/gtzydtlmiq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jyoumei.cn/gtjxoltbvh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtbtafoogn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtstrbfzhe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangkeji.top/gtlydrcaba.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtiubakvxf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttwidiijc.html

K. JSON 与序列化
来源：http://hz.xziqi.cn/gtmccacxao.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqxbkhfdr.html

[K01] 对象转 JSON 字符串
来源：http://hz.sufxvd.cn/gtaqwznsnh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtokrnirvg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.vqdsnc.cn/gtyjxozhyn.html

JS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtrurynnry.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtwbnntjab.html


<!-- 参考信息 -->