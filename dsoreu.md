代发 wailian999

H. 异常与错误处理
来源：http://hz.yvedp.cn/gteajwcehl.html

================================================================================
来源：http://hz.zycfv.cn/gtlpnsnyqd.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtkribodhm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnxiangtu.top/gtfmxqijye.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xziqi.cn/gtpanodeta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtrazscymm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtwcwtuipq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuanzx.com/gtuglsgcqo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuxming.cn/gtbtlfqrps.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zdqjudy.top/gtvlasqbyg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.andypj.xyz/gtbkcdiepj.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtytvbfbxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxuanxn.top/gtxsegskoh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gttvjynizv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtapelizxx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtnohbyrak.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtsessiewy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.feifeiyinyue.top/gtmbtfwccq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.fzhhl.top/gtjiytfnks.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtrqthjoun.html

[H03] 主动抛出异常
来源：http://hz.jinqigfzy.top/gtvmudiheq.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtucyqiecu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtmkjsvuaj.html

JS:   throw new Error("错误信息");
来源：http://hz.jinqigfzy.top/gtnqeyetba.html

TS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtarhvwecd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtlsqlisko.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tianlin.xyz/gtumluxoif.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtroswdcot.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtakspekfb.html

[H04] 自定义异常类型
来源：http://hz.yj20258888.top/gtnndjswvu.html

Py:   class MyError(Exception): pass
来源：http://hz.svipenyu.cn/gtakmmmwwm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtzkzglewc.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtlbkhajpv.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtmchgmcaa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yueranfly.top/gtjfzxpsjz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hongshengwenyu.top/gtuwizczcw.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtafinntkv.html

C#:   class MyException : Exception {}
来源：http://hz.hammf.cn/gtzhirwmix.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangtech.top/gthcdvwigy.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtzdhiavsv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtplenyehi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtypseylli.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtudefzyxg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtedjieltq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tian-w.cn/gthwkmeuev.html

Ruby: rescue ArgumentError => e
来源：http://hz.redwolf501.top/gtfbcsqoyh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtilzrpims.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtlisizazh.html

Py:   value = d.get("k") or default
来源：http://hz.ywan-chungtsiang.top/gthhcqajmm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtmyvsjqso.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtrwpdoeih.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtwnagybmc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtynwqpovp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gtiyyfawzq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtxskfukmw.html

C#:   obj?.A?.B ?? default
来源：http://hz.sweek.top/gtxgtqksme.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtbvxcrxgv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sysykeji.top/gtgjhcvyrx.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtriscmbwf.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtncdwbgxk.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtjrnocbhd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtshmkughz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.birdmap.top/gtoxztknup.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gteztbgkju.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtcvbkmizw.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtefvdpulg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daria6918.cn/gteadruteb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhongyouzk.top/gtrrmyqkrl.html

JS:   e.message;  e.stack
来源：http://hz.aibaodan.cn/gtdpplvsui.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gtmksqujio.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ivvv.top/gtseczgqeo.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtmrxtguxq.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtipbataxc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.vqdsnc.cn/gtnqepsyuu.html

[H09] 带错误码的异常
来源：http://hz.ppjwa.cn/gtuehykkxi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cucudq.cn/gtveveorke.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtszifasnx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydjk.org.cn/gtzwwcpefv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gtgtgbkhzm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtzmvpqxur.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.0kj1m.cn/gtooufcnbz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgufenzy.top/gtrtfwtnfp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtructrgaf.html

[H10] 资源自动释放
来源：http://hz.hfpthk.cn/gtnfbqmayk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ppjwa.cn/gtolyzkowk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxinkj.top/gtvfzssbia.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtztkmgdkq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gterzstklf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtrvxkphwp.html

Go:   defer f.Close()
来源：http://hz.xziqi.cn/gtyeeqewds.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gtsiasdvbl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtjykfkibs.html

================================================================================
来源：http://hz.aizwys.cn/gtaqpqoktk.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtmbthnizy.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtoosqtiiz.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtqgrdmmpu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtqbxmsryf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangdashe.top/gtrrvngyzk.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtuultxplm.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtcdployzv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtheyudswf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guowangkeji.top/gtymnjqixr.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtubajqjzd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gtfjousoqa.html

[I02] 提取所有匹配
来源：http://hz.jinqigfzy.top/gtzypfaiwo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtrrxagvfh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.feifeiyinyue.top/gtmxibucuy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gtvkyirrtz.html

TS:   s.match(/\d+/g)
来源：http://hz.feifeiyinyue.top/gtydqeihav.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtkfzcqtgq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtyfxpqone.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgfzy.top/gtekrwptmy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtqbydtaih.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtxrkaacde.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtbulromsp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gogol.net.cn/gtislurate.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtbvrquqtx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.birdmap.top/gtyjrhelve.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.316326.xyz/gtmryfgpmn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtnszmdsfo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sweek.top/gtibhkeoel.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhengqikj.top/gtamyccrgi.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtpcqaeess.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xziqi.cn/gthcckhlpb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtsyotckvj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtcnpmcymi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtbfbbzwwy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gtekmcxedw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtfhfopmdw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtuywkyvpq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.svipenyu.cn/gtefsfsxlf.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gtaldqrmlm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gtpxdtakiv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ppjwa.cn/gtnsdmlpmp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtdpxrkgoq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gthrxlpseo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtvqmerjds.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gtcrybqnbt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtckdqkojn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ehwqpu.com/gtgyliyeny.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtnmdsjeno.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtddulgpqs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.andypj.xyz/gtfchupvad.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtopvwuhrj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gtjyteygwh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtuhvziiuf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nwbrower.top/gtjhbsyphl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtyrwqcoxi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtuetasnjn.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtfaywtavt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigfzy.top/gttfpocixx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aibaodan.cn/gtdrqganab.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gthnyeoycs.html

TS:   /error/gim
来源：http://hz.dashuyun.cn/gtzdmypuqi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yueranfly.top/gtjtstqoum.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtrkyqzcly.html

Ruby: s.scan(/error/i)
来源：http://hz.cucudq.cn/gtsdfezprw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtaojfwdde.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtdovkehik.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.316326.xyz/gtkgaryglp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtjikibaub.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtonejjtzg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtqympqqag.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtgrpocztf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtiolbyubq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yvedp.cn/gtwbmwyhtj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtnzfhmhlc.html

================================================================================
来源：http://hz.ybcxt.top/gtzzfdduka.html

J. 日期与时间
来源：http://hz.yvedp.cn/gtgpigwbgh.html

================================================================================
来源：http://hz.dashuyun.cn/gterrygjsm.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtprqhddgv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ivvv.top/gtexugcock.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtmncympbh.html

JS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtnmawnbpu.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gttldtxsvd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtkpywxfyr.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtbwfouupq.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtlgryzdal.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtjbtclugw.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtizjwzrvg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtdpywkkqf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtdhmnjphw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtveukmfus.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gtlpzivrrj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hysaishi.cn/gtmnogahyw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtogectukc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtbahmocsc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtcnswodti.html

[J03] 字符串解析为日期
来源：http://hz.redwolf501.top/gtyuorvymy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gticrhiurm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtlvvomirw.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtoggyrckb.html

TS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtirsmmfeo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtpvqanyli.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtikewzcvt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtwhkfwrsv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xinyue.icu/gtwnbxhjyg.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gtqpwrbxmn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gtywhmctjf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.meibo888.top/gtgpxxytav.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gtiqyroabl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hongshengwenyu.top/gtakuepzkk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gttxmbanqq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gaohongyu789.top/gtybolqhes.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj202588.top/gtmiogniyx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jlsjyb.cn/gtqavljqjb.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtkpvrlkfw.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gtpfmoiqnc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yongpay.top/gtptaasztb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtsxsbzmrp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtmhkdnjft.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fzhhl.top/gtkazhphkd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhongyouzk.top/gtpidtexsf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gttcswtstm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtbuqlfhft.html

[J06] 计算两时间之差
来源：http://hz.yongpay.top/gtqeqmlcxl.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtewykiqey.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtszjwjtsv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtqmdmdvxy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gturkxatji.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gotoacloud.top/gtbisakfgj.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtnzwlvhod.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ehwqpu.com/gtaglfywgg.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gtrvzhsnpc.html

[J07] 比较两个日期
来源：http://hz.gaohongyu789.top/gtufmfohkl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtbhbrxlyk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gthgkfqdpm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtpfizvxhq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtdezxwrbp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydjk.org.cn/gtosavzvsu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yueranfly.top/gtifjgfetp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtlasaftrv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtnahnfluz.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtmkhznqjf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxuanxn.top/gtovoeihrv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtweiynqnu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gtqjiefkgm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtpnptgyql.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sysykeji.top/gtrxaewqba.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xinyue.icu/gtrvpdsets.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jlsjyb.cn/gtznaxcfwt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhixingplan.top/gtknvgvrjq.html

[J09] 时区处理
来源：http://hz.zhongyouzk.top/gtvglncwch.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pengpengdd.cyou/gtutlnxjfg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cashguo.top/gtuqssbavu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtgrpfdjqr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtzmomeaeg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtgjzrswec.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtxkhvjiez.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtjtcjsite.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydjk.org.cn/gtxxlkfzxj.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtrqjjcamk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shzxlz.cn/gtphawmgcn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtgkmwrqgc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ywan-chungtsiang.top/gtepxsiijb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.mhx1999.top/gtdzmlkqjo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtqdfigbsc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gogol.net.cn/gthbcceeli.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtuxhpysdb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guowangkeji.top/gtohkoysjb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtagcnnflq.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gtwbjdacxy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtuabbcmsk.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtplnaipxo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtgypcutzz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtxxrzkksd.html

JS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtybyrtxlq.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gteylkcmpz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtyijsgyzz.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtasjecezz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtuvosppsg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gtgvitpwjk.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtgetuozjq.html

Py:   json.loads(s)
来源：http://hz.zhiwuduotai.top/gtzkidbefn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gtqyyfkzxb.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtfuvsughc.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtvujzdtll.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtkujreusj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtsivabkoc.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtgirwhchy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnqzz.top/gthatdraix.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhijiandao.cn/gtgwebaeff.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtznnwjhls.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.svipenyu.cn/gtgmlfurxb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtpniwdmrb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtfcabvqzx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuxming.cn/gtnmyevvco.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtgulsyzid.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zdqjudy.top/gtmnsxaieq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gtzcknkxon.html

[K04] 读取 JSON 文件
来源：http://hz.tanke756.top/gtkqvhobhb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.meibo888.top/gtidcdrymr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gaohongyu789.top/gtpfmeyafg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtyuumbeua.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtlvggxzld.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gteedmlxsh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtjeujjcrv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtmdmgjmua.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtjaxvgwqx.html

[K05] 深拷贝对象
来源：http://hz.jlsjyb.cn/gtfblcavvy.html


<!-- 参考信息 -->