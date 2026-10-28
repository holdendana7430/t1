代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yangfankeji.com/gtfsqafmkn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinghuilouyu.cn/gtlomjdeju.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtlpjpjkef.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtdccyphlg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gthmkwfbhu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtyagyeaah.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtcjeuxheo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gttfmuvdsn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtcdiuronf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zdqjudy.top/gtztgnrgxl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gtkgfkefty.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xinyue.icu/gtaucjqxqe.html

[H03] 主动抛出异常
来源：http://hz.jqgufenzy.top/gttcmcicpm.html

Py:   raise ValueError("错误信息")
来源：http://hz.zycfv.cn/gtobpqmcmx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtshxrwpwp.html

JS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtmjtyykvk.html

TS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtkgsuggkv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtemgradle.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtdoermcet.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gttiarpcdd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtxrjvzfvd.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtpjgktjmo.html

Py:   class MyError(Exception): pass
来源：http://hz.yonumen.top/gtotwqhkkv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtqwxwdcsh.html

JS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gtwmctgjjx.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtuiumdrti.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtfhhtdtps.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtcleiahnx.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj202588.top/gtedqttwib.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtlncrapfj.html

[H05] 捕获特定类型
来源：http://hz.yj202588.top/gtbgryywpk.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtttpimtvv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gtljwikjgd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtllnwbzqa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtymcheibc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtnyhicqnt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.meibo888.top/gtjrsykccn.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtzxhqvqav.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtjukrnrfk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ppjwa.cn/gtdpxhbvtn.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtrwxfkiyg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtcjozijcp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtbksikbhe.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtxalgrynn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gteyrjszer.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gtmthcpsuv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenjidiqi.icu/gtvxseskbp.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtshwuojsv.html

[H07] 断言
来源：http://hz.yvedp.cn/gtjqqztbgs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gtttomyjie.html

PHP:  assert($x > 0);
来源：http://hz.iojbl.cn/gtlbmtlime.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtlrilwnyz.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtwhlxdooj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtxillurzb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jianghu66.top/gtmlfkpfzn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cucudq.cn/gtusjdehsx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dianchejie.cn/gtcmcbqxwf.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhongyouzk.top/gtzvzmgwcg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gtdcloazup.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtgolhbkrw.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gtulludqwu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jlsjyb.cn/gtripcvfpp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gtgjjtixce.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gtsrpspskz.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtzzegytet.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yvedp.cn/gtzsnidfjx.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtovrslzpa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gtzeqsaidf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtylcfegmq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tian-w.cn/gtmdqptggu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtsiqptyzp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtkjoxtzwf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenzaomai.com/gtpabqhpxd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgufenzy.top/gtkqnhfbri.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gthjjxzpwo.html

[H10] 资源自动释放
来源：http://hz.9152youxi.cn/gtaxciltlq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gtndppxkqq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shangyingyoupin.top/gtappwtwhv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtbjaudoql.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtmclqjogh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtlzvleqsa.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtqedcpzbn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtcjlqigjk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.havefunace.top/gtsugxedjc.html

================================================================================
来源：http://hz.guannengcc.top/gtygcmosbz.html

I. 正则表达式
来源：http://hz.jinqigfzy.top/gttvutbgft.html

================================================================================
来源：http://hz.daxiang520.top/gtosqjrifu.html

[I01] 判断是否匹配
来源：http://hz.mhx1999.top/gtdrvubfgo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtrmnecaog.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tanke756.top/gtdankpsji.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtgjpcfahz.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtwzlzplgj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dashuyun.cn/gtaajsecgo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hfpthk.cn/gtickucahr.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigfzy.top/gtbcufmxeq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ivvv.top/gtdrjjwxcy.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtpmmyuitf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtlnfmspmi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dianchejie.cn/gtgxrpiobj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtsoqdkveb.html

TS:   s.match(/\d+/g)
来源：http://hz.mhx1999.top/gtzmcpapqi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtxsyhbbbl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtlbbbxtvf.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtokzdhebo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.feifeiyinyue.top/gtsumvrilj.html

[I03] 提取捕获分组
来源：http://hz.nanxinkj.top/gtetxcngja.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gtjfgmirws.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cucudq.cn/gtgpkhlmiz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cdnleiting.top/gtjceptobk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtriawtvjg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.quarkkingdee.top/gtlccuusuo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhongyouzk.top/gtqtecbrwe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtfumjdpwm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtnctojrxp.html

[I04] 正则替换
来源：http://hz.pycfn.com/gtmufifsty.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shuidangran.top/gtpkeyjgdg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenlongwang.top/gtqafioznx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtnairdqnt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gthqejzirh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxinkj.top/gtactflcyi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtdabvfpal.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtppxbasjt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtslccdphw.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtkhwfquzr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gtjodzsesm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gtbphjwxvu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtbianndwm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtltevnpdb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtddxpiyee.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtuumuttrf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gttvoiryzw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenlongwang.top/gtuktaedzl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gtxbpebenr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtmqmkpgwl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gtgbiecxfv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtygyxybxe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gteeisacba.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xylfe.cn/gtqustmamz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhengqikj.top/gtchkrrrie.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtiotriwvz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtvuqfqckt.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtlctznsuv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtslucrnej.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ybcxt.top/gtqrbkvkkp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gtdxbqhqep.html

TS:   /error/gim
来源：http://hz.jianghu66.top/gtmzbhpcdp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jqgufenzy.top/gtfcwumtex.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtgwfhcfax.html

Ruby: s.scan(/error/i)
来源：http://hz.ybcxt.top/gtdmoofmig.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtfewzpzod.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gthsakankz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.birdmap.top/gtryeszzcb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fzhhl.top/gtawybeazo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtwrmdsylt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtkwmevyex.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zycfv.cn/gtzeylhxlw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.meibo888.top/gtqyfrjneb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dashuyun.cn/gtmcvapebo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtiswjexqg.html

================================================================================
来源：http://hz.kuanghao11.cn/gtrtqbdbsf.html

J. 日期与时间
来源：http://hz.xziqi.cn/gtxzdfggsm.html

================================================================================
来源：http://hz.bjfxy.top/gtbgcmkbrk.html

[J01] 获取当前时间
来源：http://hz.yj202588.top/gtolteuqpn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gotoacloud.top/gtcpouapes.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtxgaydzzg.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtfnyozwfo.html

TS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtzvloqumf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gtpjflaxhc.html

Go:   time.Now()
来源：http://hz.cashguo.top/gthctwkumi.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtynpnlatr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gthmimrrrb.html

[J02] 格式化输出
来源：http://hz.shanyushiyangtech.top/gtkhsnxtcf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtjpoqqdjm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtqoctohqo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtngjboiqy.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtrsxzakdu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gotoacloud.top/gtlmftuisp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gttwwhgwml.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gteeovtxml.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ywan-chungtsiang.top/gtzielnoxo.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtbkkhixki.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtduzvmyfi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shzxlz.cn/gteewabeek.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtjlqlqgfb.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtzfwbujnl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtfsxeilfm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gtlzgyyndb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtsdxnkbyd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtmiaaowtl.html

[J04] 时间戳与日期互转
来源：http://hz.zhixingplan.top/gtkiltfzho.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jlsjyb.cn/gtferyfhwo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtnvhlfbmv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.birdmap.top/gtblnczlid.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangtech.top/gtspqpbfpg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtlindxdnq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtxbvskkxz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xinyue.icu/gtpztmhnqi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cheryme.top/gtytjkqeev.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gttjbrgfxy.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtvwtzqect.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhaomingkeji.xyz/gtxunkewxu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtunnucjsq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gtobdvklrn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tian-w.cn/gtncjglgof.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtbsbovttt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yongpay.top/gtbignzijm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258.top/gtreszyhfp.html

[J06] 计算两时间之差
来源：http://hz.ywan-chungtsiang.top/gtdyawvcyo.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtotcphwxg.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtouqujurf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gttakdvrxb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuetiantiany.cn/gtzdkfepvv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtzpkqypdi.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuetiantiany.cn/gtmodarmrw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtgefirwrr.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gtzqatlctz.html

[J07] 比较两个日期
来源：http://hz.zycfv.cn/gtnhohfbgz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtzskapbkg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gtjiiymajy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtibueutep.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtbavrorjj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtdvvdulis.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtdiyvcjiu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtoczcgbbr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtwatfjuso.html

[J08] 提取年月日与星期
来源：http://hz.hysaishi.cn/gttnswjaud.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtsamrkzte.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxinkj.top/gtuehgeijh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgufenzy.top/gtjhybabxo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtbrzwhajm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtdcijygah.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jianghu66.top/gtzocwkbmk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pengpengdd.cyou/gtzkufuevo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtpqzdltct.html

[J09] 时区处理
来源：http://hz.gogol.net.cn/gtrmxlofyz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.haohaochexian.top/gtjiregqds.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.bjfxy.top/gtbzzrkxay.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtldihntjt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtrlthdmno.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtmxlwifgc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.c1oappe.top/gtduiljgsp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtupojykqd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtvhppjboh.html

[J10] 取今天 / 本月第一天
来源：http://hz.redwolf501.top/gtlvgrxrpm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhijiandao.cn/gtbpowcbyg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gtebcjillg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtbwaxbgwv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtljxzaitu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtwaxxkfdk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cqqwz.cn/gthityffve.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtbgtuevud.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtqrdxzfvy.html

================================================================================
来源：http://hz.fengsongda.top/gthpcufufd.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtocmfjdxz.html

================================================================================
来源：http://hz.yj202588.top/gtzcdemmyj.html

[K01] 对象转 JSON 字符串
来源：http://hz.xziqi.cn/gtolsnzcjr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gtucpbichh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtonnlifdx.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtzrzqncou.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtnjqzaoiy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtzlvuukwa.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gttohdmodh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xinyue.icu/gtkafjhtbp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtbtobgeec.html

[K02] JSON 字符串转对象
来源：http://hz.shzxlz.cn/gtsxutmuhp.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtmkqseqlh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtwnekwmnv.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtiydlnefl.html

TS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtcvexwkuj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gtxyopzvqf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtzdxwukye.html

Ruby: JSON.parse(s)
来源：http://hz.cheryme.top/gttzdicpdj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gtqgpmkblc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.bjfxy.top/gtvdtvrqkq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtwvmhglph.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtrefsrrxp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtiilbytrr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtcxcjeysz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtwdxotknl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dianchejie.cn/gtnfcmyjcw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtgjswslii.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtaztdxyvw.html

[K04] 读取 JSON 文件
来源：http://hz.dianchejie.cn/gtjtpivsqm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtvkwlfsyz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtuqdoiwro.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtmwbgsqrf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtxyllncez.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cheryme.top/gtkpmqmkic.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtkpzrnykz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtgvimhims.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.meibo888.top/gtopgqfghl.html

[K05] 深拷贝对象
来源：http://hz.yuanzhike.top/gtaaxevsla.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtnriodvoz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtgvrdsnlt.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtubwbixhz.html

TS:   structuredClone(obj)
来源：http://hz.yj20258.top/gtjylnhoyx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shzxlz.cn/gtiuccuryk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gtzhlsfgau.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jiagoushi.top/gtieargvmc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yueranfly.top/gtlvpkqwlm.html


<!-- 参考信息 -->