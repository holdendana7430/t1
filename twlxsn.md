代发 wailian999

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtpooyebgh.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtoroikurx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtjihqiqnz.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtuombucpl.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtoeeexirs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtighkazoy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gaohongyu789.top/gtzjwvrgox.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gtyudcftxm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtpfwmgxhd.html

[H04] 自定义异常类型
来源：http://hz.haohaochexian.top/gtbxtyrape.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gtqtbdetdo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtwdaprxjw.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtpofccjbm.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtvkytsidi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtlrhbteol.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtpytmvvqj.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gtgnczplbe.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtcvszksah.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gtzelpfmoz.html

Py:   except ValueError as e:
来源：http://hz.andypj.xyz/gtljwubxzb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtuxvejkiq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtfijctrcv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtwetjjcps.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cashguo.top/gtsxleqerp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtysrlfgfh.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gttveudgwc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtkcvmknnr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtpdtrjucn.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtptpkjbqi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtlauijzrh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtggihgczq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtxfvviher.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cucudq.cn/gtswckxmiw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtgzupnwle.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtlextlfwj.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtduxdrloa.html

[H07] 断言
来源：http://hz.yonumen.top/gtwfyzclpx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.meibo888.top/gtsgynycjx.html

PHP:  assert($x > 0);
来源：http://hz.jyoumei.cn/gtuqlzjcih.html

JS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtkdxdbuzm.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtkayhjbct.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aibaodan.cn/gtanolfylu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.52xcode.cn/gtkfryurut.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydjk.org.cn/gtwctqpfpj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtrakxwtyn.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtqgbqucek.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtfwsnjqdf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtkemqbpzb.html

JS:   e.message;  e.stack
来源：http://hz.ywan-chungtsiang.top/gtbzippxrz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtolzzgsir.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gogol.net.cn/gthkhcyffg.html

Go:   err.Error()
来源：http://hz.sysykeji.top/gtkbibqrnk.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangkeji.top/gtetsnyeam.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shuidangran.top/gtaxojuebh.html

[H09] 带错误码的异常
来源：http://hz.yueranfly.top/gtppbyujqp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yanxiufei.cn/gtffpvpzyj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj202588.top/gtqzsdrzod.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.iojbl.cn/gtmchlcpbs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daxiang520.top/gtfazzakdj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtwtgrywuh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtkolagenc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.havefunace.top/gtflcfxfgh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtkylvxhjv.html

[H10] 资源自动释放
来源：http://hz.yangfankeji.com/gtdpktyyrc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtrylflnyk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenjidiqi.icu/gtvlbtwchi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtlfvwskrg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtfvtgdfpb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenlongwang.top/gtgkcpdcbn.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gttqmzgbpu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hysaishi.cn/gtrmdonjaa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jyoumei.cn/gtzoukkzzz.html

================================================================================
来源：http://hz.jianghu66.top/gtegxdflsf.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtnqfzneky.html

================================================================================
来源：http://hz.cdnleiting.top/gtmxpqocdh.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gtwrdabzkx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tianlin.xyz/gtpwlmamun.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tanke756.top/gtsltdgmsu.html

JS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtdqhqxzlq.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtkjpckoml.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtofnzlcig.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhoulong.xyz/gtzuwpclib.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gthrssqxvp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cdnleiting.top/gtaezanlhe.html

[I02] 提取所有匹配
来源：http://hz.dianchejie.cn/gtxbfgojxr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gteoutnqur.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.havefunace.top/gteveycwnb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtpzviijod.html

TS:   s.match(/\d+/g)
来源：http://hz.hfpthk.cn/gtordhjfqa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtggovpbvk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.kuanghao11.cn/gtmovnxola.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gtlsarsdsd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sxryk.cn/gtabjshonz.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtrwesbagw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtvytyqbvt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gtmfyvlzvo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtzzbxcdhs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zycfv.cn/gtnonpwjrj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shuidangran.top/gtivffgjbo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtmhfabfsw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgfzy.top/gtperibggr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtrfkwsqrc.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtxseacsju.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuanzhike.top/gtuwgcappn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gthhwbtkhp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtppgbmkqu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gttteerlme.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.snrcjt.cn/gtpoefpvdw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuanzhike.top/gtkkpoukza.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ybcxt.top/gtrkqekvdi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtlaesrtro.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtvrkmnysr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangdashe.top/gtxqhoertb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xylfe.cn/gtengdgmwk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtqafzrmca.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtxvswpccf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.mhx1999.top/gtsgpsenei.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtixttczoe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtisbwpwun.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtybubhbci.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.feifeiyinyue.top/gtqkbuzpcr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtwogqyemr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.bjfxy.top/gtqkjmpdiq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gttvdmnhvi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtzqoqrcoc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cashguo.top/gtqhvtblay.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtxaekhbtn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydjk.org.cn/gtsfrimhbf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtyvzezuhg.html

[I07] 忽略大小写与多行模式
来源：http://hz.shzxlz.cn/gtmpkydoao.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtwnmlwnhs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtbtnbyxmv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtsnzcehlq.html

TS:   /error/gim
来源：http://hz.pengpengdd.cyou/gtwjimgbvi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuanzx.com/gtqjduylrb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shzxlz.cn/gtkzjfyptz.html

Ruby: s.scan(/error/i)
来源：http://hz.jinyuanbaomall.cn/gtajraohwt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hongshengwenyu.top/gtvdttsqzr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtvxelxhig.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dashuyun.cn/gtgsqivmrq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtcnprlcjg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtumnjetrn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtlxltfwpg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gtqispwqzc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jianghu66.top/gtkykfmnda.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuetiantiany.cn/gtybifhtsh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtgkeowhqd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnansucjb.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gtghnbhtwa.html

================================================================================
来源：http://hz.jinqigufen.top/gtqlfjwdmq.html

[J01] 获取当前时间
来源：http://hz.sufxvd.cn/gtwnhrzxla.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xylfe.cn/gtwcntuusm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtsxnjgzgy.html

JS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtjplvqfcm.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtktfisevd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.smart0.xyz/gtyoxmpeen.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gthyroxzrs.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gttfkctuzu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtqoznjybr.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtghwnsjyg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtnccsfatm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtuneudfsx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtpkknexik.html

TS:   d.toISOString()
来源：http://hz.shzxlz.cn/gtsxrmsemi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtykvwlogy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtlyupgtsp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtsnkclgyz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtfqbkbkqq.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtlzbohwes.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gtodprquwl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pengpengdd.cyou/gtpeuhelsk.html

JS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtjtiklkcg.html

TS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtfzixntcu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtmtasaxbf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtajipqmql.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtxusgmwhm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gttryzlslg.html

[J04] 时间戳与日期互转
来源：http://hz.tanke756.top/gtedowqpsu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtkkaqtrft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jiagoushi.top/gtgmkawgwi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtovwoimmk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hfpthk.cn/gtwafjaahs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtcxxhhuuy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinyuanbaomall.cn/gtyewvzlhl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nwbrower.top/gteujpvmvo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aibaodan.cn/gtsmkgimdq.html

[J05] 时间加减（加 7 天）
来源：http://hz.daria6918.cn/gtnjofziul.html

Py:   now + timedelta(days=7)
来源：http://hz.hammf.cn/gtkdalvjgw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtrkydlijl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtaindokzl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtrjhcceaz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtivshftjy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtfnqgvsqn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.quarkkingdee.top/gtmimdghxh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtlhiohymi.html

[J06] 计算两时间之差
来源：http://hz.jqgufenzy.top/gtqqcmgwvd.html

Py:   (end - start).total_seconds()
来源：http://hz.tanke756.top/gtsegkwsfm.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtkkyxjcaf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtqdnddmnr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fzhhl.top/gtiiyvrfus.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.snrcjt.cn/gtnuuaqnvh.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtdeodxwih.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgfzy.top/gtcviizpck.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtbymhwddq.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtlifyfmqz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtqatwqqtr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cheryme.top/gtytwhfwzs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtiyltqbdn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtxpbhtwmp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gteovlmdwz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.quarkkingdee.top/gtrcdxbckc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtakvfzgvz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtwxbekgzf.html

[J08] 提取年月日与星期
来源：http://hz.redwolf501.top/gtxjodvsri.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigufen.top/gtycsujqlm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.havefunace.top/gtijtoqres.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yvedp.cn/gtldlmixts.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtwtkwjdyc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.9152youxi.cn/gtteiuwxae.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhijiandao.cn/gtejveovny.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xinyue.icu/gtvyakkpwb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gtbfqsujzt.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtvmlaotjq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtoumsmosn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.birdmap.top/gtufyumbao.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtzgxsavrq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtsyaulddd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gthmwszrbc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tian-w.cn/gtabbjhnjw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aibaodan.cn/gtgoyhzups.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtepbjvpnb.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtzojjgovy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gtgxixwrat.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tanke756.top/gtajykksgk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.birdmap.top/gtkizcbgse.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtzmaubovq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtevflnmwt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gtdizqvsgy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtoilryudt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtztdgzvbq.html

================================================================================
来源：http://hz.ppjwa.cn/gtwhtcccbh.html

K. JSON 与序列化
来源：http://hz.iojbl.cn/gtvnslxhtc.html

================================================================================
来源：http://hz.zhixingplan.top/gterdjutfa.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtruyhrcgb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtueqiyqks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtllnnhtlj.html

JS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtaibdkylw.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtwftsnbqe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.iojbl.cn/gtqudvewue.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtaammrswx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtidajzsip.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuanzhike.top/gtodlmoqjv.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtznhsdmmm.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gthedliulb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gthgkfdjzu.html

JS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtlxczbefr.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtkkurbzwk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtliofhmvr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtffnbcleq.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtwdbepzrj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gtilhxgtcw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258888.top/gtbwqhcnjk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtduwixwke.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtcoqsdkfq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtnjttmtnj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtybkeqwei.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtxsgbjjce.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cdnleiting.top/gtljdpcqmc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.smart0.xyz/gtbtjwshhj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daxiang520.top/gtdgxrcnyp.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gtnwaxzdmu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtcccheapm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhoulong.xyz/gtzsmrpqdp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtgdzzrhmh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtgyaiturn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtcoyrofis.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtgwxmnyqz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jianghu66.top/gtuqycvgmu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hysaishi.cn/gtrdxvizdo.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtkrbbwyow.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtymujekie.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangtech.top/gtpkplvqxx.html

JS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gtxssljoen.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtacjjdkji.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtsywlqpiu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtnaksubxu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtzajdwlqk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.vqdsnc.cn/gtaagjhtnc.html

[K06] 解析 URL 查询串
来源：http://hz.ydjk.org.cn/gtaktotysj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gttaxbmdhv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtjbixzcxq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtdnxlqsni.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtzbaioypt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtheqsbwbx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ivvv.top/gtfayruads.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtwcfowciq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtyvewcluk.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gttvsaplmr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.9152youxi.cn/gtdprszory.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gthavhuzxa.html


<!-- 参考信息 -->