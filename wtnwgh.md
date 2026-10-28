代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtkbckmtil.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.0kj1m.cn/gtmxdzemre.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenlongwang.top/gtvqqbwqec.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtbuphtouk.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtmpuzlhoj.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gtzrrgbhus.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtwjywguhl.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtmibaxkqb.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtnccioyhh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtoxjyxogm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgfzy.top/gtkvznujzs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sxryk.cn/gtxbyavkwt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtosxgmdyk.html

[H04] 自定义异常类型
来源：http://hz.jqgufenzy.top/gtnieofjhk.html

Py:   class MyError(Exception): pass
来源：http://hz.yonumen.top/gtflgmuzgn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.andypj.xyz/gtmzqrzfnn.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtlxvpywan.html

TS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtgkawktos.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtpnmkypdr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtrznznylv.html

Ruby: class MyError < StandardError; end
来源：http://hz.xylfe.cn/gtnlwnmdfj.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtftkvjovc.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtuvfuhlvf.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gtzpwdczfs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtcfuubiqg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtlhntxtva.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtphpwiqrx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gttztuzucl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.kuanghao11.cn/gtmyngacxo.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnxiangtu.top/gtigtlbrtl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtffwjakvv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtxnlejcfk.html

Py:   value = d.get("k") or default
来源：http://hz.birdmap.top/gtobltzbsk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gtekvzskxc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gteiftkydg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtzuqqrmcj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtmnxscmjh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtqgoklwqg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtrthyocnk.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhaomingkeji.xyz/gtfooqmhsn.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtlqsgnqnk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gzhubu.top/gtbhokvvcv.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gthfhzcryd.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtwdoyzwnx.html

TS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gthspmioqv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuxming.cn/gtoecmehcg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pengpengdd.cyou/gtuynjnegy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtwvuxdbgg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gteidbfqxj.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtazgjkefs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtdjhalint.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtvivouiap.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangkeji.top/gtpyehkfth.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtpikdiwnn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtgtryjtmx.html

Go:   err.Error()
来源：http://hz.ybcxt.top/gtvinmxaiy.html

Ruby: e.message;  e.backtrace
来源：http://hz.yueranfly.top/gtnymkkvgj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtepkvsqen.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtbapyswak.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtgxzrnmsc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtvgyqnfym.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xziqi.cn/gtjbfbtpfr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtixwlpphk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtpyqmwxgr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.quarkkingdee.top/gtsftixtye.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.c1oappe.top/gtucbkolug.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj202588.top/gtyuhuokst.html

[H10] 资源自动释放
来源：http://hz.xziqi.cn/gtsdfldeuc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtptfnggeu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtaltwhtgh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtgjblhcpx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gthuyqipgn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cheryme.top/gtobsznmry.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtruxxoong.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtnfnrhnhk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtpsoiesrn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmzqagtya.html

I. 正则表达式
来源：http://hz.quarkkingdee.top/gthjtmgqbh.html

================================================================================
来源：http://hz.yuanzhike.top/gtvmebbnci.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gthadtrezj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtbbddfyhv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhixingplan.top/gtvfoqlwrk.html

JS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtoruyigoq.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtvlvtfvzj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtuvbylaex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.mhx1999.top/gtbjxjdvwh.html

Ruby: s.match?(/\d+/)
来源：http://hz.quarkkingdee.top/gtfvcvvjpq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guowangkeji.top/gtmnyilfrs.html

[I02] 提取所有匹配
来源：http://hz.cheryme.top/gttpeohprk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtlffjoxfr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guannengcc.top/gtnjqjghjq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ybcxt.top/gtchtrmhvw.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtsexiazmq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj202588.top/gtpsejwhur.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gteiulbvhj.html

Ruby: s.scan(/\d+/)
来源：http://hz.havefunace.top/gtlxqrexqg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gtddipruot.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtjfiylsqg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtdxapukkh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yanxiufei.cn/gtfhoutldb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.iojbl.cn/gtpgqhoddo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinghuilouyu.cn/gteaoevyje.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.316326.xyz/gtmtuhynda.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sysykeji.top/gtgsslcawh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shzxlz.cn/gtqxolbjtg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.snrcjt.cn/gtdgjzycqd.html

[I04] 正则替换
来源：http://hz.nanxinkj.top/gtsomaamnj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtkicxhlgn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtvuahrixn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtdinxbqng.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtsmnqeqdo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hysaishi.cn/gtdvbuakiv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtpobncbeh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhiwuduotai.top/gtxixxcwfo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.smart0.xyz/gtqwfxowfm.html

[I05] 按正则拆分
来源：http://hz.bjfxy.top/gtwjjopnlz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnqzz.top/gtvuwdqrmy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtamporiaj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtnztxomgg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtlrksyohu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.mhx1999.top/gthiflzqyt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtzaqjtvut.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtseamltwu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtibvhxbyp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtfgseyobu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtlrkznnho.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hammf.cn/gtsormoglj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtilufosje.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtxbrcmczl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtczzbgvrl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cucudq.cn/gtlxhlvnks.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtsizqmfak.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtqjmthohq.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangtech.top/gtzcnvtiau.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pycfn.com/gtwidoomhf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuanzx.com/gtdyjmkphm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangtech.top/gtcqjthdts.html

TS:   /error/gim
来源：http://hz.hnqzz.top/gtfzpbpnmj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.mhx1999.top/gtpdshjpft.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tian-w.cn/gtwxidtafq.html

Ruby: s.scan(/error/i)
来源：http://hz.cdnleiting.top/gthqpzjrxc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtifuokson.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtrzgrpina.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jiagoushi.top/gtjvhaoxcm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtzjeixnnh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtibpmafms.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtxjxssnbi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtegpdjpbo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aizwys.cn/gtiubxktvu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gtugqscpah.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zycfv.cn/gtdzjdicag.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgyctbupf.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtooqddmor.html

================================================================================
来源：http://hz.guowangkeji.top/gtsujnpaqb.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtqsdpwkii.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yongpay.top/gtxkvqbkui.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtilwflyvi.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtmwbleqli.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtkghvjokp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenjidiqi.icu/gtfvoftwsj.html

Go:   time.Now()
来源：http://hz.zdqjudy.top/gtlsitdhxj.html

Ruby: Time.now
来源：http://hz.daxiang520.top/gtabistypb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtafrnqsqg.html

[J02] 格式化输出
来源：http://hz.havefunace.top/gtnoelsznq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtmffgmfuk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gthgthvuty.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gtevopubdp.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtwkteymly.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gtwigutcjz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zycfv.cn/gtwmouhgue.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtjknlmdmw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cashguo.top/gtewahyeea.html

[J03] 字符串解析为日期
来源：http://hz.guannengcc.top/gthbmweqcy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtswsbsmpf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guannengcc.top/gttxhjebhz.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtobarurdi.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtlcdjgwdu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtoaorpcbm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daxiang520.top/gtfftrzrct.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtrcphuzgj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.birdmap.top/gtkbqkytac.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtqjirmacp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fzhhl.top/gtgodwqcag.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cheryme.top/gtvlazbpsq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtkxomlkzc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtflvhhyhr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtrpesztuq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtcnlhesyz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yonumen.top/gtuqjycadl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtezjbucbf.html

[J05] 时间加减（加 7 天）
来源：http://hz.daria6918.cn/gtgygrcnqp.html

Py:   now + timedelta(days=7)
来源：http://hz.xingfuxueyuan.xyz/gtfmqahokj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sysykeji.top/gthgplneti.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtaeduojll.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtzvvfvswa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtvbyxntcg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtzrxvdjzl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtoatvtqtf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtfcayexvs.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gtdvyibqri.html

Py:   (end - start).total_seconds()
来源：http://hz.chenlongwang.top/gtywzjhoxc.html

PHP:  $end->diff($start)->days;
来源：http://hz.guannengcc.top/gtbcjmvqmi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhaomingkeji.xyz/gtynzcqnan.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtixsjqvrf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tian-w.cn/gtfmkbabbl.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtidbccgam.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hysaishi.cn/gtjcbxrxqe.html

C#:   (end - start).TotalSeconds
来源：http://hz.yangfankeji.com/gtbxlrqpgo.html

[J07] 比较两个日期
来源：http://hz.cucudq.cn/gtcgqjkivl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtrilkmfvp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtcaqjobhi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtehgfnwvb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtgwfgwouq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgfzy.top/gtprlruqpb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuanzx.com/gtjkalfvmv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtanjiimyf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtjeqacqsg.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gteobzenll.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sweek.top/gtkowulgsi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhoulong.xyz/gtvvqhpeli.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtzkiypgps.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenlongwang.top/gttceiglpz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgfzy.top/gtigelhhxz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtcilhlqux.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhijiandao.cn/gtvealkfpb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gtcxeiajfz.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtaaotcnyy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daria6918.cn/gtibfuxinv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtfueqgjaq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gthunfpwrx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtcavvlzpk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnxiangtu.top/gtyzaenvvd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtojkacaqa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtylcdykbs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtnwipqawu.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtnrqbnuak.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenlongwang.top/gtzhgnkgto.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtuajyogql.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtnyqotnmy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gtypjeiqbg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtnvhxmlgq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtipgrtmiw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtyneozsdj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sysykeji.top/gthghkncmk.html

================================================================================
来源：http://hz.ybcxt.top/gtrlkiirou.html

K. JSON 与序列化
来源：http://hz.ybcxt.top/gtwpodeqga.html

================================================================================
来源：http://hz.nwbrower.top/gtermwwtne.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtxidsdgiz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtvgmbbhbe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtshdocdbw.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtskkfwvia.html

TS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtcyzedbdm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtqossxirh.html

Go:   json.Marshal(obj)
来源：http://hz.nanxinkj.top/gtmmtjweta.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hammf.cn/gtkhmslcgj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gogol.net.cn/gtmlusodvm.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtfsfufdnm.html

Py:   json.loads(s)
来源：http://hz.jyoumei.cn/gtngczewgu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.kuanghao11.cn/gtpftkozgv.html

JS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtpkizbdoj.html

TS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtjotvpaum.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jyoumei.cn/gtrezqvbng.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtccajzdmx.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtmtjqmwkh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtqwyqsxcl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtyolxjzxs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtwwdworfd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtnovxjiod.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtjducarga.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtfkgukijf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtnztfgqmu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtgrberywl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtzonlicpq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtspegfedx.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtrexutdcq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtfykdrjrc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtinafzbro.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtnkfudmoz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtgrclztku.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guowangkeji.top/gtcqfwdeqq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtytuvntky.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtcbhzxnll.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtdoqtcfya.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtipqamqbh.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gtxbfznexv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtocrwcirz.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtcmuavtay.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtpdadcspj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gtjkrsgqje.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtbzxcfilf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinghuilouyu.cn/gtoklujyjd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gthhnudvdb.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtwnxfshot.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gtqhvpasnk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtsaacdhsn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtdveoeicc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtqvyqqnyw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtthynzzya.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtfdiynujp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtzagoqemh.html


<!-- 参考信息 -->