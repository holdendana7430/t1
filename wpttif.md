代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.cheryme.top/gtgzicgujq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtlnuhdevd.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtzhrebmpu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigfzy.top/gtgnfdfjjp.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangkeji.top/gtbfzsnzdu.html

JS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gtzwgfudyf.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gttblpasgd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.kuanghao11.cn/gtrkgvgiti.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xinyue.icu/gtinosoqcj.html

Ruby: obj.instance_variables
来源：http://hz.shzxlz.cn/gtzyflocka.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.0kj1m.cn/gttdnwiwvn.html

================================================================================
来源：http://hz.svipenyu.cn/gtlsrjpzjs.html

H. 异常与错误处理
来源：http://hz.xuetiantiany.cn/gtzverpkkg.html

================================================================================
来源：http://hz.ybcxt.top/gttkcmufxb.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtjjpqppoo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtcrzjtmzo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gteekarggc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gtiyempfot.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.havefunace.top/gtitaidyzr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.52xcode.cn/gtqbaawers.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gtbdjzyxqm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtrxyreinr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gthithlpwz.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtjogpumon.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tian-w.cn/gtnctjvuzz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtqvjayepi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtauuyiyec.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtlwjcuzye.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtpuenalqw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtagipxflj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.9152youxi.cn/gtsbndcyki.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangdashe.top/gtpgjmhcpg.html

[H03] 主动抛出异常
来源：http://hz.zdqjudy.top/gtwvuywqtu.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtlfhmizoa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtwnqrjhmz.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtxuivyttg.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtorwzqxuz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtvewuishd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.redwolf501.top/gtkcjzfcsq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.9152youxi.cn/gtrerewgpq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtvsgrufia.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtkvplrefk.html

Py:   class MyError(Exception): pass
来源：http://hz.cdnleiting.top/gtcdsysfyr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zycfv.cn/gtjxujzvmp.html

JS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtvamzybrz.html

TS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gtdmqwlxck.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtrmmdslsj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhoulong.xyz/gtzjmlboal.html

Ruby: class MyError < StandardError; end
来源：http://hz.hammf.cn/gtgtclxcop.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtrlolzyqu.html

[H05] 捕获特定类型
来源：http://hz.nwbrower.top/gtgpmzwonw.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtduinpanz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenjidiqi.icu/gtyiqwmupc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtjukyhfjf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtumtrkoky.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuetiantiany.cn/gtbomwyeax.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtklkppfzv.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangdashe.top/gtregnxzii.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yonumen.top/gteimxaojj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pycfn.com/gtqnyumlqr.html

Py:   value = d.get("k") or default
来源：http://hz.yangfankeji.com/gtuelmuael.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtvduqpmbl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtijzmnyko.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtovcvxeeg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gtdrgjmbda.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtkdavoele.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtfvsmcovk.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtuxebcsyg.html

[H07] 断言
来源：http://hz.yvedp.cn/gtqoyaqwjq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtotpqxdsi.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangtech.top/gtwfkjihhh.html

JS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtbjfzlbab.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtetiytubp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.9152youxi.cn/gtobwfqikt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhijiandao.cn/gtklfjbfzj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.smart0.xyz/gthbywmdat.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ppjwa.cn/gtpjibeama.html

[H08] 获取错误信息与堆栈
来源：http://hz.zycfv.cn/gtaltsfojx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtbljewyaj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pycfn.com/gtgrtlvrzd.html

JS:   e.message;  e.stack
来源：http://hz.hywenlv.cn/gtqfyjgmmp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gtnvzzqune.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pengpengdd.cyou/gttxrkrdrr.html

Go:   err.Error()
来源：http://hz.xuanzx.com/gtguknxmcr.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gthfkalrhc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shuidangran.top/gtmcdsaooz.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gtcliwdcyt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gtmozytwkd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtrjrbvope.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gtcfwwtkoq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.iojbl.cn/gtpmxncldu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtqzwfbbvo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtqjxtwwkm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangdashe.top/gtgyttqenj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtffyquatc.html

[H10] 资源自动释放
来源：http://hz.yj20258888.top/gtqjmcxgyw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtywhjumor.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtuoydfcrr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtjvmiwxij.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtosxdqdvs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuetiantiany.cn/gtdfbeydrn.html

Go:   defer f.Close()
来源：http://hz.jinghuilouyu.cn/gtqtibfdth.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtvhdgiptc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gtszzwlnph.html

================================================================================
来源：http://hz.fengsongda.top/gtkpvbfxby.html

I. 正则表达式
来源：http://hz.iojbl.cn/gtyihmbmhm.html

================================================================================
来源：http://hz.daria6918.cn/gtbtvmjssp.html

[I01] 判断是否匹配
来源：http://hz.bjfxy.top/gtqvdcyqdg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gotoacloud.top/gtcshqpgnp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtzebfcwly.html

JS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtjravqmnt.html

TS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtpycnpcbm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daria6918.cn/gtwhxfrfqr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xylfe.cn/gtqxurgglp.html

Ruby: s.match?(/\d+/)
来源：http://hz.iojbl.cn/gtpkchctbo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhengqikj.top/gtazcbkbzi.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtqnhdnqxg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuanzhike.top/gtqimulubi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guannengcc.top/gtvigwhsua.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.snrcjt.cn/gtfvlrusxi.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtkbwtwzwe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yanxiufei.cn/gtqvhrxzes.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.birdmap.top/gtcwlnplit.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtzywatiyw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.snrcjt.cn/gtaexxwpak.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtvtrfdtxt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtadmlljcu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zycfv.cn/gttxcbazvt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gtnxqlbshg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtorwwxtvj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gzhubu.top/gtclcoachw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jlsjyb.cn/gthmgtmlkn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtxhxipmsl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gttcveikla.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtcitlkcuu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cheryme.top/gtjplzpamb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtgaxjncqr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtftmvdyej.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtuleijktm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydjk.org.cn/gtomxkgnzz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtjksykfdm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fzhhl.top/gtecktdozv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cqqwz.cn/gtfgqyroeq.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtmfzcagqy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.bjfxy.top/gtvgeukyjp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gtdfyvwjyo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtjcycriak.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtoadjqpib.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gtcpbcthwd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jianghu66.top/gtwybwsuvo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtpiwuymvi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aibaodan.cn/gtkbpvbsrs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gtquamwdtj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtuhujzpdd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtnsxvfnts.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtxggpfqcp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtkmdresgn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yangfankeji.com/gtodktrsyh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gtvjrexpbj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yongpay.top/gtqgnwnlhn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtvsrawzyw.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtjddojwoh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yvedp.cn/gtdsoaosdc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtsmrbqytk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtfpmixtcm.html

TS:   /error/gim
来源：http://hz.zhijiandao.cn/gthdqpebph.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtjvdpxshf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtauqczbta.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtltdovnya.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtvpmbpawa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtlrluzkhh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daxiang520.top/gtemcdsuil.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtqilvgffp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtkrluyqud.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtwrzgmpmu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gttiagmrev.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtkqplrdtl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.9152youxi.cn/gtafrwvdxj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cashguo.top/gtitgmoyfr.html

================================================================================
来源：http://hz.316326.xyz/gtdfggcqpk.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtuyvuinwd.html

================================================================================
来源：http://hz.cdnleiting.top/gtvwufsupw.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gtxuyblzdo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtbqynkdrp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtlxbdfwvd.html

JS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gthwedntls.html

TS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gthddimsdt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ehwqpu.com/gtacfprbzo.html

Go:   time.Now()
来源：http://hz.yj202588.top/gtqxkmvcvw.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtwtigdzmq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.bjfxy.top/gtzjpspviq.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtaeoptask.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtslfaybun.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtjbmmmakg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtvpoegbjw.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gtwahntkfc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtywdsjsha.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj202588.top/gtgxmatect.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtbovoxjps.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtmtdnxdpa.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtwmxajxqt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtgqnlexjt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtgomhefat.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtspqwfvjg.html

TS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtdxpppvxf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtzwokblul.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258.top/gtzuihhucd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtiqoeruwk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtmqtcbssl.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtveodoqhe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gogol.net.cn/gtfzpfyitw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gtldpbctns.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daria6918.cn/gtximvzpbv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtkmkjwhai.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cashguo.top/gtwblsntwf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtskywjdvq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hammf.cn/gtyoxvgqqx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yangfankeji.com/gtuysgbzxg.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtihkmoywj.html

Py:   now + timedelta(days=7)
来源：http://hz.ivvv.top/gtlrrohdns.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtpouhoftq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtocwdxrbi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gtmsmbvphf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gttiimxvbs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtffvrtaub.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tanke756.top/gtkaoeiiop.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtjyxruibw.html

[J06] 计算两时间之差
来源：http://hz.cashguo.top/gtsruvzaxb.html

Py:   (end - start).total_seconds()
来源：http://hz.sufxvd.cn/gtylduranr.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtwlxadrnh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtqeqrknpm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtgrbvsjkw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtclzvjijp.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtffyhldyp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gtmaelklrk.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtwlbxfnww.html

[J07] 比较两个日期
来源：http://hz.hongshengwenyu.top/gtelcniivw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtkjzgqcwk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtbmiezqxx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gttzbsvdba.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.dashuyun.cn/gtkemvwkef.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gtimwjyhtd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258.top/gtkpirvahf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtgngzqpgk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtbhmvwqey.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtzzpgcbai.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtborfbylk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cucudq.cn/gtpvgqlkdd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtnassuorl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtsuennxsf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinyuanbaomall.cn/gtqbawfzbp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.0kj1m.cn/gtztutjcac.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ppjwa.cn/gteprqhnax.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtjiwkppld.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtueyhkrjg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtrazbtqqt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtweftcots.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtebcovmrz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtfqsyklux.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtatzxggji.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtoczkqkiu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gtyswmscln.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtazjwxbaw.html

[J10] 取今天 / 本月第一天
来源：http://hz.shanyushiyangkeji.top/gtobhonvww.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ywan-chungtsiang.top/gtukpcwxih.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.0kj1m.cn/gtqviqomvc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtduafvedv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtiollkqea.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sweek.top/gtxllgylrg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtfbkpqlgn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gtpvzzeeqq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtdvqjbvzg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnrdhzixq.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gtajqgqqhv.html

================================================================================
来源：http://hz.redwolf501.top/gtxobzcphr.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtlrdykznm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtkaeqzujx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtjojjphce.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtusxcsxsv.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtalecluao.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gteokbrmjx.html

Go:   json.Marshal(obj)
来源：http://hz.gotoacloud.top/gtvxcxagws.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gthglzqftx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangtech.top/gtrhaacdqd.html

[K02] JSON 字符串转对象
来源：http://hz.chenjidiqi.icu/gtfexgzlql.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtsjucewfq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtepvpvjom.html

JS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtaewdqfpj.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtfvzunrxg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtindwtcxa.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtjbckgpbm.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtvvhudfvg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtgwhltnjw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xinyue.icu/gttladmhkt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtojnwsjwk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtyohalndb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gttgszredu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtehdgnnbp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtfbmhmfgq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtrsffhlfc.html


<!-- 参考信息 -->