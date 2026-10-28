代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtccvguhsh.html

[G15] 枚举
来源：http://hz.pengpengdd.cyou/gtdsxdunup.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hywenlv.cn/gtyfakhkub.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gthoiwgtes.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhijiandao.cn/gtbvmfgqvp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtmpewzhws.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtmylavxzw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnqzz.top/gtnkoklwzv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.c1oappe.top/gtqwdlhhay.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtamniknnf.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgufenzy.top/gtivgpkjrf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtqrtscdhg.html

PHP:  get_object_vars($obj);
来源：http://hz.shuidangran.top/gtxgnngrox.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtbwrdtsst.html

TS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtziicxyvd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtuxpjzpnk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtaiexltjz.html

Ruby: obj.instance_variables
来源：http://hz.c1oappe.top/gtijehupxb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtfsvdzqkm.html

================================================================================
来源：http://hz.shzxlz.cn/gtnniswsml.html

H. 异常与错误处理
来源：http://hz.feifeiyinyue.top/gtznashpxr.html

================================================================================
来源：http://hz.fengsongda.top/gtekilaueg.html

[H01] try / catch 基础
来源：http://hz.gaohongyu789.top/gtyzqasuwa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhengqikj.top/gtqgrbasvk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.svipenyu.cn/gtvvajnrlh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtvirvdjom.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtsubltorc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtgwnboxon.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinqigfzy.top/gtiqxopslv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgufenzy.top/gtmhdhfkkz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtgywgnokj.html

[H02] finally / ensure 收尾
来源：http://hz.zhoulong.xyz/gtigebflgj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtloozkjqz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtclxugrak.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtcuizvbot.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtkkhcxvco.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtxsdonuiy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gzhubu.top/gtexuufzuy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtvmcvhcrf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtyyuaxowa.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtcpgcvaov.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gtajnrvtny.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gttnukicnl.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gttgpcxtvj.html

TS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtcviqiwvd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtatzjwdms.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yvedp.cn/gtmmbaorbk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtrbjdabfj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtyxmjgmae.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtnikggekk.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtwkbqyjzh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtlkdbtzdy.html

JS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gttnkenika.html

TS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtzhyhzown.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtknkrwkfa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gtbbqyjtqy.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtdywwyqkg.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtxjcavxsu.html

[H05] 捕获特定类型
来源：http://hz.316326.xyz/gtevlsjrld.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtjyezyapg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtxhrgkaxm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtminhsobc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtmigvuqkj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtpxennjav.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtufdigerz.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhengqikj.top/gtqlieicql.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hongshengwenyu.top/gttnksxcjk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xziqi.cn/gtxfyczxvw.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtmetagoxu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtnasxbzhc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtazmqfhne.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtgdprzjdh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tian-w.cn/gtqhjlsvjk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gotoacloud.top/gtlvntdzjm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtpqzcudoe.html

C#:   obj?.A?.B ?? default
来源：http://hz.smart0.xyz/gtjwobthpu.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtayiydtsg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtjcojkfbq.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtlinfufur.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtmqlwwpfk.html

TS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtfcnixsnw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuetiantiany.cn/gtnlboqrbm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtvjzvdsde.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xylfe.cn/gtnchadjfs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtsgtohzdl.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gthbtxhxbn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shuidangran.top/gtubtiyaze.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtklywqjzq.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtbcbjqoer.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtthgpjanv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shangyingyoupin.top/gtzhjqhfzz.html

Go:   err.Error()
来源：http://hz.redwolf501.top/gtogwlgjzo.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtxqulictr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cqqwz.cn/gtzkjoybvj.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gtqekntaph.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hfpthk.cn/gtzbfmjivz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yvedp.cn/gtlllhidff.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtnmcgdntu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtkrzbmehz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jyoumei.cn/gtqpzrgaub.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guowangkeji.top/gtcfmprema.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.c1oappe.top/gtxltnttex.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtgvcuknzx.html

[H10] 资源自动释放
来源：http://hz.jianghu66.top/gtfkbkbyta.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gtldqncczi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtgovlffug.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtclsglkqb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtyhgqgjie.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shzxlz.cn/gtawqiximw.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtmqbuxssx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtaqwnhpxg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtsljtthgs.html

================================================================================
来源：http://hz.snrcjt.cn/gtjegklqeg.html

I. 正则表达式
来源：http://hz.xziqi.cn/gthyaumeuv.html

================================================================================
来源：http://hz.hnqzz.top/gtuovhfrvs.html

[I01] 判断是否匹配
来源：http://hz.c1oappe.top/gtvwcsopee.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtwqunajse.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtnbepebtm.html

JS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtzsojslox.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtcgtvbkyi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtspbxqrow.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtjtntzssq.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtukgyanad.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258.top/gtuxfiiqoz.html

[I02] 提取所有匹配
来源：http://hz.xuanzx.com/gtrqcktmix.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxuanxn.top/gtrzfdijce.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.haohaochexian.top/gtbtqidihq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daxiang520.top/gtjvsneanw.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtolxybrtr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtiacrvriz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtjrzdhsbo.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtzrswrvlj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gtwpwoeyik.html

[I03] 提取捕获分组
来源：http://hz.nwbrower.top/gtuaydfctd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.9152youxi.cn/gteslcaakt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtmpqtenae.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gttmtvrrsw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xingfuxueyuan.xyz/gtggoxakix.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dianchejie.cn/gtxbythsyu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hammf.cn/gtacsgtcdu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtxwwdxdai.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtbyovmozt.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtltexnsvw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gtqygtlfhk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtjjzscpvl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtfdacqrsf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtuxkbzrah.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yvedp.cn/gthaiypujn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuanzx.com/gtgusaetvr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtofldddrw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gtjcimcdnh.html

[I05] 按正则拆分
来源：http://hz.jyoumei.cn/gtmwqrfdre.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.andypj.xyz/gtyyipeygk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gticrafoex.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gttengajfd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtzmffoikj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtiupfkqfu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cucudq.cn/gtwfulbsin.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtdqtfjugo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.redwolf501.top/gtewfaufkf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yvedp.cn/gtvejzkpdg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtlmfldbtb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gtzgvygyyi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtkoymmssy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtwkvbgpec.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.feifeiyinyue.top/gtqhvrpwbi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cucudq.cn/gtultyojoa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtafdvqpig.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtvdsnllqo.html

[I07] 忽略大小写与多行模式
来源：http://hz.birdmap.top/gttgmtgwcz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtnusdjmdx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtktfoaynu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtvkyzdjrn.html

TS:   /error/gim
来源：http://hz.yuxming.cn/gtgizhcmol.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuanzx.com/gtscgoijih.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtdvoddywy.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtbnzyehyy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtihswfpaq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtelrocodi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gtseykboah.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtilrfsbrf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtdftqwatu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtcrakysxa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtlohpnufd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gtpguiqicr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtolaxbglp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtpbevzrkn.html

================================================================================
来源：http://hz.guowangkeji.top/gtpgkadidm.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtrgapejjv.html

================================================================================
来源：http://hz.0kj1m.cn/gtzehiikqb.html

[J01] 获取当前时间
来源：http://hz.yuxming.cn/gtmslkmlvg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtrzeesmur.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtrawrkbqc.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtnkzonjsc.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gttdlpsahr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtbqcvgmdv.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtswnhhkey.html

Ruby: Time.now
来源：http://hz.gaohongyu789.top/gtszwjcslj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtkayvvazb.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gtbopofcpr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtckmbifox.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gttqqkiozd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtqxtfbgmf.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtspghlztf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtyjzhllpa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daria6918.cn/gtqppwvhxw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtabaujqka.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gttfjjbcrj.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtzwtorfeq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gtmtaufhhz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtckcrxhvi.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtgvukpwzs.html

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtnayblhrm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gterzmmhox.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtkjlrelah.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtaslsotfv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtvvavnrlv.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gtikxtrurv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.52xcode.cn/gtqsxrtsmy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ivvv.top/gteqvdvdym.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangkeji.top/gtxbulghcp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtrurcmtrv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gteigbwldy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ivvv.top/gtitnilwdv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtlhqjbnwo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigfzy.top/gtjxtnxrau.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtfdkickoi.html

Py:   now + timedelta(days=7)
来源：http://hz.yj202588.top/gtnseqgjsl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gttrmvsjkf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtipwcrvkf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtajjtvzid.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtpdqfvanf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shzxlz.cn/gtwxoawzej.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtsgfzlzze.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtieifcuub.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gttmahfkjk.html

Py:   (end - start).total_seconds()
来源：http://hz.xylfe.cn/gtlyenbbwb.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtzmfqinpa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtoifeuxpk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.havefunace.top/gtiauremue.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtayyrdwuc.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtdiexucdg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xinyue.icu/gtsbbhrewn.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtnnkzrljl.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gthznyiivo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtbfjxlnsj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gtryqllits.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtuomppdgc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtsddksbud.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sysykeji.top/gtdnhostix.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtmkymrhwu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gttsxviuir.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtudhtagma.html

[J08] 提取年月日与星期
来源：http://hz.shzxlz.cn/gtzvrfvpgs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gthddqbjhw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gtpxjsmsqd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fengsongda.top/gtcoteimei.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhongyouzk.top/gtgmhrbzou.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gtuvezglti.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gtrxhjisba.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gtgnwzuonf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtuiqhexcm.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtmlxwnhmw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtdgpsnkzf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtuxljqvzn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtjasctzdv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtbiooqrwm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jiagoushi.top/gtwxpdswte.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yvedp.cn/gtopseeodh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aibaodan.cn/gtcyaslpjc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtnidlakpw.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtydtirled.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.mhx1999.top/gtprnyrebe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtbvenwnjz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shangyingyoupin.top/gthraqiget.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.mhx1999.top/gtytdezgkc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydzc1.top/gtfhkwzizn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtseshsyhi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgfzy.top/gtaaraxcoj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ehwqpu.com/gtabuyoevz.html

================================================================================
来源：http://hz.guowangkeji.top/gttwhngyqq.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtyzvuvhkr.html

================================================================================
来源：http://hz.iojbl.cn/gtsjvbazft.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtrmiizxdu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtuylbprxb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtogrjbibu.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtrelwotsm.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtuilkkimq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gthwkrlozl.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtrcftnulr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtpovzhlhc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtesyjljrh.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtnyzowbwj.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtuxlpmbpr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gttqzyuyls.html

JS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtmegosjdb.html

TS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtguptrnkf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtsitvutsf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtqvuvwxsv.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtaeymxlhz.html


<!-- 参考信息 -->