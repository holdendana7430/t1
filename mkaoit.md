代发 wailian999

[H03] 主动抛出异常
来源：http://hz.jinqigufen.top/gtbqbjpdbd.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtretbqmnn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtlqnmhxoc.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtbdgofrfy.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtfshixpjz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtdcsprckh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhaomingkeji.xyz/gtmfwhcljw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shzxlz.cn/gtajrjromi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtlvowgkhe.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtlccewlft.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gtgghqdxan.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtpmtxrimf.html

JS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gttjlskabt.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtaavjoxfd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.redwolf501.top/gtawtgicox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangtech.top/gtgresdetf.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtnmvzwcyy.html

C#:   class MyException : Exception {}
来源：http://hz.ybcxt.top/gtwyshwpww.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtejcjpscz.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gtagafafes.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtijxbzwhp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtyqcaropy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtejdiigmq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ivvv.top/gtszsceirj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenzaomai.com/gtpuebcdis.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtxbihqmci.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yanxiufei.cn/gtejaqfkko.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gtnhfnojxo.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gtsqvzihcs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtunijukay.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtmwunvmjk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtuphtzbok.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtwunrhzod.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dashuyun.cn/gtbgsmewiz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ppjwa.cn/gtjcfyyzeu.html

C#:   obj?.A?.B ?? default
来源：http://hz.c1oappe.top/gtcuiyatlf.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtynmohfws.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gzhubu.top/gtdcelxcbu.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtklhzbghz.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtbduidlhp.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtdohfemrw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtfjxmuzyu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtiqzkwycz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yonumen.top/gtedesgheq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenjidiqi.icu/gteyrtlzqi.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenzaomai.com/gttwnjjmkz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtudquyyvk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtoipjhbzc.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtmctmurgb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenlongwang.top/gtbpgejwvp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangtech.top/gtvtchcpta.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtgmrqfspk.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtgqtnyphg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.birdmap.top/gtfcxgtlnt.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtcrojkglz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yonumen.top/gtonmqzics.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuetiantiany.cn/gtprwggxgd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtqaluabaz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.mhx1999.top/gtvijgwxfa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jyoumei.cn/gtnggpeaul.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenlongwang.top/gtoegnkgix.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtsitesviv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.birdmap.top/gtodrazpux.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtxnqklxxj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.9152youxi.cn/gtexqoelub.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtlrgwrowu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtbcdffdax.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtkazbpnps.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtjlkhxvym.html

Go:   defer f.Close()
来源：http://hz.daria6918.cn/gtdcfevtwd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtexlgucwt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aizwys.cn/gtuheotdmr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmxpfkvax.html

I. 正则表达式
来源：http://hz.yonumen.top/gthbygcbzo.html

================================================================================
来源：http://hz.jlsjyb.cn/gtusafmuiy.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtdaflbqqk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.c1oappe.top/gtufgopfjn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuxming.cn/gtrvsajrse.html

JS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtlfxveifw.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtjkalrywp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtntqmpock.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.52xcode.cn/gtwilohpxq.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtaprfqstv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhengqikj.top/gtdgzrexul.html

[I02] 提取所有匹配
来源：http://hz.c1oappe.top/gtmplioyfk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtstsxcucu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gticwvhqmn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.andypj.xyz/gtfjclyxxg.html

TS:   s.match(/\d+/g)
来源：http://hz.zhiwuduotai.top/gtqgrzubdc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtdvppwnfm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtbbxapqfo.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtmpxftgxy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtnfvxrkfm.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtjazcicju.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gtlwzfuato.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtgrjsfgje.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.0kj1m.cn/gtcceppebg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gthirqphvb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtuhnfudha.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtlgwirptz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nwbrower.top/gtmemzwogy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtbfvqcqfr.html

[I04] 正则替换
来源：http://hz.zhengqikj.top/gtecboslgg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gtibhyufvs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtgukeluxc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtehrinyyy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtlktsawvz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj202588.top/gtxjpcyrnk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gtkokdhria.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aibaodan.cn/gtnbydorpk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtiprxcahn.html

[I05] 按正则拆分
来源：http://hz.xuetiantiany.cn/gtvxinayjg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtjmvxftnn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtvfyotddn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtsmmdnzol.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtvfzwfbuy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtqoxhzttk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtmmuhsdob.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtxcvmnuva.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuetiantiany.cn/gthxgedcfb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yongpay.top/gtxbtcrthy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtaffbixvu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gtwnelzeeq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtswkfooat.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtxkfhyowu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gttjzbmozj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gttcohuuku.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtfdbthmfc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtooyarjfc.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtxezgrjvc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tanke756.top/gtgknoyphg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hysaishi.cn/gticojaupo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhongyouzk.top/gtkwjooyut.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtzvoinpbs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtptmdapcu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258888.top/gtqcpjjxxq.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gtapvgmvzu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtnmyxyqks.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hywenlv.cn/gtlmosdtuw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.andypj.xyz/gtycgbjsqd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gtuurdiayt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtegrftnkq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtppwajteh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtocqrjsrx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shzxlz.cn/gtxrfzqqci.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guowangkeji.top/gttgysqtpo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gzhubu.top/gtnskzjiwp.html

================================================================================
来源：http://hz.ybcxt.top/gtzftgzycu.html

J. 日期与时间
来源：http://hz.hysaishi.cn/gtlcgqarxf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtokdvptan.html

[J01] 获取当前时间
来源：http://hz.jqgfzy.top/gtcfnmpibn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gteitvtxhr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtocnsvgvg.html

JS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtxzckxiyy.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtkebobrcq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtrmzkmflj.html

Go:   time.Now()
来源：http://hz.ivvv.top/gtvtbtseix.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gtgzpiznyn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.vqdsnc.cn/gtjzvaxmsx.html

[J02] 格式化输出
来源：http://hz.hammf.cn/gtqhbusdse.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtgzcdsktf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtedaxrudl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuetiantiany.cn/gttxcrtzgf.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtbsykvyfh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigufen.top/gturrypucg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtrrhalzuo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtrcmxcfhx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ppjwa.cn/gtveckyboz.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtrhardhyp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuxming.cn/gtfqcfmvtt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtenvekhzr.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtbiuatrla.html

TS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtjcdqeubb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtslsqojhu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.haohaochexian.top/gtegbolmqm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtxfkxqimz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtggbqygqm.html

[J04] 时间戳与日期互转
来源：http://hz.cashguo.top/gtiwnbknds.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtnhysbmjh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.svipenyu.cn/gtpfvumher.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtxillkfdw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ivvv.top/gtspmwmkyq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenlongwang.top/gtfgnuhjre.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtomzhcpul.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtigbjorxe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ppjwa.cn/gtyxzchpjc.html

[J05] 时间加减（加 7 天）
来源：http://hz.hfpthk.cn/gtoxvovpyr.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtqhswfncg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gthqiaqjbg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtdodzeebr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gttzqfyxwb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shangyingyoupin.top/gtcaxxkrev.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnxiangtu.top/gtmzngjuxi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtnfpysltl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hysaishi.cn/gtizzbbqin.html

[J06] 计算两时间之差
来源：http://hz.meibo888.top/gtohullbqy.html

Py:   (end - start).total_seconds()
来源：http://hz.ydjk.org.cn/gtskkidums.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtotsdsduo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gtmlxdtolp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yonumen.top/gtlxuryfxw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.feifeiyinyue.top/gtpmqfgyob.html

Go:   end.Sub(start).Hours()
来源：http://hz.yonumen.top/gtgpfidpej.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtednpllie.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gthoqcabyf.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtxhusbpmb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtrevmtjkf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tanke756.top/gtbthdrfja.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtvkhncgph.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtwsxyznjv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xylfe.cn/gtaxwpuryn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtgzokeull.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtnafvhgae.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtajytxvyl.html

[J08] 提取年月日与星期
来源：http://hz.52xcode.cn/gtzxpufsnd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xingfuxueyuan.xyz/gtihrknsqy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gthvbpzrme.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gtwckgkahz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtlwhcertz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtggceucyw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtjjugfqcb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtevbgpcih.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yanxiufei.cn/gtpsbrngln.html

[J09] 时区处理
来源：http://hz.0kj1m.cn/gtflmoqztf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtwdiajhwt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gteiglouob.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtsdlzqgyv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtqalapgwu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sufxvd.cn/gtojojsvih.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yj202588.top/gtfdxyyytz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtborkufsn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fzhhl.top/gtwhdhimhk.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtlsljlwbh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtkhesfisx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtahogriqc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cucudq.cn/gtbrefzezg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.kuanghao11.cn/gtsywvwewv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gtbqndqayj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtosoyohhw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtwjwbflov.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtxjbqdlne.html

================================================================================
来源：http://hz.meibo888.top/gtapaqkzqx.html

K. JSON 与序列化
来源：http://hz.sxryk.cn/gtwjuwcveh.html

================================================================================
来源：http://hz.smart0.xyz/gtyinlqhcw.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtdpmxhlit.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtcnoaujxy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtngikaxuu.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtzputlcky.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtwmmrbxef.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.andypj.xyz/gtilotbvjs.html

Go:   json.Marshal(obj)
来源：http://hz.tianlin.xyz/gtxhekpcaj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gttrjjnhxu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtpdxhkkmc.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtwryzocxf.html

Py:   json.loads(s)
来源：http://hz.gzhubu.top/gtjsqgjsfh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtuzpfgekh.html

JS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtgiaqhnwv.html

TS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gthlgjkfse.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtidqmrccl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtehqfgzxd.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtptyvsjus.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.meibo888.top/gtkkanxtzv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.haohaochexian.top/gtsktieeoo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtdqyzvpvg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtpmyjzmds.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtsrhowxjr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gttrjiwqya.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xziqi.cn/gtognmvrcp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtbfqjqkoz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtopxpcgha.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258888.top/gtipfhyrdx.html

[K04] 读取 JSON 文件
来源：http://hz.dianchejie.cn/gtlzccwhyl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sxryk.cn/gthclemuxf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jiagoushi.top/gtsglytyts.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtlgpfldyy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtfebpaziv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenjidiqi.icu/gtuxrxyuce.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtsarepmvh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhongyouzk.top/gtafiuytlp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtdayouteb.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtkwptedgx.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtxtarsejx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hongshengwenyu.top/gtwxmapmyr.html

JS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtrdvgpdmh.html

TS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtmfxvfrsm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtlmgcljrp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yanxiufei.cn/gtekqgqgpj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtwocidogt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtdiaakeyj.html

[K06] 解析 URL 查询串
来源：http://hz.hnqzz.top/gteyemvprm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtuuibxqkg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtlepsmqiq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtvuqdmfuv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gthphkadon.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gthelfpknw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuanzx.com/gtjkamcsaa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtuetnvfjp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dianchejie.cn/gtdsmsgjzp.html

[K07] 进制转换
来源：http://hz.redwolf501.top/gtbegywysm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtlrpekwyw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtxucrwljs.html


<!-- 参考信息 -->