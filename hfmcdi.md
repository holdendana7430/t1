代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtkanezhhg.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gtmdgvixxv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.redwolf501.top/gtdolzfcuq.html

================================================================================
来源：http://hz.hysaishi.cn/gtnpkraryu.html

H. 异常与错误处理
来源：http://hz.ehwqpu.com/gtxqotoekg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtjrleeevc.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtfqucldws.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtivspwiix.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yueranfly.top/gtovntpxcd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtnhsstgwa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtoolkhghm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shzxlz.cn/gtfwipplqv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtighmnwet.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtyrilcqyx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtsdcfzoex.html

[H02] finally / ensure 收尾
来源：http://hz.aizwys.cn/gtknindyer.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtjyavjyjk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtrgovqsme.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtlonikysw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtzgzdzama.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtpgurzhug.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gtiywknyye.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daxiang520.top/gtsdghhjac.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jlsjyb.cn/gtwtqchblw.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtrgxmhvbw.html

Py:   raise ValueError("错误信息")
来源：http://hz.hongshengwenyu.top/gtvnhmljct.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtsbyeoimr.html

JS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gttphwinmp.html

TS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtpksrsvjy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtqhuamvjo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtlxtygvat.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigufen.top/gtcwtgqftq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtbxvgbiid.html

[H04] 自定义异常类型
来源：http://hz.c1oappe.top/gtfedkpikq.html

Py:   class MyError(Exception): pass
来源：http://hz.sxryk.cn/gtxueysubc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtvuxmihnw.html

JS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtlivnasgz.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtwmnuqjag.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gtrdikqfzg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtryqhwmpo.html

Ruby: class MyError < StandardError; end
来源：http://hz.zycfv.cn/gtpakibsbm.html

C#:   class MyException : Exception {}
来源：http://hz.52xcode.cn/gttjnokvxz.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtgtyijzka.html

Py:   except ValueError as e:
来源：http://hz.sxryk.cn/gtwbbtbgun.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sysykeji.top/gtksydqqoy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtyclizoii.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtfhoaivrz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hongshengwenyu.top/gtiorsxdwt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtblntziwu.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtabkgnthn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gteuywjemz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gtgqlmfuzx.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtmrtgncom.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtzjcfrpox.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gttazesnnb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtyopnjmga.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.snrcjt.cn/gteqgiusrt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gtsjxjdbhs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zdqjudy.top/gttiichlxm.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtkenzdzuc.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtguhehvco.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtnfoufzld.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtlksugcpz.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtqludwxor.html

TS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtqythenyn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuanzhike.top/gtevdgyezn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yvedp.cn/gtsgglsenw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtlzmrkebe.html

C#:   Debug.Assert(x > 0);
来源：http://hz.meibo888.top/gtcwidhvat.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtiwzlunqi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shuidangran.top/gtwsmitbye.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtuwuigoeg.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtioazxiki.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gthfpddvri.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtkiwwgvzu.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gttqikywzn.html

Ruby: e.message;  e.backtrace
来源：http://hz.smart0.xyz/gtdarziibj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.haohaochexian.top/gtjbosrlmt.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtwguxqrbu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydjk.org.cn/gtabqotwnp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtcupeserr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtzesuhbxs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hammf.cn/gtfietqbht.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pengpengdd.cyou/gtzeiegfal.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtkveqppuu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jiagoushi.top/gtrjyovqwz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.quarkkingdee.top/gtitlipdgo.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gteontrdew.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ybcxt.top/gtphzzhqoq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gtqnpfigob.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtzogjxuhj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtrwtwmmyo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hfpthk.cn/gtaeipkpiw.html

Go:   defer f.Close()
来源：http://hz.aibaodan.cn/gtltxkakny.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cheryme.top/gthzhsfrwr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtlebohubh.html

================================================================================
来源：http://hz.yuxming.cn/gthaonvpah.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtjcvgzqqf.html

================================================================================
来源：http://hz.andypj.xyz/gtemtgqpxa.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtszmdkmsb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtqftsmtso.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtokizenow.html

JS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtmccmdzsf.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtboaltfxr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daxiang520.top/gtazshiblp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj202588.top/gtegpkudhl.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtmuwdgadz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtqbkxpohh.html

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gtabiqvqob.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtommneanr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yvedp.cn/gtvnpcxftv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.smart0.xyz/gtpnscowsl.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtrtxtkgsl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangkeji.top/gtmgwvaamo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhengqikj.top/gtfpfoarvg.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gtlfsyzpni.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhijiandao.cn/gtmtkmriiy.html

[I03] 提取捕获分组
来源：http://hz.quarkkingdee.top/gtiffjvyea.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtvlehvkqk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtnkqbmpee.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ywan-chungtsiang.top/gtlbvawlrp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gteouyncur.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtrryxhijx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sxryk.cn/gtjalglwwo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.meibo888.top/gtzdwmrjur.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daxiang520.top/gthjxzdagx.html

[I04] 正则替换
来源：http://hz.aibaodan.cn/gtpkgpglgb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gtahlfneas.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xingfuxueyuan.xyz/gtrdavnebv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtabglkvmv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtembdwpnx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtjarweusd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtyyatofgz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gtdyaevxfe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dianchejie.cn/gtceudlpjb.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtprjbrvxb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtjmvbhalr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gttmxqufsx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtkelwqzwq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtezyvtgrw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gtvrulqdyv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gttijokavj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtonxbidhy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtxtkmkssv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydjk.org.cn/gttaxnfdic.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtgwzrlgnt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gtwemkomel.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtebaupvvu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gthaukbqom.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gtzlarjclq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtjnshzbyk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtpmpewbie.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtpseauijd.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuetiantiany.cn/gturefltpt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.snrcjt.cn/gtxizljgsg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtgjpwzncu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenzaomai.com/gtecrhboxd.html

TS:   /error/gim
来源：http://hz.nanxinkj.top/gtpwgmilkg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtlffhpccd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xylfe.cn/gtegwpdakk.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gtpfrwqsiy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtrvhewdsi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtttmhqmyl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aibaodan.cn/gticzkysba.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtzmwfgsgs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtbcoivqkf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtepzpcpxf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cucudq.cn/gtixujromq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xingfuxueyuan.xyz/gtftgtkljs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenlongwang.top/gtmadxnush.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtadptdwii.html

================================================================================
来源：http://hz.gzhubu.top/gtkfpwhtnt.html

J. 日期与时间
来源：http://hz.c1oappe.top/gtpzpvsbhm.html

================================================================================
来源：http://hz.yj20258888.top/gtjbmocstx.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gtshudogmi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shangyingyoupin.top/gtbemffvkj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtpxjvhfiy.html

JS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtfckuxlct.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtmefdoess.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtimhnttyl.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtjaqoutmd.html

Ruby: Time.now
来源：http://hz.yuanzhike.top/gtuclauiph.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dashuyun.cn/gtpwlrztsi.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtqwllprsq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtklzlwgnb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtlxabjqtk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yueranfly.top/gtspllgdya.html

TS:   d.toISOString()
来源：http://hz.shzxlz.cn/gtzqrckftf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yongpay.top/gtcqscyait.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtjojotcph.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtlldyuskj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gtmlxbibtw.html

[J03] 字符串解析为日期
来源：http://hz.hysaishi.cn/gtpdwmerhn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtylvoikmf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jiagoushi.top/gthfzqofxj.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gteyyvwdix.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtptkyzzcp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtaasipjkk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtlopbrvfj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtjgmbwjhj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tian-w.cn/gtxbwilysu.html

[J04] 时间戳与日期互转
来源：http://hz.chenzaomai.com/gtijtkladm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gtemcvgens.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hfpthk.cn/gtdbpknjbv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtrusavadk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtlqrqdtkz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtpniohyjr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtsijrqtez.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtwbnpbinc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtlrpfvzir.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gtfzaujdia.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtkxmdhqhl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pengpengdd.cyou/gtyswhiuxp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtcnchbrxd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtdgfberel.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtvjqvwvtc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtpzhfgisj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtmuzyljfe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtevxksqde.html

[J06] 计算两时间之差
来源：http://hz.gotoacloud.top/gtckxyprdp.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtzdxhypor.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtwahtczuv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yonumen.top/gthjdqajot.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aibaodan.cn/gtoxnidwwv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigfzy.top/gtwziwipxp.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gthwtlyuap.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtocseprej.html

C#:   (end - start).TotalSeconds
来源：http://hz.bjfxy.top/gtzgwylykf.html

[J07] 比较两个日期
来源：http://hz.yj20258888.top/gtcltbkvan.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtdkxsdabk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtvtyjgpys.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtndhuzmco.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtuegubbel.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtdkowropz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtufesptxv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtijlaurlp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtwcqshmrd.html

[J08] 提取年月日与星期
来源：http://hz.vqdsnc.cn/gtvzcklboc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangdashe.top/gtahfghogs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtjqojpdky.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtwjtjaimb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtkanuooaf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtmhguttfb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtoacaicyr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtilbslbqk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtfzbueoal.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtzqabtesc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtmfkpsvtk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hfpthk.cn/gtfbbcpocw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtbezdjxvi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtvmijaque.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shuidangran.top/gtfhylzwma.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtwddophkc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gtketfoxlf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtdiaofndz.html

[J10] 取今天 / 本月第一天
来源：http://hz.shuidangran.top/gtzmncyzpe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ppjwa.cn/gtevtgatlq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gteebvzmna.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtzwpvegsw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtmurlgclf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtcsilsxew.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.c1oappe.top/gtygoczbsi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtcwghyhpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinyuanbaomall.cn/gtzfwqoqli.html

================================================================================
来源：http://hz.ybcxt.top/gtumbrkrir.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtfppsgsco.html

================================================================================
来源：http://hz.haohaochexian.top/gtgskoecjx.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangdashe.top/gtmovqpehg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtfsmprlcj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtxfclqlxx.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtymeiopvd.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtqyywcpsk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangtech.top/gtubmdcblz.html

Go:   json.Marshal(obj)
来源：http://hz.gotoacloud.top/gtnwysracw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tianlin.xyz/gtgdhnwjvt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yueranfly.top/gtkfztibhe.html

[K02] JSON 字符串转对象
来源：http://hz.haohaochexian.top/gtbvxmmsgo.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtypxnojjg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shangyingyoupin.top/gtpvvvszun.html

JS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gttvfnxuev.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gthfwrnhph.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtxqkvyzzl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtyuqdxnid.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gttwqzpgrv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pengpengdd.cyou/gtboguwvuf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtdguutlik.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gttngvqwbf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtojzowgsm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtviflhfgx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtjvivlfsi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gaohongyu789.top/gtncurxjde.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gtpchdsyjx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhiwuduotai.top/gtalcdhxfx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xziqi.cn/gtxcpcssqo.html

[K04] 读取 JSON 文件
来源：http://hz.gzhubu.top/gtttbzkclp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gttxkilzau.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtwgaqhaxs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtehlmwrns.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtnyextbvq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtdycjsdsc.html


<!-- 参考信息 -->