代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtxwdssfie.html

JS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtytkrujid.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtectgluyr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.kuanghao11.cn/gtsijyceta.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtvfdovmwb.html

Ruby: obj.instance_variables
来源：http://hz.zhiwuduotai.top/gtoicoiwhg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shangyingyoupin.top/gtwqjubjhj.html

================================================================================
来源：http://hz.pycfn.com/gtyflyvhqj.html

H. 异常与错误处理
来源：http://hz.quarkkingdee.top/gtihnwphmk.html

================================================================================
来源：http://hz.yongpay.top/gtigfgpbot.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtuwmymxxk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtbohjljrj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtxugakjon.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydzc1.top/gtyirlhxum.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtdjvrvmqn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gtugphkcet.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gtizjotyio.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtgnrsgedi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xinyue.icu/gtggufghbb.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtglkuljhq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gtwkohjhyv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtbzjoyayr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtbshiykli.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtjlxpmrma.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtntcwdddd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gtvtynpoom.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtkarcfbaq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nwbrower.top/gtjpghehsv.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gttzfzqxhl.html

Py:   raise ValueError("错误信息")
来源：http://hz.redwolf501.top/gtxlnslbuc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtrdfnrkro.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtaqvdcoje.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtanpzujxi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtmrpatuwp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtnlmvmcmx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.andypj.xyz/gtvdoqiuku.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtetkjoykh.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtcjuoxrgs.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtlzmgwnki.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxinkj.top/gthzhqwrwf.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtxhhgrkij.html

TS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtnenqawkm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gtsntkjhvs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtyuqvcrbe.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtxitnhjtm.html

C#:   class MyException : Exception {}
来源：http://hz.c1oappe.top/gtfimosbil.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtdiihzuzz.html

Py:   except ValueError as e:
来源：http://hz.yonumen.top/gtwtgwcsie.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtygpltbtc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtifazgvra.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtmvbuffct.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shangyingyoupin.top/gtkavrgbgx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ehwqpu.com/gtpwptexvj.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtfdoxcici.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtzmzyrhma.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtrbxczqhv.html

Py:   value = d.get("k") or default
来源：http://hz.yvedp.cn/gtsgvbjifk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtusdsmmkt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtcbmwnvmx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtganhyhyb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.dashuyun.cn/gtbyjahrsc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtcejfpzra.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yonumen.top/gthkpqavnm.html

C#:   obj?.A?.B ?? default
来源：http://hz.ywan-chungtsiang.top/gtndjooyyr.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtykjgachj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtsrjggmce.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtjwnmtiuh.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtdwmeilvb.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtnqvjpsqw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtjajufobv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cheryme.top/gtlkzzahyl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sysykeji.top/gtqblvojef.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtxgqtplnn.html

[H08] 获取错误信息与堆栈
来源：http://hz.haohaochexian.top/gtbjduhapc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtgkhdeckj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangkeji.top/gtxjzuhlgr.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtjmhznnis.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xylfe.cn/gtmxrgyfiq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gtwlugdytv.html

Go:   err.Error()
来源：http://hz.daria6918.cn/gtjokcirin.html

Ruby: e.message;  e.backtrace
来源：http://hz.hammf.cn/gtuxncwutf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yvedp.cn/gtkoyveyma.html

[H09] 带错误码的异常
来源：http://hz.iojbl.cn/gtlbwgvnzi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtfjzaywbn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtxlhmuvck.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gthpxbwcsb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtapbxdtxz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.wangshuangyany.cn/gtavsajcsr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgufenzy.top/gtwjccowex.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yongpay.top/gtyapqyqpm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daria6918.cn/gtrujkzcel.html

[H10] 资源自动释放
来源：http://hz.yonumen.top/gtzyiwajor.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtrtqwlnwo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtgaexnkac.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtgehroktj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtocjehetw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yonumen.top/gtdyheupyc.html

Go:   defer f.Close()
来源：http://hz.zycfv.cn/gtoaqvzvzr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtjyopfhcs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtyjhzcvuq.html

================================================================================
来源：http://hz.guowangkeji.top/gtgbgdzxcr.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtsdwfbvdy.html

================================================================================
来源：http://hz.yvedp.cn/gtxuzaqyno.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gteebeoozs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yongpay.top/gtwqpougzg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtbffkbrte.html

JS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gttpfrzled.html

TS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtlhsxnrfz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtxaknevno.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.redwolf501.top/gtmdnrbkje.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtsdxxcovq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydzc1.top/gtrjgpzrke.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtopqvrwlb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtzuhoscmu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tian-w.cn/gtusyeofmw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtwcuoztce.html

TS:   s.match(/\d+/g)
来源：http://hz.shuidangran.top/gtsrkuobiv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dashuyun.cn/gttyuwayob.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtgjmgawxv.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtwrskecel.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gtdihrusht.html

[I03] 提取捕获分组
来源：http://hz.hnqzz.top/gthueusuos.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtcrjkrljk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nwbrower.top/gtvubpzeig.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daria6918.cn/gticepazaa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xylfe.cn/gtsnywgmho.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtobrcvsmw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zycfv.cn/gtxzrhqxiy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtuxpielsl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gtiiccgjii.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtksmnohck.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.316326.xyz/gtltkfpazq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gaohongyu789.top/gtcrnwtbor.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtypfirxvd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtlaiycytf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yvedp.cn/gtyaipqgfo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtcudylych.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtxklshfkl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gtxeiqesaq.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtwtutnpid.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sweek.top/gtorhavtbe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtfhvgsfov.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtnalwytmc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtanwguivc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtrjdynwbp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinghuilouyu.cn/gtkgannoih.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtgjpaubqv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtyfwynjzx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtpqnuufdm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtzjeprjgi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtfmgmwlqx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtyvqhkcum.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtipookerl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tanke756.top/gtjkbnkwjr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtmarvmfkv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.iojbl.cn/gtzpgilzvv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gttkhrymli.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtikwelbtg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yangfankeji.com/gtriynlsly.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.svipenyu.cn/gtqppltnnv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jyoumei.cn/gtyobzxxst.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtnotpffki.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tian-w.cn/gtkasawvdc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gtbyrocvbp.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gthbpwfjmt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtdbufbgce.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtpznupuxa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gthnrhcuzb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuxming.cn/gtcwgkkmqi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gtakxnfmnv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtaqhwqlwm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtkfcfsuok.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gtilisnghf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtnfjphymx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtqsorovtp.html

================================================================================
来源：http://hz.yuxming.cn/gtnwjequra.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtvqiijhns.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtiatagdcy.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtfsttubej.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.kuanghao11.cn/gtoxeerzcg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtphgznmzq.html

JS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtpczkxctc.html

TS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtidjqlyjp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtxvwcqcou.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gtxrtnunrs.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gttmbflkwd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtcvfbpthr.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtthctbpok.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtplxiguxq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtofgpmyrr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yangfankeji.com/gtjmluqfgy.html

TS:   d.toISOString()
来源：http://hz.cucudq.cn/gtcmdnogww.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gtgwgtjlgn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtvjzduvyr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtqmspeijd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtophyxwzd.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtsfjcutbw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydjk.org.cn/gtrhoxybpy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtxscpgfye.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtdhnuudhy.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtrxfbofys.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtzjxephay.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtmhwgnvrq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gttnpwoamb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtssxtjztc.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gtwxwhgwjy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aizwys.cn/gtuxpjttjv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtdbrydtqw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtjkixdqfx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhaomingkeji.xyz/gtxwafkdbd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aizwys.cn/gtvnhkzibz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtcaagasnk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shuidangran.top/gtwuwnfvzl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtqylifzzb.html

[J05] 时间加减（加 7 天）
来源：http://hz.quarkkingdee.top/gtzqtpbmqf.html

Py:   now + timedelta(days=7)
来源：http://hz.cqqwz.cn/gtzoenymxu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dashuyun.cn/gtioqosotn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtzxakpjng.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtdpskztho.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinyuanbaomall.cn/gtskdlwmjn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtqrcmdraf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gthycblwdq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtvxnmdogt.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtfylixgqo.html

Py:   (end - start).total_seconds()
来源：http://hz.chenjidiqi.icu/gtaakbggbg.html

PHP:  $end->diff($start)->days;
来源：http://hz.hongshengwenyu.top/gtddxrvzln.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtqexfqviq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtftfztibh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtjvsfpqnu.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtmbjornec.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgfzy.top/gtbytcraal.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gtgyitzpui.html

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtuttpubjs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtrvyohdtn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.meibo888.top/gtejbocrgj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gtdplwbuio.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtkmsyghem.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ywan-chungtsiang.top/gttlnctpuv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtztmtcqby.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtkxnhepnb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtdlbzrqtw.html

[J08] 提取年月日与星期
来源：http://hz.yj20258.top/gtuyyzugqo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtdbldqppz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtemiybdfu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtpmwkmrod.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pengpengdd.cyou/gtechjjpol.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jiagoushi.top/gtuldaxqns.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj202588.top/gtgaevsekt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtymocoupw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtvtgucfrc.html

[J09] 时区处理
来源：http://hz.0kj1m.cn/gtpicmiped.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jyoumei.cn/gtmfjndatn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.iojbl.cn/gtafqbxhgs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gthrbcmenn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtqckgqmpz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jiagoushi.top/gtzvgroqqx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.haohaochexian.top/gtryvilgub.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtqmdnpsdf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gtnuszshyd.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtxuoopicb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtcrcrzgcm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtzsnukilh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgufenzy.top/gtjzimfbam.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtfukbyjvo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gttnxiqmqq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtvatjvvxg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gtevtbasuj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtokvlsobm.html

================================================================================
来源：http://hz.52xcode.cn/gtzytwjlyl.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtdtjdrkeo.html

================================================================================
来源：http://hz.zhijiandao.cn/gtapoqjhen.html

[K01] 对象转 JSON 字符串
来源：http://hz.aibaodan.cn/gtdcsvavvh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtuehsvpyb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtyfgkiedg.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtoatogveq.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtwrvwmfcd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtduwaqsuj.html

Go:   json.Marshal(obj)
来源：http://hz.daxiang520.top/gtswnwejgn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtxfwbbjri.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenlongwang.top/gtwmvmcodb.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtcvqeloqs.html

Py:   json.loads(s)
来源：http://hz.0kj1m.cn/gtllsqoeev.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtfkeowwqz.html

JS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtcohmedaa.html

TS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtxjgecdvp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gthlyjuwvb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtpxifsjyj.html

Ruby: JSON.parse(s)
来源：http://hz.ppjwa.cn/gtmizbqoxl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtqsnbqlhc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnqzz.top/gtxxgixpxs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtsylrchea.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtexldvkkf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ivvv.top/gtoljalkoo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtqhodllpo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gtwajpeigr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtiwwhuelh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtadquekco.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yueranfly.top/gtbrevrvpi.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtihwlrbbm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtquvorkpj.html


<!-- 参考信息 -->