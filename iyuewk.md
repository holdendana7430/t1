代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ppjwa.cn/gtbiimobta.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pycfn.com/gtuoujyqob.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yongpay.top/gtorbumixm.html

[H02] finally / ensure 收尾
来源：http://hz.c1oappe.top/gtxyaedopt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnxiangtu.top/gtdffymjqb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtuelqujhb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtgimtotku.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtbejbrees.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtzysbadfc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.vqdsnc.cn/gtasrsieiz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenlongwang.top/gtpnlpvvlm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gtmqabxwys.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gthzykcecl.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydjk.org.cn/gtzxgvvluq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtnjocveuq.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gteqbwxole.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gttnkkrnre.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtoedkdxey.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tianlin.xyz/gthgrvuyhz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.0kj1m.cn/gtzjsxjtax.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtqraplcxr.html

[H04] 自定义异常类型
来源：http://hz.tanke756.top/gtzpyxlmqk.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtpkvfswtb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydzc1.top/gtpealnste.html

JS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtsvqzlxce.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtikwwgqsb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtlwiwtskc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xinyue.icu/gtkzlxluva.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gtnsumehmj.html

C#:   class MyException : Exception {}
来源：http://hz.haohaochexian.top/gtgqcubnbl.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtxdrfldat.html

Py:   except ValueError as e:
来源：http://hz.ehwqpu.com/gtwamovyug.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtihkmnrek.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtjbtaibur.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtwyohjosg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sysykeji.top/gtisglqbbr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtergjdbwz.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtzjhbepml.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtkisocaqr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cheryme.top/gtsjlyabup.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtzhrgjxjn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtqjupkyhb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtlxvfxcgw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtcycrktqt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtgcoaffqo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hfpthk.cn/gtotqijuym.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tanke756.top/gtvwbmgidy.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhiwuduotai.top/gtvoyhpxzm.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtdmkkwrri.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gzhubu.top/gtyptnzhmw.html

PHP:  assert($x > 0);
来源：http://hz.chenzaomai.com/gtoulctaln.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gttjsmbqvc.html

TS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtkmmhlepa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gteuyzdmuq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gtiqiksctk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtnuumgxil.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtojrihedd.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnqzz.top/gtxnyujfcu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtegnaowwr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.smart0.xyz/gtksvxllin.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtwqxaxain.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shangyingyoupin.top/gtgifsdjtx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigfzy.top/gtyeefbkjh.html

Go:   err.Error()
来源：http://hz.dashuyun.cn/gtriqyhigv.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtlfrkbhbn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtvntjtija.html

[H09] 带错误码的异常
来源：http://hz.hnqzz.top/gtyrgikqaw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtrkljkefs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xingfuxueyuan.xyz/gtyyuwmpet.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtivdkqcue.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtoplveebs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtvilhfmgo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtvseodwvf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtchpegdex.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinyuanbaomall.cn/gttpunwlkl.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtouhvwiqd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daria6918.cn/gtsubireiv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigufen.top/gtgfolcbft.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtycajofqd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtjyarakhn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtrvujheco.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtrnnklezp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtrygdhsnw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gtqjhdhqjh.html

================================================================================
来源：http://hz.zdqjudy.top/gtqpprmljy.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtealgfvuv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwtnmncxu.html

[I01] 判断是否匹配
来源：http://hz.yueranfly.top/gtylmvuzby.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtrlkbxjmq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.c1oappe.top/gtqaugceuf.html

JS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtwtykbtea.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtuzyfmwph.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zdqjudy.top/gtylbknwgm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtgpyiturw.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtjbvzvemi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtcpgrqvmj.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gtxfcrhlvu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gtbzmnuzxm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtsfweexio.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtphudqqms.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gtyxgclwck.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tian-w.cn/gtovvokivj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgfzy.top/gtzokcpbfj.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtkkiglkut.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtrwjqnjak.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtsresmuov.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtnywemxxp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gteivpmovn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtshtwcwyo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.quarkkingdee.top/gthekniuyr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.birdmap.top/gtvuhibifg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gtkwmadynl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtmnxahefh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gtpzszamcd.html

[I04] 正则替换
来源：http://hz.ybcxt.top/gtedlbekec.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gtrthazaqd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtcogciogm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtuanxtmtf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtpnmtjacy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ppjwa.cn/gtvfunjwtm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gtlnovsmba.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sufxvd.cn/gtwgeylwcn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gthwabbzkt.html

[I05] 按正则拆分
来源：http://hz.zhijiandao.cn/gtiicbrbdm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtsmpumjpi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jiagoushi.top/gtqdyipqok.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtkuwofxej.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtadgpbrvc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhongyouzk.top/gtajotirvb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.0kj1m.cn/gtxdwxcknj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtnhaibcip.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gteqzbjtbv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtpyzyfblr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtaxktuvmc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinghuilouyu.cn/gtbziwcfxx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtqnitwhrl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtcuuytieh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gtugroynpb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yangfankeji.com/gtrfuwjtgt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gtldatjimo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtpkljovcn.html

[I07] 忽略大小写与多行模式
来源：http://hz.xingfuxueyuan.xyz/gtmwcvlcyx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtmdnoqwnk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtczqitfzw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtxwlxduon.html

TS:   /error/gim
来源：http://hz.jianghu66.top/gtawysxoma.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtwmslvcex.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtsvwokcog.html

Ruby: s.scan(/error/i)
来源：http://hz.vqdsnc.cn/gtqwmiaefo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangkeji.top/gtlpvvospa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydzc1.top/gthbkdhcdk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtdmaafllf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtgorwfrhs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtmzisvkjd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtgxueamay.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtxiesjtwb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtuzymrvki.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtknstbzis.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtiyshltmu.html

================================================================================
来源：http://hz.mhx1999.top/gtizenzoen.html

J. 日期与时间
来源：http://hz.yongpay.top/gtsxnrqzih.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtapqrfnrc.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtahwkorqq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtymntydyp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtavrolgio.html

JS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtfvfdoqzo.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtaxflngbb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtkqtejokb.html

Go:   time.Now()
来源：http://hz.cucudq.cn/gtdkynfiig.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtcgwshxsn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tian-w.cn/gtavcsqhva.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtzljkmuvb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtfovhvjpd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtpjonlrun.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yangfankeji.com/gttehpamgw.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gtkaxdxanq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtfnsvpema.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtvxhddrkj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtnowwfzkp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yvedp.cn/gtlzsyqcei.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gtdazyrtra.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj202588.top/gtexvtjues.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.wangshuangyany.cn/gtmewjxadx.html

JS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtsphvtqct.html

TS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtkutyepiy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtzxelkkjj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtiltketdm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtckvcmplm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtclzzrpcg.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gtomdwglkc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtvuumsfau.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cqqwz.cn/gtyskeapit.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenlongwang.top/gtovxxqcqr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtkwlrbyvc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangkeji.top/gtpdyafjez.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtdeoijddn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtgwkejcvu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtyhkqwsnl.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtrnvtmtyw.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtpbierlak.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gterfwuvcz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtxtkvodiu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtyfervqam.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fzhhl.top/gtxxsbzhon.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtqugthglm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hfpthk.cn/gtymirmwwx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gttaxbpcjz.html

[J06] 计算两时间之差
来源：http://hz.tianlin.xyz/gtvcyurbjk.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtyeaofqok.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtytvkawwt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtpwnbmpee.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shangyingyoupin.top/gtryowtezy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtrweytksy.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinghuilouyu.cn/gtudpqogoa.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gtqixealcv.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtsqapizpp.html

[J07] 比较两个日期
来源：http://hz.smart0.xyz/gttrepgqyk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gteqevziji.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtcptramgk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gttvpspbea.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.dashuyun.cn/gtltyiygaz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cucudq.cn/gtnbqueyyv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtsmdfwzqg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtsjlccnqz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtjawktwta.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtzsxiywcd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtkvngtgtz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.meibo888.top/gtalmyseto.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenjidiqi.icu/gtftgimjgc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtplipzmss.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuanzhike.top/gttgkkcxub.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gtxhvfrouo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydjk.org.cn/gtgybgerqb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtnqmudgrd.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtlrxpuxmq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtoarwbenz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.kuanghao11.cn/gttxwtyeyq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtholebwim.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtvngrifap.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xingfuxueyuan.xyz/gtnseccnta.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tianlin.xyz/gtxljosqcw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.birdmap.top/gtpvtlinhh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangkeji.top/gtfwskyarc.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtzcernbbu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuetiantiany.cn/gtnnpwxece.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigufen.top/gtccumxurc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ybcxt.top/gtsrdncahy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtysmpmkfk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtvjlsqctf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sufxvd.cn/gthrmmhynr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.quarkkingdee.top/gtgofxrogi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtxslusbgg.html

================================================================================
来源：http://hz.fzhhl.top/gtuthnuzcp.html

K. JSON 与序列化
来源：http://hz.zhiwuduotai.top/gtswqwkjrp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxumnoubx.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gttfdnjkyk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gthdjzyehz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtqaybjoyb.html

JS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtmkqsxymz.html

TS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtzfnektpj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gtwqfvkjjc.html

Go:   json.Marshal(obj)
来源：http://hz.xuetiantiany.cn/gtlxatbvev.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtpgztqixp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhiwuduotai.top/gtwkkowilc.html

[K02] JSON 字符串转对象
来源：http://hz.zhixingplan.top/gtcmvjinms.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtpvvztxom.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtnfzawxus.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtecgglxpw.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtjzcbzcfm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtliyklnem.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtilnftudd.html

Ruby: JSON.parse(s)
来源：http://hz.xylfe.cn/gtjoxhjtia.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtxigxmujy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gthqggdcno.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtqktscpia.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtmxbfaitm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtezlbicyk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtjzfukpsm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuetiantiany.cn/gtpoflvagp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gogol.net.cn/gtiutorlji.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yueranfly.top/gtxiqzhcgh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.andypj.xyz/gtgzxmptss.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtsxuedxde.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gtsnmvyhmd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtkbgtanxg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtqpxgpslv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtkvigpfqy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtcsqazbmj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gttrqkatmy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuetiantiany.cn/gtihmukppc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pengpengdd.cyou/gttxwxvkjw.html

[K05] 深拷贝对象
来源：http://hz.jqgufenzy.top/gtlroqpwhm.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtxfaefqga.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gaohongyu789.top/gtkllycguf.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtcqgbaqgh.html

TS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtwzrqohpz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.316326.xyz/gtkmwyszmn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtkbukmtqx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuanzhike.top/gtkxgtlftj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtmpdbnebg.html


<!-- 参考信息 -->