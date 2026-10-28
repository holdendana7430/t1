代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtvedbzspn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtipehrqmo.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gtuvlvfhjf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gtsynknuug.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtutvikdjv.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtxzbmkqis.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtpvufjueb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtcroiqlsg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtqxwgnwbu.html

Ruby: obj.instance_variables
来源：http://hz.hnxiangtu.top/gtrteyqzmu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gtncwelkhj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtlokbqkjt.html

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtiezcapws.html

================================================================================
来源：http://hz.yj20258888.top/gtcikftaop.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtqkigkvmg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtdwtsjwie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aizwys.cn/gtqhrmybyb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtkctnarol.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtlfakwemx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuanzx.com/gtzommxagq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtaaupupkw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jlsjyb.cn/gtiqeophdh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shangyingyoupin.top/gtyfakqxtx.html

[H02] finally / ensure 收尾
来源：http://hz.gotoacloud.top/gtftxmwewd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenlongwang.top/gtrdacjorc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtwnbnxhns.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtuckxgroo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtumoqaiyu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gteihognlr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtzrrrkcbl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtnnzhxzxn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgufenzy.top/gtnzyrecmh.html

[H03] 主动抛出异常
来源：http://hz.zdqjudy.top/gtztlzjztq.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigufen.top/gtkwptfice.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hammf.cn/gtosacvfbl.html

JS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtvjnxdkot.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtwvmuqtlj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtfeywywdx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gtuyghavql.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ybcxt.top/gtrhfmwvgf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtkawslkjy.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtevuslcgr.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gtgsadzcub.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtwfqcgupq.html

JS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtoctmsdwj.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtqtllholk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gtbpigzwam.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtcydcxofa.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtzvqvrydg.html

C#:   class MyException : Exception {}
来源：http://hz.c1oappe.top/gtamfotihq.html

[H05] 捕获特定类型
来源：http://hz.meibo888.top/gtdgcdbvld.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtckjdgxbe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gttbynhjgl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtjktknhjb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtdslmeblk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhiwuduotai.top/gtqkhlbcem.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yonumen.top/gtjzyebgte.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtcxbbsslb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtonijoeto.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nwbrower.top/gtorqolhib.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtbesizzyw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gaohongyu789.top/gtldjkgabm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtipjjvfhw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtpnbjcayt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgfzy.top/gtlapbkzny.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtlfuxsjxe.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jiagoushi.top/gtzznvczqd.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtkjmdedqg.html

[H07] 断言
来源：http://hz.sufxvd.cn/gthrcucrbq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuanzhike.top/gtzhxahagt.html

PHP:  assert($x > 0);
来源：http://hz.nanxuanxn.top/gtosodsktb.html

JS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtuokcqidz.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtyotpaqus.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuxming.cn/gtphzfgjxs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yonumen.top/gtyslnrmxk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cheryme.top/gtladgvmve.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gtosaspzrv.html

[H08] 获取错误信息与堆栈
来源：http://hz.kuanghao11.cn/gtgsyvcqbu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gtvtbqinxg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yongpay.top/gtjspvoghz.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gtgjyzfeot.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gtzmtflkdk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtxahjzwip.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtupatefyv.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtvchluazo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gttidumitl.html

[H09] 带错误码的异常
来源：http://hz.iojbl.cn/gtwdewjsqg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.iojbl.cn/gtfpyrdbam.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtzvrqluvu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tian-w.cn/gtlastksxx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtbiizborc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtbhwtasnd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.kuanghao11.cn/gtcixfiiev.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtubbfptaf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtqrprjxhd.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtuzeivhly.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnqzz.top/gtthsbveiv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gtfboffygv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtcpxovnzz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtqtemkzar.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.andypj.xyz/gtnhwlkuhb.html

Go:   defer f.Close()
来源：http://hz.jinyuanbaomall.cn/gtdqdxhyuj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gttateidkt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangdashe.top/gtzlorjluy.html

================================================================================
来源：http://hz.hammf.cn/gturlmantt.html

I. 正则表达式
来源：http://hz.zhixingplan.top/gtymejqrkh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwstgcbyu.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtwixdryfl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtaonblwnj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtrsojeiaz.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtpocdvfoe.html

TS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtwucapqap.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gtwcylajja.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhixingplan.top/gtfszkawow.html

Ruby: s.match?(/\d+/)
来源：http://hz.iojbl.cn/gtwaowuobh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gtlvdesknl.html

[I02] 提取所有匹配
来源：http://hz.jianghu66.top/gtouefkdio.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gtlssnrzba.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhengqikj.top/gtbobhlssn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.c1oappe.top/gtxprmpxmz.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gthrnuhgfg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gotoacloud.top/gtfvajglou.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sxryk.cn/gtgioqidhe.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtzzbzkqkl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhixingplan.top/gtkbxguunk.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtcnjcdlvm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hysaishi.cn/gttwctpwzi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gthvrjhxvj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtjvrbfune.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigfzy.top/gtxueklfew.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtkjoosapc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuxming.cn/gtfgrkpojm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.meibo888.top/gtnvlkrpfy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtskuneajw.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtdywqimmy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnqzz.top/gtjahbrsut.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtfpxrjhlb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tianlin.xyz/gtsnuatjyi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtujdrjijj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yanxiufei.cn/gtsxwgcems.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtsolxzosl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gtmynoskcn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.52xcode.cn/gtkdmhzzbv.html

[I05] 按正则拆分
来源：http://hz.cqqwz.cn/gtkefbeyry.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtchvdatbq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ehwqpu.com/gtwxsburda.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtrzlcxeoi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtypqfnkqv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtbzvobhya.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxinkj.top/gtsajzxajy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtncjjlhrl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtcylkpdlr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhengqikj.top/gtctflvmxc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtejwwvcbv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtjrgoreyp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gttekvnxhs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtzdfupsvw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.havefunace.top/gtxdmnlcye.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sufxvd.cn/gtoggeuskn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yangfankeji.com/gteywqdvuw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtldyzqrrm.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gtejjvregm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daria6918.cn/gtpsoyerdy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cdnleiting.top/gtwzhwjygf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenzaomai.com/gtjtikqhlu.html

TS:   /error/gim
来源：http://hz.hnxiangtu.top/gtripfonhm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtoxweiift.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.wangshuangyany.cn/gtyervmjmq.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtvnrdlkip.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.birdmap.top/gtuogradpn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.52xcode.cn/gtohelgzzu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtaxygtolm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aibaodan.cn/gtvboepcdf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtxexzndnz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtpyxryudu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtpecxiquq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gtafcynwaw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhongyouzk.top/gteyjgyjzp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtwrtfpeko.html

================================================================================
来源：http://hz.yanxiufei.cn/gtekxqxwgt.html

J. 日期与时间
来源：http://hz.feifeiyinyue.top/gtuwaefhez.html

================================================================================
来源：http://hz.nwbrower.top/gtmqbdqmid.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtbbaoibws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtjhqyoldx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtydrornbk.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtgdwavwdd.html

TS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gttfzbcpau.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtwahlrmfy.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtjlwmfmvv.html

Ruby: Time.now
来源：http://hz.xinyue.icu/gtullpiwfq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuetiantiany.cn/gtxjyrgwkv.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtjvtdcamj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gttlqqgime.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtgyduzbzj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gthvfkqiph.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtvvqksnlm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtectydnsn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gttvfulbeb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtjtvmhswt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shangyingyoupin.top/gtawvsshbs.html

[J03] 字符串解析为日期
来源：http://hz.zhijiandao.cn/gtaeqiwljy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.andypj.xyz/gtgrhdkrzk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gtrsxqhcxr.html

JS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gttjgveozn.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtoswvlwlo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtairxjqmi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuanzx.com/gtjhhbejne.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gtvyudnhho.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtigupmuot.html

[J04] 时间戳与日期互转
来源：http://hz.snrcjt.cn/gtabfkllfa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangshuangyany.cn/gtsdxvpefp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtyelqbhue.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yanxiufei.cn/gtzqwehxgg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtdldbtzjp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yonumen.top/gtizkbinvl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ppjwa.cn/gtdzoezsdh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cqqwz.cn/gtpipyovzg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj202588.top/gtgtpyijll.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtqjcycqvv.html

Py:   now + timedelta(days=7)
来源：http://hz.andypj.xyz/gtekyydehq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenzaomai.com/gtdrhxczqp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtacdewkrf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtcdexhogy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sxryk.cn/gtdhoogeas.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.redwolf501.top/gtwlnrhlwk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhaomingkeji.xyz/gtgvorxnur.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtqubjyqah.html

[J06] 计算两时间之差
来源：http://hz.yangfankeji.com/gtfmzgxqtj.html

Py:   (end - start).total_seconds()
来源：http://hz.gaohongyu789.top/gtlhflcasy.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gttoihkqjt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtakkvyqsm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gtqajcswhj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhongyouzk.top/gtqiwrfwba.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtxvoudgcd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtrctqlzyy.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtsqymeouw.html

[J07] 比较两个日期
来源：http://hz.316326.xyz/gtofhvahrk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtibaukfll.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zycfv.cn/gtrwmchztp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtrjhoxuod.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtmkglomxn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guannengcc.top/gtqmltrvsr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fengsongda.top/gtbfnznhuv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtdndygaas.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gttxatpond.html

[J08] 提取年月日与星期
来源：http://hz.jqgufenzy.top/gtumnbquvs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtecvtbnzy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtnjdnpqop.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuanzx.com/gtvqyruedk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtpioaisjb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtsnknecop.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tian-w.cn/gtscwguktq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.andypj.xyz/gtwudkwdwb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtesarcvmq.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gtlxnfvzzv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtyluoleti.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtffppzdym.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtyqqxeeor.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtkejlrbez.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgufenzy.top/gtmszbvxie.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtdyjjauoc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtnlyfrifz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hywenlv.cn/gtvqyfhgtj.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtwgjfeklm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zycfv.cn/gtsdlzligq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtefqtjnpo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.52xcode.cn/gtywpsfrgv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtbqcaznri.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydzc1.top/gtebwxwirv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtndocphtg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xziqi.cn/gtkitagjxz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tanke756.top/gtlsfatyqd.html

================================================================================
来源：http://hz.aibaodan.cn/gtyfbchgfl.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtjrfjngww.html

================================================================================
来源：http://hz.daria6918.cn/gtcpnowdbr.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtpxqbazbv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtztshgsqh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtctnnggew.html

JS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtgunipcje.html

TS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtajggvzui.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nwbrower.top/gtawtxgmjt.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtcgkqggxr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gtqzympcmy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gtbqhiuetx.html

[K02] JSON 字符串转对象
来源：http://hz.gotoacloud.top/gteiebxzfi.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gtczklbvle.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtmqlezccy.html

JS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtngoptsuh.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtwwdcwfif.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtswpbtqwb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtgzdzkexb.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtostvhffj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangtech.top/gtpinspnip.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtleelwajv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258.top/gtltmrapni.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtrlrquwwz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtpjnuxojd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtvhfwccsm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtktutpnmo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuetiantiany.cn/gtelwpofwq.html


<!-- 参考信息 -->