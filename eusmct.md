代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gtkarfwhdg.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtosxldbfy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtjvsuodcw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gtyhpjxvxs.html

C#:   record User(string Name, int Age);
来源：http://hz.chenzaomai.com/gtneayrhzh.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtqrgbgetj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtbjpgxftn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtqoerrkca.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fengsongda.top/gtsucsdzcm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtthqqecdc.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxuanxn.top/gtyjtlxxim.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtiluoldkk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtcqyayqyo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtnirgiynd.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtocmygdlj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxinkj.top/gtwwyhyasr.html

PHP:  get_object_vars($obj);
来源：http://hz.c1oappe.top/gtveurpbsf.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtxzcybiku.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtlylbopsc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gtarbpdejq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtjjotpsjw.html

Ruby: obj.instance_variables
来源：http://hz.jqgfzy.top/gteofukacl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hysaishi.cn/gtczeislpx.html

================================================================================
来源：http://hz.aibaodan.cn/gtauolzoha.html

H. 异常与错误处理
来源：http://hz.meibo888.top/gtfesogxaq.html

================================================================================
来源：http://hz.haohaochexian.top/gtemkiblbs.html

[H01] try / catch 基础
来源：http://hz.xuetiantiany.cn/gtxxirztmj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gtwyyzqypk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dianchejie.cn/gtxajyjqjp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gteyucjemz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtaqenensi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtrgormsgg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aizwys.cn/gtpbberygl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtrovwdhfb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ivvv.top/gtcyjirynu.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gtnttmexge.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fzhhl.top/gtkwwzbnjn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtimukomac.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtlzljilli.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtddfaamev.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtlkxdqwhr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtefzdntgi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtbejhyffa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gtioowskae.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtpqdvwasv.html

Py:   raise ValueError("错误信息")
来源：http://hz.sweek.top/gtwjcvwezl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtwojaztuo.html

JS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtcrsfjuiv.html

TS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtmlrbdxna.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtdvhelpvz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gtebesfeqa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gtpjnyyrls.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtimdlrqlg.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtwxhxaavz.html

Py:   class MyError(Exception): pass
来源：http://hz.meibo888.top/gtgmvgyesd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtjagzbmsn.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtvkwglwhi.html

TS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtseommili.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtgovfghiz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtrgnbbvst.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangshuangyany.cn/gtdbkhkjoh.html

C#:   class MyException : Exception {}
来源：http://hz.zhaomingkeji.xyz/gtanputufi.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtqunihmol.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gthghmkynx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtkzweeoso.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtorqyydke.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtolvobnej.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinghuilouyu.cn/gtdexjzyvp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tanke756.top/gtticcsscx.html

Ruby: rescue ArgumentError => e
来源：http://hz.ppjwa.cn/gtcaxieiox.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gtsbxqgyoa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtdeibxaej.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtjcppxbni.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtvlskhtmx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtarknbkox.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtpkmtleme.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.andypj.xyz/gtatrcxfss.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtwmfgnlwl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daria6918.cn/gtlqaaesel.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtphtswcst.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtglahiijm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258888.top/gtvejawgrl.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtfpvrrbww.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtzehvtmhm.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtvndhcqdf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sxryk.cn/gthesparjg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gtjvqmxoah.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtmwhwvmsp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtpggrdeco.html

[H08] 获取错误信息与堆栈
来源：http://hz.yanxiufei.cn/gtwdtxjacw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.vqdsnc.cn/gtmsscihud.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.52xcode.cn/gtowhavrpj.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtzfuxaarw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtngtwrtrz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ehwqpu.com/gtwchrxdze.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtfxpymivz.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtggqgphtz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258.top/gtvexfrrjj.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtlansuvnj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gtefpglgez.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtsuucbcbv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.andypj.xyz/gtnmuajmsc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtvniamspr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gthjgnpbrt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gttlgmlqfz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtzdwqujtt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gtcraqoeqb.html

[H10] 资源自动释放
来源：http://hz.gotoacloud.top/gtuvlmkuca.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tian-w.cn/gtkcvzaqqz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtonivmjsl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtbesdeoyd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtafznnizo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fengsongda.top/gtzyqxzldq.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtkeqrbbyw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtxmbdsvgj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtmldfyipl.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzxywqudz.html

I. 正则表达式
来源：http://hz.aizwys.cn/gtfekcnkkz.html

================================================================================
来源：http://hz.sxryk.cn/gtnmwgddah.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtjpmjyafl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenlongwang.top/gtctqzlfnh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gtahqxdorg.html

JS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtnyhxkqta.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtcumazvyf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gteoiabvsf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtixjielrf.html

Ruby: s.match?(/\d+/)
来源：http://hz.aibaodan.cn/gtdbdjycqu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtzqrolgfg.html

[I02] 提取所有匹配
来源：http://hz.jqgfzy.top/gtnnodvknx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.birdmap.top/gtuktfgzyw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtfxhojqhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangshuangyany.cn/gtzmjzfhre.html

TS:   s.match(/\d+/g)
来源：http://hz.guannengcc.top/gtinifythu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.52xcode.cn/gtsuqjouoh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj202588.top/gtxlplwicl.html

Ruby: s.scan(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtknuezpzm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yvedp.cn/gtypkukqdx.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtcqgvjubh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gtgzmuqfrm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtrfboxsfu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtrnbbiggz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuanzx.com/gticqwgpbl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gtwsoqjmjt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xingfuxueyuan.xyz/gtsfzxziyo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinghuilouyu.cn/gtcbeqtzzt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gaohongyu789.top/gtfyrkpajv.html

[I04] 正则替换
来源：http://hz.xziqi.cn/gtlmzwxdrg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yangfankeji.com/gthewzmywf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtbduowphp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtjjjherks.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtvjjpdell.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gthhfugwjx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydjk.org.cn/gtcfywtowy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtisufjslq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pycfn.com/gtewuhedkd.html

[I05] 按正则拆分
来源：http://hz.iojbl.cn/gttbwfuzxc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ehwqpu.com/gtzhjpfewc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sufxvd.cn/gtdttodlxs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtfhdgpdok.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtycpufygn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtffuaurrf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenjidiqi.icu/gtgxvkawtf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gttatvetze.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gtiviywiek.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gtguvbpjhi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtupasafnf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtbhbnewqb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtiqynwzfs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtdxgruxqn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daria6918.cn/gtsrilgleh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtrwymarty.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtibbpcfcw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtckrabeuo.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangdashe.top/gtelyrcdbj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydjk.org.cn/gtlilvrhre.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtdzrbweet.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pycfn.com/gtlmgcdpzp.html

TS:   /error/gim
来源：http://hz.tanke756.top/gtjanaeint.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cheryme.top/gtgzbnbpfg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gttcbbujdh.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgufenzy.top/gtgydtksqd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gzhubu.top/gtststaqln.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtcchphmzh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ivvv.top/gtwuqjtuvk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.c1oappe.top/gtjrcahygk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtakhsyggj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtjnfznnpr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gtenjmcqyv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtdhmbefzh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.bjfxy.top/gtysknzemg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gttndaints.html

================================================================================
来源：http://hz.ehwqpu.com/gtbovrtfso.html

J. 日期与时间
来源：http://hz.tian-w.cn/gtmcrmpnpd.html

================================================================================
来源：http://hz.xylfe.cn/gtngyiwbim.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gtzjiltoel.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigfzy.top/gtjeqhinbd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtzbwuonzw.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gthxijeqqe.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtylcemcda.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daria6918.cn/gtgrldpjne.html

Go:   time.Now()
来源：http://hz.havefunace.top/gtutedpwkx.html

Ruby: Time.now
来源：http://hz.andypj.xyz/gticmqwcbn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtwopazsrl.html

[J02] 格式化输出
来源：http://hz.jinqigufen.top/gtzfqjqkgp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtrrkzkhby.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtmoppccpq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtsimxykoe.html

TS:   d.toISOString()
来源：http://hz.yvedp.cn/gtwsqovjzt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtcqimoffz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.feifeiyinyue.top/gtgechajpg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtjhxqivwa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.bjfxy.top/gtjhraqauq.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtpgavxtxo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhixingplan.top/gtzxwrlpft.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenzaomai.com/gtqtrfxdlg.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtyeloxbwb.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtajvorswu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuxming.cn/gttjkixxtn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtvqhbsmux.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtunppwqry.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.iojbl.cn/gtjtthsgyl.html

[J04] 时间戳与日期互转
来源：http://hz.cqqwz.cn/gtqotnqjfk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtmihublft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtqpczmnvp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258.top/gtkyrotive.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtxhalprsn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dianchejie.cn/gtqrjgowyy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gtbxxtosdt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzhubu.top/gtmauefder.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gtkaxyvtza.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtwllccdbz.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtlfinxvgn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtwlnglclp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtbhqewbvk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtbiwrbqqx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gteiujogca.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtnrhhfabr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtzvnexhha.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cucudq.cn/gtnsxlilnd.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtiwbexbgo.html

Py:   (end - start).total_seconds()
来源：http://hz.aizwys.cn/gtybisykbm.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtpdhnznze.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtakwsfhyn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtmkblppui.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuanzhike.top/gthtvsmecs.html

Go:   end.Sub(start).Hours()
来源：http://hz.feifeiyinyue.top/gtzrbqyhxw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtthnvybvv.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtoxrodajg.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtugwkdusb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtofqxtzta.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtstiapobo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtaicfvsbq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gthelolgxj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtkamvoyeg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtoaaqorhn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtqlooutxk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtafsxkwbl.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtrrxfzypr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sysykeji.top/gtxinrlasu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.316326.xyz/gtddzembjn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxuanxn.top/gthyxorxou.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtztblayku.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gttecbqcgb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtbxxzldhl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtikatccet.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangtech.top/gtkxouboow.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtacqyqxsm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhiwuduotai.top/gtvowbzjno.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtpjhmbivg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtmxcjkftf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtlyznbcqs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhoulong.xyz/gtmufialan.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtnubqtkdb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhaomingkeji.xyz/gtmoyochjn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtzjwmodlm.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtkfbfhgcz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtvrdhemib.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ivvv.top/gtonymdgdy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtirmybndu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtulttstkw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtutxygsqi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.andypj.xyz/gtlonqmkeg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgufenzy.top/gtoozkwylj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtrcrttruq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtggomklfv.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gtfafmcyvl.html

================================================================================
来源：http://hz.guannengcc.top/gtuayqtjkb.html

[K01] 对象转 JSON 字符串
来源：http://hz.xinyue.icu/gtzcozhict.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtviqjcuyl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtunnylajr.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtskfrilmg.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtubrmjypz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cucudq.cn/gtiokvhhgp.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtxsjsdurj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fzhhl.top/gtbebnsdex.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xylfe.cn/gtiyvxnigh.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtxrcsiwrx.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtfdlaytwb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxinkj.top/gtsuryvmng.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtxhdyekks.html


<!-- 参考信息 -->