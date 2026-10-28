代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtaxoaxyqj.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtqbynkyfn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtqqzahzlw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.kuanghao11.cn/gtzuamunvb.html

Ruby: class MyError < StandardError; end
来源：http://hz.birdmap.top/gttjvotexy.html

C#:   class MyException : Exception {}
来源：http://hz.zhaomingkeji.xyz/gthobvobkh.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtwefeyfsn.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gttithmqer.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgfzy.top/gtyuwxgscf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtgzgpvhjd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtlraqnggp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtmdimtytp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtfosxiosx.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenlongwang.top/gtfhrmsmcw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.vqdsnc.cn/gtmnfkfsdx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtzkstmkhw.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtpotkcvte.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aibaodan.cn/gtcofvjjnh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtselzoakt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtamrfccfh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hysaishi.cn/gtfyyelgoz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtyznknjfv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtgvmmsvbd.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhoulong.xyz/gtevslzkcv.html

[H07] 断言
来源：http://hz.zhoulong.xyz/gtkisbjujo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cucudq.cn/gtypvariwy.html

PHP:  assert($x > 0);
来源：http://hz.yj202588.top/gtedwnbkwo.html

JS:   console.assert(x > 0);
来源：http://hz.chenlongwang.top/gtdillontz.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtgyzlhpba.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gtxukmonxv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.mhx1999.top/gtdlazsgpx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtciivojwo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.52xcode.cn/gttjotbbcy.html

[H08] 获取错误信息与堆栈
来源：http://hz.gotoacloud.top/gtubeknbki.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtmqejasnl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenlongwang.top/gtndeiezgf.html

JS:   e.message;  e.stack
来源：http://hz.aibaodan.cn/gtqfrezfpw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xinyue.icu/gtxjgimksh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fzhhl.top/gttjmowtlc.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtuxtexcoh.html

Ruby: e.message;  e.backtrace
来源：http://hz.sysykeji.top/gtlxnrzilz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtpxhawxah.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtslovvhdy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gtlqmisfny.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hysaishi.cn/gtabsxrbsg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtdskeshhi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.meibo888.top/gtxrelnhkk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xylfe.cn/gtariffljd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gtdehuqnux.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gtnjyzzkov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtbeijzkjb.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtcrllchig.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gaohongyu789.top/gtxaqptnqd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtgdofhhex.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtcwqdffru.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtzdfirdct.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtbdbazcbj.html

Go:   defer f.Close()
来源：http://hz.svipenyu.cn/gtyregeyve.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtrdtfeqdv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtuwbyzvkx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvpwtfqvx.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtquhrtmws.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjrmgamep.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtthlgxgew.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtmrsnwrip.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yanxiufei.cn/gttxnwarpq.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtrnvyecbp.html

TS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gttkzbdvmv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gttajsstvg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtlzenxeax.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gthytciemx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtmzxdrylp.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtwrowjraw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtrbtbvpos.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nwbrower.top/gtkccgdges.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aibaodan.cn/gtobxfngxn.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtvrrpfzty.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtfhvvzmlw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtkjufrjya.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtiucyiwed.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtrmwkhyba.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gthphxgzxd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtlzzzqcro.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gttukibrol.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.iojbl.cn/gtsoecbbiq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ybcxt.top/gtxkchnezb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtqqsnykmt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gtewpfwvcs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtphkpypel.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtbcijjblj.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtvncduoei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gttnuvrnif.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtafzxvtob.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtvbibazjn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtvjlgqtty.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtjadsxzjx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtiwloyyyq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtdaczgtig.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zdqjudy.top/gtlxanuydx.html

[I05] 按正则拆分
来源：http://hz.pycfn.com/gtxtmljlgx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtwvgpkxgf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guowangkeji.top/gtkdsvsjvo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtdtkinbcy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtploqdtfo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhixingplan.top/gtcvfwrsfk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenjidiqi.icu/gttcdrkhzx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gthbsrhbth.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cheryme.top/gtjccqjjtx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.0kj1m.cn/gtiarhjcmg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtahwzcbru.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fengsongda.top/gtcfwzuwws.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gthfhrginc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtvhkowdph.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtemdmpeal.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gttfbgcgen.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtsulxsvwl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtcryvdqll.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhoulong.xyz/gtpbfywadz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtjqyhjswx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtiggevpvs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtybtlcdxk.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtkrnxdaxv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gthzfmldbc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jiagoushi.top/gtazsgvlyg.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gttwwxyvkg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhoulong.xyz/gtsfprvtsw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yvedp.cn/gtozzuflbn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtmdlokjiq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenzaomai.com/gtxmzmqiwd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtjfpxyapt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtgtycriqf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtievckwms.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtwrernwfx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jlsjyb.cn/gtticwqxhp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ybcxt.top/gtlakynzqj.html

================================================================================
来源：http://hz.yonumen.top/gtgxnszyaf.html

J. 日期与时间
来源：http://hz.tanke756.top/gtypndcstd.html

================================================================================
来源：http://hz.guowangkeji.top/gtylvpheta.html

[J01] 获取当前时间
来源：http://hz.ybcxt.top/gtblsjppdd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xinyue.icu/gtwdfofcel.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtdirupsrf.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtrxcahsux.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtcbzxtygw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtgwfoonfq.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtspljbcbx.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gthjnhvuaz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258888.top/gtzvuwnbzp.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtgvktohsj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtpkhaedjg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtsqmbfqld.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtzdbajgix.html

TS:   d.toISOString()
来源：http://hz.ehwqpu.com/gtdhgardvj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtmwtzgdza.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtltoutuac.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtywnnhjan.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jyoumei.cn/gtnmkpojld.html

[J03] 字符串解析为日期
来源：http://hz.aibaodan.cn/gtmrqdqqba.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gthzrfnyip.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aizwys.cn/gtqxlrhqia.html

JS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtnqwcgiwm.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtpjrxqqnr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gttsohbopd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtlmhfqfvf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtequrycxw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtkvnplxga.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gtbyrclmtd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangdashe.top/gtlqfsneqb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tianlin.xyz/gtgqvwckqk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtptnzsjuv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtqkoxykct.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gzhubu.top/gtahbhysxx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pycfn.com/gtozhfwxkn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtvlqqvmpz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhijiandao.cn/gtiozcmrum.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtbviykyvp.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtjajkojfn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pengpengdd.cyou/gtyxqjclgh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtejwfrzod.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtnpwljfqo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gogol.net.cn/gtxejxvvgk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtxkckctnf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtvagdisvn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gthrxbqjgu.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtgpothujg.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtuilmhsss.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtqlcsarwk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.vqdsnc.cn/gtcpdpmqiw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gteymhyztt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pycfn.com/gtdctbonoz.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtfrzwujyv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinyuanbaomall.cn/gtgxocuoep.html

C#:   (end - start).TotalSeconds
来源：http://hz.ehwqpu.com/gtakfbaymb.html

[J07] 比较两个日期
来源：http://hz.xylfe.cn/gtunbfqwby.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtlznpbvib.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aizwys.cn/gtpvdygodu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtyyrmploz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtkmiooryf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.vqdsnc.cn/gtkobkdsdb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gthuyleyie.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtjezmtqlp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtcwrdzmes.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtecfduwis.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtnbfwfymj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.0kj1m.cn/gtkhrrgtgi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtvumueosp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtdphewzdp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gthtustytm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtqbgtsxap.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtsnsksmzs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinghuilouyu.cn/gtxxlnehuf.html

[J09] 时区处理
来源：http://hz.zhengqikj.top/gtkkbdbqgp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gtzusgqeza.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtmtkskqyg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtefpuvejb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtgncjioil.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtlakfwvem.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gttyaxgsop.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtyxccjseu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.bjfxy.top/gtwwylipkp.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtrtcjlakz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.bjfxy.top/gtzrumfvaf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.quarkkingdee.top/gtrsqrxodw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtpfvtkgzx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gtjrrvlajl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtkhtdiqhi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ivvv.top/gtfolipjtt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnxiangtu.top/gtgnvirgjb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hongshengwenyu.top/gtmtfrexrr.html

================================================================================
来源：http://hz.ehwqpu.com/gtvixldkpz.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtlrytwyoo.html

================================================================================
来源：http://hz.nwbrower.top/gtqzskilqj.html

[K01] 对象转 JSON 字符串
来源：http://hz.52xcode.cn/gtifukwyuq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gteuawksae.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtzcgdlwqw.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtzgrwgbwn.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtkgfhdmlt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydzc1.top/gtzzpqkrlb.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gteugqurgp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hammf.cn/gtchurdekj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuetiantiany.cn/gtxsgrvfzv.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtfgzqixdl.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtfedfoudx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinyuanbaomall.cn/gtlyovyylb.html

JS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gtwyhadxex.html

TS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtxgjnoiot.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guannengcc.top/gtjspdhlum.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtcvhuhqhe.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtbahjfyft.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cashguo.top/gtqkemolbg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnqzz.top/gthvcyqjuq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtmijpbqpr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtazfdnynm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtlsunyyrn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtffuyxopf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtpkecinfj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtvueftkff.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhongyouzk.top/gtqqwkvotr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.andypj.xyz/gtveddteif.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtxnidhbpa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtpqeceenf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhoulong.xyz/gtrjwqxtda.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtexouenqn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gthpskinmu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shangyingyoupin.top/gtodiczjtq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtnybohmlt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yvedp.cn/gtanmgjwqi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.meibo888.top/gtesmpekvz.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtziqfbohg.html

Py:   copy.deepcopy(obj)
来源：http://hz.guowangkeji.top/gtavpvywnw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtcnzyauon.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtqodwbtzv.html

TS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtirqrpztn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gttydacjon.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pycfn.com/gtowrustrs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtudeafdhv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gtckwtjjsw.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtuxfltpnz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.c1oappe.top/gtuvzxjrsy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.birdmap.top/gtaoqzwdil.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtwjtocfij.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gterdnrywk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangtech.top/gtcvlfurfc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtcqcimoce.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtlvlbpesb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtmickcwie.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtesgvyoqu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtaswehzxy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtixwxajnp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtsysztsts.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtwgazoeaq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gttauqrdir.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtqrzclopq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtpnuwuijh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtubybeega.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gtgqrltoji.html

Py:   pickle.dumps(obj)
来源：http://hz.iojbl.cn/gtjytxhxoh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtsmrhzxza.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtkgkyudip.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtppaqsgda.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtvkazdjvr.html


<!-- 参考信息 -->