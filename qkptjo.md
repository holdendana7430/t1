代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtsebsqlna.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtuxohqgyl.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtvrscgqgl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtstmlddje.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtrqvdwlyz.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtzghhglup.html

TS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gttpxhiwnz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hfpthk.cn/gtwbvswtmd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtvodwcxdv.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gtggtxzriq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtpyvitmgg.html

================================================================================
来源：http://hz.sysykeji.top/gtcjlobztd.html

H. 异常与错误处理
来源：http://hz.jqgfzy.top/gtcqwaezjc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthohqqeat.html

[H01] try / catch 基础
来源：http://hz.zhixingplan.top/gtgnnoomyq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gaohongyu789.top/gtccrmuqyy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtogbzqzqb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gtjewralrv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtrhbwrsyu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtcrgrkxns.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtkogiwtbj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xziqi.cn/gtndhdjpea.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jiagoushi.top/gtpypvvjeh.html

[H02] finally / ensure 收尾
来源：http://hz.zhongyouzk.top/gtbvmdwbtp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtwwiquakn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtyasbhugd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtnyzmbrrp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtmkaragda.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtrvlxscbp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtmfnykrvc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ybcxt.top/gtegabgyms.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtvmrpoohi.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gtrzjiwebm.html

Py:   raise ValueError("错误信息")
来源：http://hz.quarkkingdee.top/gtzdbpgpbe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtpqgclkul.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gteisehggx.html

TS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtmjnsoyte.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtaasddxox.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gtkncqutms.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtsnwqwfxq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtkiiuskqk.html

[H04] 自定义异常类型
来源：http://hz.ydjk.org.cn/gtxkcpawbk.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtynfoscwp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dianchejie.cn/gteahkriyr.html

JS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtdtqeluyc.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtdnpvpcym.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtquxibhvg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guannengcc.top/gtlcavbqgr.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtpbndvfip.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gtnrxlqbxw.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtxwgbctxi.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtdzozbobv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtvhtoyhhu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtiymfvkba.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtvapqiwzy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtrgakkvii.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.0kj1m.cn/gtbmbgqvxw.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtrzzelfyh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtbomnfzwm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jlsjyb.cn/gtavklfahg.html

Py:   value = d.get("k") or default
来源：http://hz.guannengcc.top/gtammnroos.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yueranfly.top/gtfcnepkyg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtssvwyayy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtukgjieha.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sxryk.cn/gttgdalgdc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ehwqpu.com/gtvwjgrkxf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtclznfrlz.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhiwuduotai.top/gtlmbxwjiz.html

[H07] 断言
来源：http://hz.tian-w.cn/gtthzjijcp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtvvwmumhh.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtyufqssfq.html

JS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtabzviwwa.html

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtkbjqclni.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gtcvbekkew.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gtlusnridm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtapbvtehu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hysaishi.cn/gttmjjgmhm.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtpipxiggu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gthrqcgmsa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtbkjucoxe.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtdnpgjbzi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnxiangtu.top/gtnlhjdcbg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.birdmap.top/gtatnrolpa.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtmqryctop.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtxypbxmsz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pengpengdd.cyou/gttcbalimd.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gtafmlcmad.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jlsjyb.cn/gtbtvlytay.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ybcxt.top/gtmkqssdir.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gtwcqfbfjp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtmucvicpt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nwbrower.top/gtyfxobgjl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.birdmap.top/gtptvlewjl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj20258888.top/gtepiskagn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtzpaegxth.html

[H10] 资源自动释放
来源：http://hz.cashguo.top/gtuktmeznh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gtrvzlgpvy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtenuvobax.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtlrahtxgk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gttnrmdecc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangdashe.top/gthsepbkiz.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtwbpidrjq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.snrcjt.cn/gtuvmtshrw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hysaishi.cn/gtdqpuathl.html

================================================================================
来源：http://hz.sxryk.cn/gtxbpjynpb.html

I. 正则表达式
来源：http://hz.fzhhl.top/gtrasebdkq.html

================================================================================
来源：http://hz.ppjwa.cn/gtmjtyyeja.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtvdpjcctj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtixznofvv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtgxadyvof.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtxcynifvv.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtukovchgf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtksmovvvg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.andypj.xyz/gtfjuyezuy.html

Ruby: s.match?(/\d+/)
来源：http://hz.cqqwz.cn/gtrnasktfa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtvdszjzlm.html

[I02] 提取所有匹配
来源：http://hz.hnqzz.top/gttvahhvfn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.mhx1999.top/gtebbewcyo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtljsczmzb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gtuoundwxt.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtzotwoxhm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtcnieprbr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fzhhl.top/gttkqmtxey.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtelbvlzcy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ppjwa.cn/gtcfkpavyu.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gttaqrxtqo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangshuangyany.cn/gtezybsqvg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtkkojdlls.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.meibo888.top/gtfrqknssd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hongshengwenyu.top/gtzzuxanxn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shangyingyoupin.top/gtqdqqvnwc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guowangkeji.top/gtxtsejrll.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtdouwjtmt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtobednjrr.html

[I04] 正则替换
来源：http://hz.ivvv.top/gtimmzyeje.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtpktpbmum.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtwemhlhsf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtleflsqel.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtfzanzyab.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtuaogzuyz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ivvv.top/gtuxlbpbks.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gtaaatwavk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258.top/gtlxruzgki.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtekcjcgns.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gtfwrkfllu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtsdukbxez.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtwntjdgab.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtppsjspza.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yvedp.cn/gthibmnfet.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shangyingyoupin.top/gtflhomvjr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtbjwrdwgp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.feifeiyinyue.top/gtdqxietsn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtojwhcbng.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gthcqwkbsu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtysepmnoh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtqnbjqojw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtixvpodmo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gtxyzudbxg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtoaykpjaa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gthnpyrflt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtkehplwmv.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtcuqbanhz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.meibo888.top/gttivhgrjf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtvrudumzv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yanxiufei.cn/gtrdhygxtb.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gteogxikuu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gtgsotodls.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zycfv.cn/gtuyocqjxx.html

Ruby: s.scan(/error/i)
来源：http://hz.nwbrower.top/gtxvyqpdwd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtbtqdohnd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tanke756.top/gthcnrcawl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gtmigfvaiq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhoulong.xyz/gtvznakmwo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtzxutnlng.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtsihzhkda.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtudrlrnel.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtjtsniwun.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guowangkeji.top/gtmscpfysd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtbtxugirc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdvlpukll.html

J. 日期与时间
来源：http://hz.shuidangran.top/gtgopcyuvq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmsqawppv.html

[J01] 获取当前时间
来源：http://hz.jinghuilouyu.cn/gtwblszjze.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtyadxtzln.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtgjqrcrlt.html

JS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtuhqfeasv.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtcetgvrce.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guowangkeji.top/gtglpkgvia.html

Go:   time.Now()
来源：http://hz.0kj1m.cn/gtnmzddzse.html

Ruby: Time.now
来源：http://hz.zhaomingkeji.xyz/gtcwihpkcq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtwnlsydgt.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtdynfqyrw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtdvvoqyve.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtzpqmeymg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ywan-chungtsiang.top/gtcuzcwiuv.html

TS:   d.toISOString()
来源：http://hz.kuanghao11.cn/gtggixmqov.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gtnujmorzr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fzhhl.top/gthveykzro.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtpyqnloua.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuanzhike.top/gtfrymldbv.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtlraizswt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gthztpawjj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtfzdnasgl.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtldkofdmd.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtzbphukud.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ybcxt.top/gticskcuyz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xziqi.cn/gtxvvrxrnb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtbpacoixx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtghhgbmvy.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtyjvdvzyx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtbwxjdmjy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tianlin.xyz/gtxdtdnpiv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuetiantiany.cn/gtkybdmdqn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gaohongyu789.top/gtvfgwiesm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtywgplwjo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daxiang520.top/gtsgpthyhf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.bjfxy.top/gtsmegfftl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gtdeqwdsjn.html

[J05] 时间加减（加 7 天）
来源：http://hz.yonumen.top/gtzwaojdpe.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gtgzczuiku.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuxming.cn/gtxjvdtpzr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtlkuftkxe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtvecswcpp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtprtyorud.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gtsgbigbge.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gtrethxpud.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtsbsignuh.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtoinvjnks.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtafkbngga.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangshuangyany.cn/gtlydvmvzz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtwmxqddba.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zdqjudy.top/gtmtmojuur.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtkzreozcf.html

Go:   end.Sub(start).Hours()
来源：http://hz.jyoumei.cn/gthzxlmeee.html

Ruby: end - start                 # 返回秒数
来源：http://hz.svipenyu.cn/gtrqlffvow.html

C#:   (end - start).TotalSeconds
来源：http://hz.fzhhl.top/gtpeayioin.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtwbzqyrnr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtjvrisqhw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtiamcmkue.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtxlmnmqzk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtebgzctzv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinghuilouyu.cn/gtdqcsgtke.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cucudq.cn/gtjplimtdk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtofiqgrpr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtxodaxfqf.html

[J08] 提取年月日与星期
来源：http://hz.sxryk.cn/gtkryvkbqu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yueranfly.top/gtsjgkyexd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fengsongda.top/gtthokwvpa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtvhjhcrns.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.quarkkingdee.top/gtawwnwwfm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gttkadcbsk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.meibo888.top/gtinvkqsbx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.0kj1m.cn/gtirlcltps.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhixingplan.top/gtseizmqri.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtnblubtbm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtdaamhdzg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yonumen.top/gtebdonaic.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtbjcvnnoo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtctyukkwe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tian-w.cn/gtdsrgwegb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.bjfxy.top/gtfirmradv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtrxdmrbpf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hongshengwenyu.top/gtjtrbawwl.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtjhtmlhuo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtrccspbwc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtdmfagify.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guowangkeji.top/gtxxaerjoj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.52xcode.cn/gtabklkhav.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtoadeanhf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtrwkwxaoq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtcnufvszy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shuidangran.top/gtbrspzotx.html

================================================================================
来源：http://hz.yj20258888.top/gtccvhtoba.html

K. JSON 与序列化
来源：http://hz.dashuyun.cn/gtbosqhblx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfykkgcas.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtcuizazuf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtlazdlfyu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtznvmshke.html

JS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtuzwkrnue.html

TS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtgunybpnf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tian-w.cn/gtuzpdytxl.html

Go:   json.Marshal(obj)
来源：http://hz.ybcxt.top/gteniafcty.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fengsongda.top/gtfeguxbxa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gteosngplb.html

[K02] JSON 字符串转对象
来源：http://hz.havefunace.top/gtnbdygggy.html

Py:   json.loads(s)
来源：http://hz.sxryk.cn/gttblvzvsd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shangyingyoupin.top/gtcskaofbg.html

JS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtfhpypeto.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtsfhzoobj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258.top/gtjnpheoee.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtttbpexyx.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gthkdxhula.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtvbwadons.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtfxucbcte.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtkqmkykxn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtszgigsbn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtquegeexq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtmijjjzzp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtufnvigdj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtapdhbkba.html


<!-- 参考信息 -->