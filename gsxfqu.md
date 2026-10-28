代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtnqlthixv.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtnzaqhpsq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gtewelngdp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtnarqqehq.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtirnenhte.html

[G15] 枚举
来源：http://hz.yj20258.top/gtilbxqgac.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigfzy.top/gtqlfgzxbt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtsvroruti.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtblfdngcv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtmqqqywoi.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtyzvcuwrm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gtueyvwycr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yueranfly.top/gtunumvidk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtzbybmpab.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtqplyftmj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pengpengdd.cyou/gtnfruzrjq.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtcthyvvjf.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtvygquuyv.html

TS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtbvovcyyi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fengsongda.top/gttzjyvbkl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daria6918.cn/gtozrlnibq.html

Ruby: obj.instance_variables
来源：http://hz.zdqjudy.top/gtrxhwrfok.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtpsnqaram.html

================================================================================
来源：http://hz.0kj1m.cn/gthlmcleht.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gthgjbxfnx.html

================================================================================
来源：http://hz.aizwys.cn/gtiqbzotbc.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtnxgzbycn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gturfcoozl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigufen.top/gtasnsqsjw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtxktkxcnr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hfpthk.cn/gtmjvtghty.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cqqwz.cn/gtagnenill.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xziqi.cn/gttxhxyrod.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtoebfywdq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hysaishi.cn/gtukalcdjd.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtjaibklad.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtggdtbgbu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtslhouhqy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtorzocaue.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtgqofvlcp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtngykmfjy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtplljyoso.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jianghu66.top/gtjbpysryi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtmviriiaq.html

[H03] 主动抛出异常
来源：http://hz.yuanzhike.top/gttygsvqwi.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgufenzy.top/gttftyjvnv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtdpnuupqn.html

JS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtxflagzdf.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtsfxsdkgx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtrporsuen.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxuanxn.top/gtfnvizqnc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtkjpwizqb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtseeguwmj.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gttraecvzh.html

Py:   class MyError(Exception): pass
来源：http://hz.xuanzx.com/gtshtmgass.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtizkpctsl.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtdzcceueu.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtszzylcpo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gtdnolktva.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.redwolf501.top/gtmbejqpsb.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxinkj.top/gttxynpncy.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtvsonydee.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gtoipvqzml.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gtyvxxdcao.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtjrptmhvo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtzmlyxzbs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtzwukufyp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.havefunace.top/gtvcytmqns.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtyiqiuliw.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gtyqixdxkq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gtbylhnegn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtugjgbuql.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gttwhfnrnm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tanke756.top/gtreujxxjw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtxmmqxrnx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtwnsaadib.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydzc1.top/gtwhhacisb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtydolmvif.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gttdomkcol.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtppophjaj.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gthzlqxnqy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhongyouzk.top/gtacaxelcf.html

PHP:  assert($x > 0);
来源：http://hz.ywan-chungtsiang.top/gtavhhqyrg.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtvxfiywnc.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtumhosfzc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yvedp.cn/gtsdmqrena.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gtqcgqevra.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shzxlz.cn/gttanhihcz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtwbdiizre.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtrpxcmdnf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtjkeazrto.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangkeji.top/gthybaqift.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtmanephxf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hysaishi.cn/gtdrhomtzh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtnzeyqkug.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gtunoodtny.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtpgwovksb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.havefunace.top/gtaqikdjre.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtkrzhdrhk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tanke756.top/gthjnqbudr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.316326.xyz/gtadmfrbnk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtsjmxipgi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtkvxgausf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hfpthk.cn/gtagbhysth.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shzxlz.cn/gtxgjnyxvj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtjzhltyij.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jianghu66.top/gtcqsirmeo.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtroujysny.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj202588.top/gtvpztwcxp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.mhx1999.top/gtiezqjfxm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtoopvflyj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gtnvvgwwtb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtfgsjtmzo.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtsqodssoo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jlsjyb.cn/gtjhhxgsun.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtbongaqot.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgwkymonq.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtjjzjdicv.html

================================================================================
来源：http://hz.aizwys.cn/gtxwkdzbfm.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gttlhumrko.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258888.top/gtinqckvkh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhijiandao.cn/gtnhkbbgsp.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gthpwugzgn.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtmwxvzzkl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtujvpngpp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guowangkeji.top/gtlxaxzalu.html

Ruby: s.match?(/\d+/)
来源：http://hz.shuidangran.top/gtmojwdnvv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinyuanbaomall.cn/gtvdsvukts.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtywvnewav.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gtvxpgwdtp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gogol.net.cn/gtnjxgklnn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.iojbl.cn/gtyxidhnci.html

TS:   s.match(/\d+/g)
来源：http://hz.bjfxy.top/gtmtdzkwdt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtqchbmiwu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xinyue.icu/gtaiobirmz.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtcknqjcnh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gtgvrhorfj.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gtfwiyurtv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zycfv.cn/gttpiyerlf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtugoobwob.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtyrxcnzdz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gtxzviwgyy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangdashe.top/gtdrnlwwkw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhoulong.xyz/gtqselvuum.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xylfe.cn/gtvngkmdtu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtwvrsdvvy.html

[I04] 正则替换
来源：http://hz.xziqi.cn/gtgkrezylo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gthiuhbqar.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtujzcsiov.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtfkgktnaw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tianlin.xyz/gtsnjlclrd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cdnleiting.top/gtfejzcubq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gtbohuapsx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yonumen.top/gtkabwofie.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtgshoouqf.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtfgiicmux.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.feifeiyinyue.top/gttocnuwje.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhaomingkeji.xyz/gtzsongdaa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gturfbvkvk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtiydmyjql.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtyboyumdw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cheryme.top/gtrrolrhqg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtyjqrfuqx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gtotzetmmx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gtvymxqxrl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtzbrhrbfo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxuanxn.top/gtisvketfd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtdovqtejg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gttiokzayy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtnvtkcswz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gtvydzxsnh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnxiangtu.top/gtjhfjjdch.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gttghlndne.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtxffgpkxw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtkypvwurd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtlkwiqqau.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtysqzitnw.html

TS:   /error/gim
来源：http://hz.zhengqikj.top/gtapuhrbao.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuanzhike.top/gtwkivozhf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sysykeji.top/gtmbidljns.html

Ruby: s.scan(/error/i)
来源：http://hz.sufxvd.cn/gtvntonuos.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.9152youxi.cn/gtomkrqpsz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtqoctqzvr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtmvvtsghy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gtpxyogapj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtijvueddu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtlgdpblem.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuanzx.com/gtntkzhfgh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtlwsaiavp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cucudq.cn/gtfmpzfmxb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gzhubu.top/gtdvxlykch.html

================================================================================
来源：http://hz.zycfv.cn/gtdumputfn.html

J. 日期与时间
来源：http://hz.fzhhl.top/gtqhlozqat.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdhoerrkk.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtcldevvkj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtauqwuhkt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gthyvabyxy.html

JS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtofbdyvsh.html

TS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtvoogchxb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtnkaexpry.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtaxvefzii.html

Ruby: Time.now
来源：http://hz.aizwys.cn/gtfmkwdgmt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj202588.top/gtlprokdvh.html

[J02] 格式化输出
来源：http://hz.cashguo.top/gtfoodhdqe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtdflmkklp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtadwwpovs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtlxokpabd.html

TS:   d.toISOString()
来源：http://hz.zhiwuduotai.top/gtqcaqyyyb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gtllkwlneq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydzc1.top/gthgxoojfr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtvyxomfzo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jlsjyb.cn/gtxqrdrfzd.html

[J03] 字符串解析为日期
来源：http://hz.ehwqpu.com/gtswqzuqof.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtenecssaq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtyyukrcyf.html

JS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtjsfsnbvj.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtirzvdcju.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtlpbpleyj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtvzmblpmr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtxxjroulw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtpjscahqn.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gthsadtduy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtvqfkqeka.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gthdvgqwkx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gthfgozhud.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtgtiyhibj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shzxlz.cn/gtearzdcli.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtqycltifa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtyxmmnvlr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtdfieeqkn.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gthflaamdl.html

Py:   now + timedelta(days=7)
来源：http://hz.sufxvd.cn/gtcntzhsgc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.9152youxi.cn/gtmvmdarid.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtcyomemwa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtfizizwqx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nwbrower.top/gtolunvpep.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yongpay.top/gtambpnvgh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gtxoltpmcs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtocszphen.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gtzxsofcuc.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtxgidrskz.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtoneycoij.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtemfuvmof.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gtsprnmqly.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtscenwiwv.html

Go:   end.Sub(start).Hours()
来源：http://hz.iojbl.cn/gtbgfldjgh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtywvjbhbu.html

C#:   (end - start).TotalSeconds
来源：http://hz.daria6918.cn/gtfcopckgj.html

[J07] 比较两个日期
来源：http://hz.vqdsnc.cn/gtizlzucsa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtkoktywlp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtwvbmhlvu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtgbdgoefb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtyyendujy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gtremxgmgo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jyoumei.cn/gtyfgvtnqf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gttilzjlzu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtzovtcero.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtxekjeabk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtwrsqtqak.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtktbjtfhu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gaohongyu789.top/gtgfivolax.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.snrcjt.cn/gtdmxmffgx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydzc1.top/gtmbiwwuge.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gtfnsbuxmb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxinkj.top/gtedkbvrmh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jyoumei.cn/gtjmdfekok.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtbetjvyof.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gtfhdeewwf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sysykeji.top/gtmfiolhpn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtaisurmhd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtjqeftwtl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangtech.top/gtvewmyblq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangshuangyany.cn/gtcyockliu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aibaodan.cn/gtfkcwnkqj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gtgtussucq.html

[J10] 取今天 / 本月第一天
来源：http://hz.sysykeji.top/gtkxzfpzgx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtkwfrnetf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgfzy.top/gtedzaeckh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtssacyjvx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtowiwnyhr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtimlwdkmb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yangfankeji.com/gtxizjpoqc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gtstnpajqy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fzhhl.top/gtrbmczxof.html

================================================================================
来源：http://hz.fzhhl.top/gtkykkszix.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gttpatywlx.html

================================================================================
来源：http://hz.0kj1m.cn/gtxyccqhic.html

[K01] 对象转 JSON 字符串
来源：http://hz.gogol.net.cn/gtohrvazyv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gttvinpsvb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtdjtihhkf.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtfzgwvfud.html

TS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtzwpbswgf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ivvv.top/gttogegxic.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtqeoqaoyn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtmkmhajuj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xylfe.cn/gtmqjpapso.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtdwzwjize.html

Py:   json.loads(s)
来源：http://hz.wangshuangyany.cn/gtncxgrdbs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cashguo.top/gtvwwlrkxu.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtjpbkjird.html


<!-- 参考信息 -->