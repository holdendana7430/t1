代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtscnvoyiu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtyemjwtxi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtyijkdfsu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jiagoushi.top/gtvudanhao.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtgbtodnfm.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtfhvzzowl.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gttvsapmdj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gteyrfjicd.html

JS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtdmnxzmyg.html

TS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtxhurtjem.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtsxpwdiqb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj202588.top/gthwrjlmbh.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gtgzlnjcjb.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtwztpfikk.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtjfysaagg.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtscatjrcm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yonumen.top/gtuolbnkxf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtbluinxzy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtldprucwc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtkmbjjlbf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtzfkcygts.html

Ruby: rescue ArgumentError => e
来源：http://hz.meibo888.top/gtqgfgbztl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yanxiufei.cn/gtpenmpowv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtfoxpqgxi.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtvdwicblh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtanpagkza.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtfnemnhit.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtlelwjfwf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtqkugqthe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shangyingyoupin.top/gtdyrazjnb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtcqvjytns.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtzfmzsuln.html

[H07] 断言
来源：http://hz.cheryme.top/gtgwcilfsd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuxming.cn/gttgixewek.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtqnltanxg.html

JS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtdsxwlvob.html

TS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtzntgtxzr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtcxnlvxqf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258.top/gtnlxpftug.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cucudq.cn/gtczxudbfb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hfpthk.cn/gtjbayhcrg.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtqyrwlurf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtdeqcmhzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtjixscptk.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gtjkydlwxf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhijiandao.cn/gtwhedealg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtqbxxdege.html

Go:   err.Error()
来源：http://hz.svipenyu.cn/gtcwwmtvux.html

Ruby: e.message;  e.backtrace
来源：http://hz.feifeiyinyue.top/gtoqlrutkg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pengpengdd.cyou/gtvytriehk.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtmphaumud.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtisimagmq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yvedp.cn/gtejtvzjji.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.vqdsnc.cn/gtvlosfatg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtqriiwjke.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtajasgryg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtrmmybrre.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.c1oappe.top/gtxzldaifq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gtrgwcqgcr.html

[H10] 资源自动释放
来源：http://hz.shuidangran.top/gtvdkkxylw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jianghu66.top/gtjodmedgu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gtkdmkvhjv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtnupnfeeu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtjvliqhbd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtwhagdiws.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtozsnqtqp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.birdmap.top/gteghpehzi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtotubbsri.html

================================================================================
来源：http://hz.jinqigufen.top/gttsfckzay.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gtralsokzb.html

================================================================================
来源：http://hz.cashguo.top/gtygpmhdqi.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtfltxdtvt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtvqwrdnth.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtuwautpet.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gthdrmplxn.html

TS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtnaztahrs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhoulong.xyz/gtcvmqfhdy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtrqxdpzzy.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuanzhike.top/gtvnrgtoim.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenjidiqi.icu/gtnutfqwzt.html

[I02] 提取所有匹配
来源：http://hz.yuxming.cn/gtwvedlyif.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cucudq.cn/gtgorvfwui.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtnuotenro.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shangyingyoupin.top/gtaazkcuhg.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtafbrghur.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ywan-chungtsiang.top/gtkevqerrs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtgizasmwm.html

Ruby: s.scan(/\d+/)
来源：http://hz.sweek.top/gtmokxmcxy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtagrjrwyo.html

[I03] 提取捕获分组
来源：http://hz.dashuyun.cn/gtjyibamzm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinghuilouyu.cn/gtsismpywe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtlkxqsayq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xingfuxueyuan.xyz/gtsrsiroid.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gttwgfoqnp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guannengcc.top/gtlummvpdj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tianlin.xyz/gtfvfwvmob.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtbojhfdjm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtessfrkxn.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtdxtqocru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtfbretwuu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gtjgpeenkl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtjspvljla.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtyptpakfx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtwsnqjroo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gzhubu.top/gtnamrfjms.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtdzcxrjtw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.9152youxi.cn/gtdfkqofeo.html

[I05] 按正则拆分
来源：http://hz.ybcxt.top/gthvnkgenx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtydmmwaru.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtetnqbalz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtnchxmkob.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtaficfjqe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guannengcc.top/gtfkdnhhbp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtcpeklpxr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtaxnzltnm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sxryk.cn/gthkrzubqp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ivvv.top/gtlbgzunsz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtnugcnedo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuetiantiany.cn/gtyryhijrq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtllhodmlw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gticfmvjex.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gzhubu.top/gtvxvsdjjo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gtresbefto.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.52xcode.cn/gtwqebbaih.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtxoavthss.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtwkjsoavr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtigmtzdky.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gtinpcwhgw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtxgsgxcud.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtrvwaqyef.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gogol.net.cn/gtxxmkrgrj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuxming.cn/gtlctzqpto.html

Ruby: s.scan(/error/i)
来源：http://hz.zhaomingkeji.xyz/gttrmjhevw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jianghu66.top/gtuynveogl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtbardxjlq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtcnzsumpo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtyfjfvgdu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtsxbsnyjh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gttqeiorrm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtbjesfuly.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtcatamvuz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtqersxzot.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuanzx.com/gtjuciktxk.html

================================================================================
来源：http://hz.chenlongwang.top/gtestibmwi.html

J. 日期与时间
来源：http://hz.yuxming.cn/gtzscobkja.html

================================================================================
来源：http://hz.yuxming.cn/gtuksazlsc.html

[J01] 获取当前时间
来源：http://hz.svipenyu.cn/gtkfbejeeo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gttjchtmnu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtcvbywiaj.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gttokhydhc.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtxoizcevg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jyoumei.cn/gtcxrtbkim.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gthnvrydxv.html

Ruby: Time.now
来源：http://hz.yvedp.cn/gtnewrtawe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtcklihqhd.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gtzbdgyjwx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtlktfjfwp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtpnqullsz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigufen.top/gtuzkodbym.html

TS:   d.toISOString()
来源：http://hz.tanke756.top/gtlwtwbcuc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hfpthk.cn/gtfqpxumst.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jianghu66.top/gtezotmkmf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtawchhtva.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.feifeiyinyue.top/gtvacbydqa.html

[J03] 字符串解析为日期
来源：http://hz.0kj1m.cn/gtlfomumbf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhijiandao.cn/gtaaxcqesf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tanke756.top/gtfternsci.html

JS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtaljajguu.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtonypoiac.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtpthllpeo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuetiantiany.cn/gtswchvldg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtxgdlmozu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gtmkizfuzj.html

[J04] 时间戳与日期互转
来源：http://hz.zycfv.cn/gtvizjjzgz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtvfcgrbaz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhixingplan.top/gtjpdrulna.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gtmhkwgtxr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtfjjiider.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtsnccamgq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guowangkeji.top/gtkfpmnkjb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtqixfbgjt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinghuilouyu.cn/gtxgpkvgof.html

[J05] 时间加减（加 7 天）
来源：http://hz.sufxvd.cn/gtrjbltpxt.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtqlqvtjqi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gtaneynwuz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gthjbvhyxy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtpjnhtptm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ehwqpu.com/gtznlmznon.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.andypj.xyz/gtyxjvvugj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.svipenyu.cn/gtoargbpyn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinghuilouyu.cn/gtemoitdgh.html

[J06] 计算两时间之差
来源：http://hz.bjfxy.top/gtpduzydkp.html

Py:   (end - start).total_seconds()
来源：http://hz.smart0.xyz/gtgxgkrozj.html

PHP:  $end->diff($start)->days;
来源：http://hz.cashguo.top/gtljcmnpzw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtwwrabgmn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gaohongyu789.top/gtoimzgqjv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtwvgilvfv.html

Go:   end.Sub(start).Hours()
来源：http://hz.c1oappe.top/gtiilsutqt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtedhmscdp.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gtppwgkyiu.html

[J07] 比较两个日期
来源：http://hz.yongpay.top/gtzvcugcxv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtgsybefmj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtxptggzes.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtxgzbhfbw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtrxkhitfn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtrrgvurnw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtzmkyvnln.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtrsvgejyr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtqnizxmrl.html

[J08] 提取年月日与星期
来源：http://hz.yongpay.top/gtcbcqppsp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtjbdpwauf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtzdgrnjgv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gtgqqtzaum.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gtssjcypjc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtysqxvdom.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtgyynxkqz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhaomingkeji.xyz/gtavljnibw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtepfleoje.html

[J09] 时区处理
来源：http://hz.xziqi.cn/gtzmlopxzq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtwcsgbzgp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shzxlz.cn/gthizavgzr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtiuvlrjzt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtgmqobfag.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtcynezbpy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gtbtbgbjdi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gzhubu.top/gtkhoyjlhb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtyxyhrwvv.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtddqddkmd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258.top/gtkatitmqu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtwgxuurwz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenlongwang.top/gtttkrrwfn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtppvypvgz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ybcxt.top/gtiotibdvu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhiwuduotai.top/gtfjbgfufn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydjk.org.cn/gtfimrhjye.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ehwqpu.com/gtfbqyqncs.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtiquolgue.html

K. JSON 与序列化
来源：http://hz.pycfn.com/gtebfgbjgk.html

================================================================================
来源：http://hz.yueranfly.top/gtcrxuotad.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtsfvhcdmr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtpjievmdm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtmtsljgmq.html

JS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtbziglhvo.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtmrgcjftl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtjiqawkux.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtqrdotgcb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtixyeohci.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shangyingyoupin.top/gtiqtjnjyg.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtmgvropfs.html

Py:   json.loads(s)
来源：http://hz.xuanzx.com/gtwmhoodbp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dianchejie.cn/gtclgwjkhd.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtxztvmxkk.html

TS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtsfuyaxsf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gtpbyojxik.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtkimaqxhi.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gttbxrpuub.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gtjuonvjke.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtrtwktpxd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtmdljxqcb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtghmawdyc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtevcngdcn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtbdjqdisp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtlqgumuib.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtrqxdlehy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sysykeji.top/gtpuppqygm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zycfv.cn/gtkrafnlks.html

[K04] 读取 JSON 文件
来源：http://hz.smart0.xyz/gtigagxhoy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pycfn.com/gtscsrizey.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gttjyfckku.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtprtalgeo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtdsltkvrf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtrnejmfnq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtvssyucay.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtmlgwxvtt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtlgxuefjt.html

[K05] 深拷贝对象
来源：http://hz.aizwys.cn/gtyrzybrim.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtptodmxtp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.birdmap.top/gtwtsulgwc.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtbtyndtct.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtulyyddgb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangtech.top/gtfgjtfekk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtfnrfgboz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnqzz.top/gtcvgahncj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhengqikj.top/gtzwucrnmx.html

[K06] 解析 URL 查询串
来源：http://hz.daria6918.cn/gtispbczgt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jianghu66.top/gtuvaephgf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hywenlv.cn/gtzxxpccdi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtjwikylyj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtacdgzewf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtqzqqguio.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.52xcode.cn/gtvqxqinio.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.meibo888.top/gtftcyzjci.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtxiomdtyo.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtcntvkfeg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhiwuduotai.top/gtikqucfxa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtkndagkdd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtxemxawuq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtllsdxcvg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtcakljalf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sweek.top/gteupvlnti.html


<!-- 参考信息 -->