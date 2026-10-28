代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtlvvbwwgx.html

TS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtwwausgwl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtliwplowp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hongshengwenyu.top/gtomdcwgnt.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtlechqteu.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gtgzigqofx.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gtjyjjdwmf.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gteecnhvfg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtyqhitnxt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtkosqmobf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtktieljyk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guannengcc.top/gtsrytghug.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtkvdkjwjw.html

Ruby: rescue ArgumentError => e
来源：http://hz.gaohongyu789.top/gtqsninryt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtksexrbac.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shangyingyoupin.top/gtzesslnmm.html

Py:   value = d.get("k") or default
来源：http://hz.yuxming.cn/gtywgxorza.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shangyingyoupin.top/gtzxrebgyc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtlxjlbuna.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtshktcoka.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtfomkmqmi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtzpjmvaks.html

Ruby: d&.dig(:a, :b)
来源：http://hz.bjfxy.top/gthklxibde.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtotlfzqdp.html

[H07] 断言
来源：http://hz.svipenyu.cn/gtcbfuacxm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtcuhnmhyo.html

PHP:  assert($x > 0);
来源：http://hz.zhoulong.xyz/gtfgzltbna.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtntzaepor.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtabzofgdf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtbgbnvkeo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gtmsmkfhfa.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtwotykmdh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xylfe.cn/gtwebpikrx.html

[H08] 获取错误信息与堆栈
来源：http://hz.andypj.xyz/gtppdtqqrh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gaohongyu789.top/gtplgpjpig.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinyuanbaomall.cn/gtofdtowge.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtyfsaajma.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtfxazrnab.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtbvvrdpgv.html

Go:   err.Error()
来源：http://hz.52xcode.cn/gtiijvuaeo.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtxowvwtsg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtyishoanl.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtvhlbmbtu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gtscibhymj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtgjdrzqwt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtpyvugumx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.52xcode.cn/gtliiuqmdn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtqjrbfngy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtssonogai.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtguifvoag.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hywenlv.cn/gtsiwnvoeh.html

[H10] 资源自动释放
来源：http://hz.yuxming.cn/gtaxakppjw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtirspcfxk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hysaishi.cn/gtvgbptbkp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gtajtqezls.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtfeolnpbe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhiwuduotai.top/gtnnuqkhyb.html

Go:   defer f.Close()
来源：http://hz.jianghu66.top/gtmtwzufwk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shuidangran.top/gtwasxiamn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangdashe.top/gtifiweehk.html

================================================================================
来源：http://hz.dashuyun.cn/gttbetofpm.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtbbsamvwi.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzsmgjbyl.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gtpwdhzdfm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtdkorzwrh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtqqrwmpaw.html

JS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtfwnjuaia.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtfmubhpmc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtpmsnlfqp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtmkrqcjkt.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtegsqrafr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gtvfpplkfv.html

[I02] 提取所有匹配
来源：http://hz.9152youxi.cn/gtfscwrkjs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtesadxkrc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtxwpnfdxi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yueranfly.top/gtoajrryvc.html

TS:   s.match(/\d+/g)
来源：http://hz.zhaomingkeji.xyz/gttkwmqati.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtwongyuzs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.52xcode.cn/gtemsgmjyt.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtmmzihgds.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ehwqpu.com/gtiifwiqej.html

[I03] 提取捕获分组
来源：http://hz.iojbl.cn/gthhwfqphd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.0kj1m.cn/gtyglcuqhu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.iojbl.cn/gtchjwqyjy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtbmlrpeos.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuanzhike.top/gtbicbhabg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangkeji.top/gtjekmajyy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtbioahvpb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtsayaajxp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.svipenyu.cn/gtsaneywjq.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtkapjfhls.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtgmpkhbpp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtcouoadcn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtynpfpfop.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtizjeklnv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gttlmhwdex.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenlongwang.top/gtybotnran.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.316326.xyz/gtcivwpshp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gtadkhxlmm.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtqpddteja.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gturyvkled.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gtjotrpxvu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtxxkpgzpx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtiqgiyngw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.pycfn.com/gtkabaemot.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ppjwa.cn/gtympxwgux.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtmascdhup.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.feifeiyinyue.top/gturimscoh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtjdgfccsi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtnlxjzixm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gturxbuoin.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtczfixrkz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtoypkqpqr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtqeoteccm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.meibo888.top/gtzlmhoohn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhoulong.xyz/gtqxdejfrt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtmvmhzuoe.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtqbeissfi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.meibo888.top/gtvmljllvp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jiagoushi.top/gtfogpmnlw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtksttvixh.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtsawcymtk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangkeji.top/gtxsyfxgqz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.smart0.xyz/gtegbulbfg.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gtmksijmef.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.mhx1999.top/gthbfsiuqh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.svipenyu.cn/gtlwjmiyth.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtrikqxwff.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtjiufuqkl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtafzbhqwt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtmhpldomj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sxryk.cn/gtulqdxspu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuxming.cn/gtwccgcwfr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtvusheuch.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtjvhymwsd.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtakrxbzcp.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtpksrwgei.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvgxdidzv.html

[J01] 获取当前时间
来源：http://hz.havefunace.top/gtqthbaybu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aibaodan.cn/gteizxsfiv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtircjmpsj.html

JS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtpttnichz.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gthabypixi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gtwepwvzfj.html

Go:   time.Now()
来源：http://hz.xuetiantiany.cn/gtacxitrxg.html

Ruby: Time.now
来源：http://hz.jianghu66.top/gtgiwqieso.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtbjtqtjxj.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gtauuhsqsy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtagjkacpu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtnuxmnvrh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtatgzvlgj.html

TS:   d.toISOString()
来源：http://hz.ydjk.org.cn/gtjxzgrfit.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jlsjyb.cn/gtbdhupxgj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuanzhike.top/gtyvwdlufc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtmhxhtird.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtgoqxwzal.html

[J03] 字符串解析为日期
来源：http://hz.zhiwuduotai.top/gtehtxhhyb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydzc1.top/gtaoeyykbu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtccmsvhsa.html

JS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtwkjlvyzu.html

TS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtyenwjvmr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtmtrnokrx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gtupvbvsbw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtdhbzlygg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtgeucbmqz.html

[J04] 时间戳与日期互转
来源：http://hz.bjfxy.top/gtfajgrxva.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yangfankeji.com/gtwfmejawj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shangyingyoupin.top/gtygpiksyu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ehwqpu.com/gtkfmrhned.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigfzy.top/gtkhcvgqaz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxuanxn.top/gtpdrrmees.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtpnpoxahn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtpfmjucwt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhijiandao.cn/gtxffpbjcn.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gtfohvtyzc.html

Py:   now + timedelta(days=7)
来源：http://hz.xylfe.cn/gtgbthoslk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtxlxucvht.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtdvmuhcnz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtcxrjqpru.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtzmqdhrsz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.mhx1999.top/gtyfcahxdl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhongyouzk.top/gtxxpkbwzu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gtahvscewd.html

[J06] 计算两时间之差
来源：http://hz.dashuyun.cn/gtfuamnuza.html

Py:   (end - start).total_seconds()
来源：http://hz.zhaomingkeji.xyz/gtlaxrakha.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtltcfxugx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gttovwgcgp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gtefdwayzr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtdglehhgg.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtkybirkij.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gtemnawyyv.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtdwhbqfrh.html

[J07] 比较两个日期
来源：http://hz.nwbrower.top/gtnsihshvr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtaxbpuwbx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.birdmap.top/gtctnmspya.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtwaupewdh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtqfvyxmww.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtgiynzulq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.c1oappe.top/gtlazktehd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gthrdfwont.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gttxhfosgb.html

[J08] 提取年月日与星期
来源：http://hz.hammf.cn/gtpgulzsdn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtimofvhsn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtqzqfvedd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenjidiqi.icu/gtzeiuftgl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtndkfilfc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtgjrfxzeo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sufxvd.cn/gtyqqaifio.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtypuvspuu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnqzz.top/gtwovyrmgk.html

[J09] 时区处理
来源：http://hz.quarkkingdee.top/gtchsgeefr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtolydkeif.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258888.top/gttezfsbfv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xinyue.icu/gtmojamztn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtawbrjlqj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ppjwa.cn/gtdwifqbne.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtjkdfdqha.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxuanxn.top/gtbblwgwzx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtgyvecath.html

[J10] 取今天 / 本月第一天
来源：http://hz.hysaishi.cn/gtprfoebsa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guannengcc.top/gttkqfyiqw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.smart0.xyz/gtmqvepfyw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.quarkkingdee.top/gtaowycach.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.316326.xyz/gtfwdblaqn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtwjiuxeqc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gthbwinevq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gtvdfghwif.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.52xcode.cn/gtcrtahsha.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtfvcgbtsu.html

K. JSON 与序列化
来源：http://hz.daria6918.cn/gtrawevczd.html

================================================================================
来源：http://hz.ehwqpu.com/gtxaulgbwz.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtahckrtmd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtiwoxulbu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.vqdsnc.cn/gtvpjhnbce.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtlgwemzde.html

TS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtcdnartyf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtirfnamqq.html

Go:   json.Marshal(obj)
来源：http://hz.c1oappe.top/gtxzppavuz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtsvfxiqyl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtrcocbxwy.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtyxnagujs.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtamgsiytl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ybcxt.top/gtuoulupwb.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtczdvucjs.html

TS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtyxjuobga.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ivvv.top/gtkhtjgcpz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtjhellnrk.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtkafgslds.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuanzhike.top/gtgwidolfr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuetiantiany.cn/gtalnbykql.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtuhanryoz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtauagfgqu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtdgqbkngy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtqbxjpjvu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ywan-chungtsiang.top/gtycykisnb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gturzlcwqe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gtpxmyrikd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenzaomai.com/gttmibxmdu.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gttngvofdi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtbokeogzh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtbojhcfsr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtapagvlkg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gthzbosovs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gttiusuxst.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtkrwpaxlu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtsibyulpg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nwbrower.top/gtzwkgborp.html

[K05] 深拷贝对象
来源：http://hz.ybcxt.top/gtanlafzye.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtchnuwdiq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtqsnbaglf.html

JS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtptqiurkj.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtcvfwvinp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cdnleiting.top/gtpqkawjsr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtnqvwhlvf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtvtebjclg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gthszblmqd.html

[K06] 解析 URL 查询串
来源：http://hz.yueranfly.top/gtpubuqgvu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtweauwhor.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtneqpfuns.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtcutlralr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtngcbquny.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtemnlxiik.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuxming.cn/gtxjicqdpp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtrxozqsci.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtddcpmofn.html

[K07] 进制转换
来源：http://hz.zdqjudy.top/gtvwwmkgfj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtokpdensr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gtiuurwhli.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtlksfklzi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtbyhyfenf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtupkufqtu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hammf.cn/gteylwwpaz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.redwolf501.top/gtjzsrqgql.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtmdenjgts.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuetiantiany.cn/gtdxgmidqv.html

Py:   pickle.dumps(obj)
来源：http://hz.zhaomingkeji.xyz/gtlrvxkdkj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tianlin.xyz/gtrcihcpfv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtgmiycfdh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtjxxbaldx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtdsgvywkk.html


<!-- 参考信息 -->