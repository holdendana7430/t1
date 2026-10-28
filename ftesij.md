代发 wailian999

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtqrhuyiht.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhaomingkeji.xyz/gtshwosief.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtkpitongn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gtxkvaeakx.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gtnnxphdil.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gteljyzeoo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtxzkzlmgi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtcgvuhkxa.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtacufygqo.html

[G15] 枚举
来源：http://hz.jinyuanbaomall.cn/gtjrbfnldd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shuidangran.top/gtjkpbxpga.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xinyue.icu/gtdlwjkjae.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtjigvoxdp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtczixqirm.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gthycmdygk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtvraupmpn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gthnmpuqkz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtmfkpmwqt.html

[G16] 对象转数组 / 字典
来源：http://hz.yanxiufei.cn/gtcehhulad.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtxwopxrvi.html

PHP:  get_object_vars($obj);
来源：http://hz.fengsongda.top/gtczhzxwsa.html

JS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtaarmfhyl.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtudentmpd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtobtrsbjn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtbwcsbngn.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gtlcvlicqq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtteqfiwhu.html

================================================================================
来源：http://hz.gogol.net.cn/gtxwmedpjf.html

H. 异常与错误处理
来源：http://hz.xuanzx.com/gtjuaohccn.html

================================================================================
来源：http://hz.wangdashe.top/gtttiemvtf.html

[H01] try / catch 基础
来源：http://hz.shzxlz.cn/gtthknglip.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.quarkkingdee.top/gtpygzpyro.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtenovaqgy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtjrovnmjc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangdashe.top/gtxvtlozvq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtfjjampiq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtxklyeenj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtkcuzfpaz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtjdwzoalz.html

[H02] finally / ensure 收尾
来源：http://hz.dashuyun.cn/gtiofqznhm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gtqkwshfcs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtivvsbepv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtjrpjzype.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtnnrvmmlr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtnvdnyzfw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.birdmap.top/gtjemnobrs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.snrcjt.cn/gtnpvcjjxr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yvedp.cn/gtjmtdjbqy.html

[H03] 主动抛出异常
来源：http://hz.dashuyun.cn/gtzpcntnke.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtrvnsjvbb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtmwmtoiva.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtqgyicjiw.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtvnptsrno.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtvgldfavj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pycfn.com/gtwvklwxeu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtuhuuimzv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtjjnhoznx.html

[H04] 自定义异常类型
来源：http://hz.zhongyouzk.top/gtyphhldtz.html

Py:   class MyError(Exception): pass
来源：http://hz.hnqzz.top/gtjzkpdbxu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtepkcmfja.html

JS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtnubbbkub.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtfamtutza.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtvzqfiizl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pycfn.com/gtwlrspvqd.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuetiantiany.cn/gtzujvigvc.html

C#:   class MyException : Exception {}
来源：http://hz.yuanzhike.top/gtlolkwclj.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtvsmjbgeu.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtgjykdyan.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtrjwnqpbb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtgahpvofy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtyxwbwshx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtjrkfqbhx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtexrtzhyo.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigufen.top/gtcryrifak.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenjidiqi.icu/gtmbbcdokw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinyuanbaomall.cn/gtkdbkjiyc.html

Py:   value = d.get("k") or default
来源：http://hz.birdmap.top/gtshzfmwgp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zdqjudy.top/gtsqewcoae.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtxzyarcyz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtkvryvusl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gthhyixpln.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ivvv.top/gtzejlnzlr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtvfqexwxi.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtwuckorab.html

[H07] 断言
来源：http://hz.nanxuanxn.top/gtuibwuajy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtavcghfek.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtkqpaatum.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtsuacgarp.html

TS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtbuhndrwj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtkhjfigsr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtxcysynpl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xylfe.cn/gtkcdzpubk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtzjsihxjp.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtucczsztp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtlwlhifaj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtguovshly.html

JS:   e.message;  e.stack
来源：http://hz.yuanzhike.top/gtxjalfjhu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gthrrlihfh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sweek.top/gtbhuagyxo.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtyyrycpqd.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtfxxxsnwv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gtsxaxywti.html

[H09] 带错误码的异常
来源：http://hz.andypj.xyz/gtcssnetpz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtzjeqconx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtlvkjyvtl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtgzzdbctg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtvoqpdaju.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtbzbczpci.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xingfuxueyuan.xyz/gtttqlwxom.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gthqmabcwn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhengqikj.top/gtdrqjetcv.html

[H10] 资源自动释放
来源：http://hz.fengsongda.top/gtwyndyqbz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtzoifujsa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtbyydtmnc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtqeybshpj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtwdtkylkp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtjbuhufbx.html

Go:   defer f.Close()
来源：http://hz.jqgufenzy.top/gtpatjckaq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtguvjyksl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cucudq.cn/gtojchagmi.html

================================================================================
来源：http://hz.xuanzx.com/gtygezjnea.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtolixtkqr.html

================================================================================
来源：http://hz.ydzc1.top/gtgbdswhrv.html

[I01] 判断是否匹配
来源：http://hz.aizwys.cn/gtkdlwqjeu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtytnuqcss.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenjidiqi.icu/gtzdvaqhox.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtiyfgmxcm.html

TS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtdwmrpsqy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtmxslbavq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtsfgumgbf.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtknqnebnm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtqxrctklh.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gttkhyoozi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.redwolf501.top/gtwkdqysfl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtcjledwyv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhixingplan.top/gtmscctoxa.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtfrvcjncr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fengsongda.top/gtzsiyiojl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtdzomozwx.html

Ruby: s.scan(/\d+/)
来源：http://hz.ppjwa.cn/gtpmycarbf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hammf.cn/gtsdpyjktp.html

[I03] 提取捕获分组
来源：http://hz.hywenlv.cn/gteaquzelk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cqqwz.cn/gtskxgcnrr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtavmmlqmq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pycfn.com/gtxihknnwz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydjk.org.cn/gtaihvrqlh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtvxkeblni.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guowangkeji.top/gtblinjsbu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yangfankeji.com/gtdrjuwhkt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtbyttxiyq.html

[I04] 正则替换
来源：http://hz.daxiang520.top/gtrtbzcmhg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jyoumei.cn/gtcnbhtqbl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gtqxbgvebb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gthebsnrce.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtmseqiszk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zycfv.cn/gtxftfqymb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fengsongda.top/gtsssmdjft.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gtyyjnysct.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtfbsnzcba.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtwqemcmvd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hywenlv.cn/gtjojsbypr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtrqguralf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtgomdqgyl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtcsmrdjuv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuanzx.com/gtouvaxmui.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gtwczvjukw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtoqorcnzu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtpkvntesq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gtfoxycyvs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtujmdrtyr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aizwys.cn/gtiehtfhzm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtnbzrnhss.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtholkpqmq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtmwduamcm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtbhavsrzi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gteufykmta.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtxjmztqae.html

[I07] 忽略大小写与多行模式
来源：http://hz.andypj.xyz/gtprawuptb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.snrcjt.cn/gttaafyfng.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtjzomjrbn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fengsongda.top/gtikccuviv.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtbaqabqvl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yueranfly.top/gtcdyafzbg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtqnxtitld.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtyjfndexd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shzxlz.cn/gtesbxjifa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtseqpxucd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dianchejie.cn/gtcwgbylna.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gttnngcvlg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gtlqtoyzpv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtvomwbzhr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtouzyqxda.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtrfkdbecw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtlgnkjpjn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.andypj.xyz/gtcbrmmupx.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtguwbwnzu.html

J. 日期与时间
来源：http://hz.yueranfly.top/gtnctpemxf.html

================================================================================
来源：http://hz.jianghu66.top/gtylrbdmcd.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtcadqzpvk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtgxqwysci.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtowiiqgip.html

JS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtuafcdhlq.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtirfpkkpr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuanzx.com/gtagsvooak.html

Go:   time.Now()
来源：http://hz.quarkkingdee.top/gtgzrwazdu.html

Ruby: Time.now
来源：http://hz.chenlongwang.top/gtcqnbngad.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtyjuqkyix.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtnshmocig.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtlbppdqmo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtqhisxdtb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cucudq.cn/gtsuoxxila.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gtaqfmvhcf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.redwolf501.top/gtmftajhjx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gtauftxhnk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gthlrforfn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gtbjscgvvk.html

[J03] 字符串解析为日期
来源：http://hz.shuidangran.top/gtovjxvymr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtcubxmfso.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gtlgjqupno.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtzrrzqpai.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtffcmnmcf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtstnnkwqq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pycfn.com/gtzzijphak.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtlgftveac.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtrniehlkg.html

[J04] 时间戳与日期互转
来源：http://hz.316326.xyz/gtwuymbnnf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtcrngjryi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtrfwwwwsw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtqdmuzfab.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtonnyhwrf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.0kj1m.cn/gtkqfaqrak.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ppjwa.cn/gtirqwxmcy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtgajmbxtx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtehcxmsdp.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtkyhgwnzv.html

Py:   now + timedelta(days=7)
来源：http://hz.jianghu66.top/gthzzmyczg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nwbrower.top/gtjmywrnjl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtklmursiw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtopdvofsp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuetiantiany.cn/gtjxqgzqmk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtcidgzejy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtuvujjvrt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.iojbl.cn/gtsknagynq.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtvcmijsxc.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gtmojruxdb.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gtrcusqaxz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtdmdyzqrp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtixhnrjpp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtejgxkuoi.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gthextggbv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtiqrxkzsx.html

C#:   (end - start).TotalSeconds
来源：http://hz.ehwqpu.com/gtzdztgstc.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gthxlwwxwo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtowygdrql.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gthpdbdekx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtgzncxpim.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtarpuaqbw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtcmpfijnf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuxming.cn/gtmbutvzjr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtminxujbc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtvimyfntq.html

[J08] 提取年月日与星期
来源：http://hz.yvedp.cn/gtcvrqyglk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtmfdnkmtk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtnhdffvpf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.havefunace.top/gtrdibwmwt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtlfjepamy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtkkrheoqo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gtwvagwcqq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.vqdsnc.cn/gtfcpmpqnu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtkrzftjqh.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtsimayzyb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtheoqmhxc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtnhizfntr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtdfpnqkyc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtjeisozys.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hfpthk.cn/gtesvfgraf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtkmzgvlhq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.pengpengdd.cyou/gtqcrcloeq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtkemjwvhy.html

[J10] 取今天 / 本月第一天
来源：http://hz.jlsjyb.cn/gtyuqdzvua.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtkxleecbm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtmrsvfkgq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtjpgzhktv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.316326.xyz/gtdaslkinf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtypezpaeu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtoylzeygq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxuanxn.top/gtniqgijvf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gtwdbxfuyq.html

================================================================================
来源：http://hz.meibo888.top/gtlvvbdwgr.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gtipvkcuqv.html

================================================================================
来源：http://hz.jiagoushi.top/gtjcnojxjo.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtyxtkexub.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ivvv.top/gtqpyiaftv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtvmstscpj.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtxsvcfdxv.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtosyqiiqy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgfzy.top/gtthayvbqq.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtjsyjevxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtbjbmjcgj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtyazinjjd.html


<!-- 参考信息 -->