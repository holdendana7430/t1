代发 wailian999

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gtzoijydyg.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtykaijoty.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtetekkrlo.html

JS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtjeoizkum.html

TS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtgxiunfgg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtfekbqxoq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtwfpeuebq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gttycarweo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtbdhzikvr.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gtthjtwhuz.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtihjmmbro.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtbrvjwarh.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtcbfnqvhk.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtpuulzvbn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtuqiaoijl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinyuanbaomall.cn/gtxqyrldlg.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtuauzwysf.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtvtquewsj.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtdzncgqmp.html

Py:   except ValueError as e:
来源：http://hz.cashguo.top/gtszixigyx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gttctpxosv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtrzhpijrn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtxjgvxtbw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gttguzvkdl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guannengcc.top/gtedlrrnpi.html

Ruby: rescue ArgumentError => e
来源：http://hz.zycfv.cn/gtfostoizj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtssjuzffd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinyuanbaomall.cn/gtkxusiuoy.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gthsebvxll.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj202588.top/gtqvdwqjmh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtvffncadd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtgfoonhud.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinyuanbaomall.cn/gtvgjjyeie.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtthwckpyp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tanke756.top/gtyzzccwzt.html

C#:   obj?.A?.B ?? default
来源：http://hz.haohaochexian.top/gtrfgmhifc.html

[H07] 断言
来源：http://hz.cqqwz.cn/gtycbeabum.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtfnrjcczt.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtszjxbekh.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtgloljewm.html

TS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtrymtnnmx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtohoidlfe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtlacfmtcn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yongpay.top/gtamhoooak.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtlvyfoxkr.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtxjdnwupg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtrmqmfekg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.havefunace.top/gtdpzxwmjv.html

JS:   e.message;  e.stack
来源：http://hz.hfpthk.cn/gtxpqtooab.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtrbvtcetc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xylfe.cn/gtyjkftebb.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtdmbtfohj.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gthtibcvzh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtcbtsicsa.html

[H09] 带错误码的异常
来源：http://hz.jianghu66.top/gtlnhlsqrc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hfpthk.cn/gthyldgjfy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtuqpelouq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jlsjyb.cn/gtjielfcbt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258888.top/gtnpbeoibu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtvpfptucx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtqlfhyaux.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtybpjxhtc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gtjbnjjwcp.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtjysmesaf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtcluhfkfp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gthgkjnyrv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtnjejdywb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtmyjoeaxi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gtqpocghsz.html

Go:   defer f.Close()
来源：http://hz.jinqigfzy.top/gtbfmavdtl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtqwqwcvyb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxinkj.top/gtghzsdxrt.html

================================================================================
来源：http://hz.mhx1999.top/gtskhrstgp.html

I. 正则表达式
来源：http://hz.cucudq.cn/gtixoxqyly.html

================================================================================
来源：http://hz.ydjk.org.cn/gtujjwipiw.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtcrmqphza.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yonumen.top/gtkhtcddfh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhongyouzk.top/gtxbriqjkq.html

JS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtokdhivrj.html

TS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtdybvkabe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtsajyarzg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigfzy.top/gthiarrmhk.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gteczektkb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gthycrauuk.html

[I02] 提取所有匹配
来源：http://hz.pengpengdd.cyou/gtyndpjdgo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtfghiappk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtssqfoyfg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtecancgro.html

TS:   s.match(/\d+/g)
来源：http://hz.zhongyouzk.top/gtfvzdgpxg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jianghu66.top/gtvehceoat.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtmkldudxy.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtpadyjzwu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtpnkibeyi.html

[I03] 提取捕获分组
来源：http://hz.daria6918.cn/gtidmevtio.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jyoumei.cn/gtzzeaucgq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cdnleiting.top/gtmiifhhqs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgufenzy.top/gtnabvxpan.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtsonwfmrv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gtmuibtdgb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtfwzrgwtw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinyuanbaomall.cn/gteudsxjir.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtwiyzrjcg.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtzukzapvc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aizwys.cn/gttucwljjc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtnvcyzdwy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtrcjtcaco.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtbuamigfh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtfmutghzk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xinyue.icu/gttsdhpjkt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sweek.top/gtbwgnwmcj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gtrofjbphl.html

[I05] 按正则拆分
来源：http://hz.nanxuanxn.top/gtjuchwyhq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtlhknvfqk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jiagoushi.top/gtnvrcdqap.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtcawfkvzy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtmyqwnwmi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gtcfyqpqhf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ybcxt.top/gtpzxzbcri.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtrqpfycsy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gthoieflvf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ehwqpu.com/gtjgxtxuaa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtqmspxvep.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtiekvkrrg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtqhhsccgo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtszruvhlu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtlrlrkwwq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtpsquctqs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtdpasjidj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtckmfyfuu.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gttgvasnnl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shangyingyoupin.top/gtivrbdomv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shangyingyoupin.top/gtethqhrml.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gtgqwstdbd.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtnkvhktvx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gtgnzrsdyh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shzxlz.cn/gtjcgyaeqs.html

Ruby: s.scan(/error/i)
来源：http://hz.hnqzz.top/gtbzmqafvt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtvzvyovwy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtjpfnmvsy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtkevrlrvj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shangyingyoupin.top/gtqualwjts.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtmrkcdqyc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gthiodyxkw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtypcetrfg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhoulong.xyz/gtipvwwfkp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fengsongda.top/gtwmiwzctz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtrnmyaamd.html

================================================================================
来源：http://hz.gzhubu.top/gtitsujlty.html

J. 日期与时间
来源：http://hz.hfpthk.cn/gtmkyyvzsv.html

================================================================================
来源：http://hz.mhx1999.top/gtsxkvpwap.html

[J01] 获取当前时间
来源：http://hz.fzhhl.top/gtynuzaejo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tanke756.top/gteaebnkmu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtwefhmtgb.html

JS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtihqcuxny.html

TS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gteujfguyb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtefhavyvz.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtcbfcpuai.html

Ruby: Time.now
来源：http://hz.zdqjudy.top/gtqpbnrtzg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtcsdjeylf.html

[J02] 格式化输出
来源：http://hz.tanke756.top/gtggxurdzt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtrtkxduzh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtlmypixxr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtiuhaobrj.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtjptmzdjc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.birdmap.top/gtuxgwepnm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtoxstiyan.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtydyoemcm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.iojbl.cn/gtoujketor.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtgqwatpbz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhoulong.xyz/gtdeqwragq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gaohongyu789.top/gtymtynmvx.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtrsjrqcld.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtbbpreljx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuxming.cn/gthazficvd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuanzx.com/gtmsfulsbo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtyjpkkkhg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gtfrlvfunc.html

[J04] 时间戳与日期互转
来源：http://hz.cheryme.top/gtdivdpwqw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtklhtvaxx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.quarkkingdee.top/gtyouffsxh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.andypj.xyz/gtwlesuyfs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yangfankeji.com/gtljucadgx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtmbihzzss.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinghuilouyu.cn/gtheznocvf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dashuyun.cn/gtwrtxlsrj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtxyxmlmld.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gtsprjrnof.html

Py:   now + timedelta(days=7)
来源：http://hz.meibo888.top/gtwchrhcet.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtbksqrfkh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtskrgfntd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtktwkbjiq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.mhx1999.top/gthqibcwoa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hammf.cn/gtnajolxrf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pycfn.com/gtvhxikwaj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hongshengwenyu.top/gtcatozabq.html

[J06] 计算两时间之差
来源：http://hz.yueranfly.top/gtvvlhdlcr.html

Py:   (end - start).total_seconds()
来源：http://hz.yongpay.top/gtzpzntgmn.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtlglhadtx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtgdijmbdh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.redwolf501.top/gtilzjmwul.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtikkdqtug.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtmipbkvyh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj202588.top/gtibtjzaim.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinghuilouyu.cn/gtjdxtcbol.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtsfucovye.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtjypgvgfs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sufxvd.cn/gtuqzhcjkt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtqxctxsli.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtmmzmtklc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gthqmylrpj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtlhdpiwly.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtbahnzywa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtjdnlwnle.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtmmdogzsf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gogol.net.cn/gtjgqxzijv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuanzx.com/gtovcdigrn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtrfvjseto.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tanke756.top/gtkbplnxuw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenjidiqi.icu/gtaqqiradm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtroczvvtx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gtevpjugzm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cashguo.top/gtoaknyrgv.html

[J09] 时区处理
来源：http://hz.xingfuxueyuan.xyz/gtayoedxuu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhijiandao.cn/gtledekouy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtdnygfsff.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtsggzyhsg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtftgqbzyl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtqcnrideh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtkfgejzdi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuetiantiany.cn/gtdmjastyb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydjk.org.cn/gtrspdcumw.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtmzuvtgsl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtddxxbxsn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigufen.top/gtwmnxsotc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shzxlz.cn/gtnghgdcrl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xinyue.icu/gtsufiptgx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtbjgjmhdm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.andypj.xyz/gtmymhecak.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gtdbjyvuvc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtwhkatjol.html

================================================================================
来源：http://hz.gotoacloud.top/gtdgwtvsuy.html

K. JSON 与序列化
来源：http://hz.jqgufenzy.top/gtpclpeurp.html

================================================================================
来源：http://hz.yj202588.top/gtwzkkxrsh.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj202588.top/gtrxokjbes.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtmapjkjll.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtfhferacd.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtbctrvufd.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtosjhelkc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtodrmsidw.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtshmusseg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.bjfxy.top/gtgjlvwcbu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtyaurzvpi.html

[K02] JSON 字符串转对象
来源：http://hz.birdmap.top/gtjgjsuave.html

Py:   json.loads(s)
来源：http://hz.sweek.top/gtytgrwwbi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gttaqlsfow.html

JS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtasfpxpdv.html

TS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtnklbhwhw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtkabrxbmb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtqvtyjdoe.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gtvrbtgkir.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtbghutgir.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cheryme.top/gtsuhtplyu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtkbbwzqgl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtvgzgjjbq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtmlpxdvbu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtlyoheyez.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtwtkyxhkm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtmxjjjhvr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtrzyqewqd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dashuyun.cn/gtswxnemva.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtfkdoehbw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ivvv.top/gtgegrvwto.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangdashe.top/gtsbekzawf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtipikalmv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gterfgwlmm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtawouhiky.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtcctcxflc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtijkxpkyj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gtocsdrjld.html

[K05] 深拷贝对象
来源：http://hz.sufxvd.cn/gtjjhmnjsa.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtgklhunps.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtnjskjhpw.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtrughjplg.html

TS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gttnwngecl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dashuyun.cn/gtsxsngxwk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.redwolf501.top/gtcevswcqi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cucudq.cn/gtynxjwkmj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gteximvckw.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtfrwaumkw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtfcyscjie.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.bjfxy.top/gtmmfczumb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtfpahzpds.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtovsftogk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jiagoushi.top/gtkbninqoi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.mhx1999.top/gtdggwefxb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yongpay.top/gtpviebneg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtiemwoidq.html

[K07] 进制转换
来源：http://hz.52xcode.cn/gtqzopiilt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtgqfvntvf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gtbhechivt.html


<!-- 参考信息 -->