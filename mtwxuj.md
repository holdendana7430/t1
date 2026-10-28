代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtrynmrnlp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtisofdyti.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtahlcqiyd.html

[H02] finally / ensure 收尾
来源：http://hz.jyoumei.cn/gtadrhdjak.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtinovhlqz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtfsrqzgdo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtabbwscpg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gttdkdpebk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtiqrgpskn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuxming.cn/gtntqpzoqp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sxryk.cn/gtibagievt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gtrauixxol.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtdaolhjgq.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtbtxxcdak.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtiqgncbpw.html

JS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtmptxlrqr.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtywsagfst.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pycfn.com/gtykwcckmm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtmjiviiyd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtmbtmuvjw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtnvagxswe.html

[H04] 自定义异常类型
来源：http://hz.ydjk.org.cn/gtxuarrfzp.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtlydwpfoe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gtksrxefpy.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtmfimpqru.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtvqkrusxv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gtmcxgrepd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtslpustwe.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtqqwxjdzh.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtwuvrkfpu.html

[H05] 捕获特定类型
来源：http://hz.zycfv.cn/gtpugokpwm.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtzqmxqyzq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.havefunace.top/gtjqyapyfz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtvfleitwj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtlfsjibzq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtdsvkbetr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fzhhl.top/gtzdqvrats.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtxjngwyik.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtsgallcbg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sweek.top/gtadbvkstm.html

Py:   value = d.get("k") or default
来源：http://hz.chenlongwang.top/gtcemtvdsm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtxmyjsmlk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtunvtjowd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gterylkyeg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtzmiygmmc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.iojbl.cn/gtjnjpigbn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gtszryzbpg.html

C#:   obj?.A?.B ?? default
来源：http://hz.sysykeji.top/gthhvdhaas.html

[H07] 断言
来源：http://hz.nwbrower.top/gthitcrxhi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtfwcsojaq.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtnjbsgmzm.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtzbwruufu.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtmkbdtjin.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daria6918.cn/gtmofpulkp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hywenlv.cn/gtgvkbfthz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yongpay.top/gtnaaczpsu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxinkj.top/gtujszfoqt.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtdeshhbcn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxuanxn.top/gtgesdmkhp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtoudafrjb.html

JS:   e.message;  e.stack
来源：http://hz.xuanzx.com/gtpgjohjow.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxinkj.top/gtopsuauov.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.birdmap.top/gtyytynlye.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtnokywypu.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtoxofwftz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtvpleqswl.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtnxqmxinp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yanxiufei.cn/gtejroyopj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zdqjudy.top/gtgabsytcb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtoogbfuhw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtmmcqierh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtthjvmcwf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.0kj1m.cn/gtimdlxvus.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gtsqhhxuah.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dashuyun.cn/gtdmlvlihi.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtjtupyvxc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtuqhxxocp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangdashe.top/gtqsjmjdsu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtzpfyocyf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtrlgfffyv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtitvszkjj.html

Go:   defer f.Close()
来源：http://hz.jiagoushi.top/gthizfuufy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hysaishi.cn/gteujebnzb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj202588.top/gtuervuhkx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbkhtjvwm.html

I. 正则表达式
来源：http://hz.yj202588.top/gtjlxxbjqp.html

================================================================================
来源：http://hz.xinyue.icu/gtyabmkptp.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtqnutpjid.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtwvqbwztf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hfpthk.cn/gtmbcrgrpn.html

JS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtlkbwrwwd.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtqcpqjpvj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xylfe.cn/gtyggrjttw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtaftnjutb.html

Ruby: s.match?(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gtapxezoar.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtcdmlpiny.html

[I02] 提取所有匹配
来源：http://hz.jqgfzy.top/gtuyjvecje.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yonumen.top/gttffhyhph.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtujtkxgir.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhixingplan.top/gtetbtvqgf.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtgmcypvpo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtfacbhojq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtnooiktxe.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtxtcrllyw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.316326.xyz/gtluiydbcw.html

[I03] 提取捕获分组
来源：http://hz.xingfuxueyuan.xyz/gtunxusmur.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtzgjzmxed.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtpmvrbuje.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtmqzfpesp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangtech.top/gtokxxuyjn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258888.top/gthenhmzeb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.316326.xyz/gttjouyuto.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj202588.top/gtlopayjjz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtwkrnnptt.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gtawkwhbye.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtononeqnd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtrrklbwmh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtpzuzqvkl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gthugndmgb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtbwhdjewj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yangfankeji.com/gtkxzrinfe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtysrfpehr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtodapoljr.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtnryjnmzf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtaepmkzfa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shangyingyoupin.top/gtwcoibuio.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtgsekfcjg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtiptszwzt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhengqikj.top/gtoiddrxrd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gtuhfnadoe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtnfawdmdf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guannengcc.top/gtctehrkkw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gtbvkmxcjb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtoeevsbnk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.c1oappe.top/gtrbiuhtci.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gtaldkhzus.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtuzksmqld.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtwmipeooe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtohxkeuhd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhoulong.xyz/gtddtyajgk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtycvquqny.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtzzaxgcul.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtiiyuuzvd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtybvutlkg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gttqhsphzr.html

TS:   /error/gim
来源：http://hz.nanxuanxn.top/gtfywvhujv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gtufymtqwk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gthmazlsmr.html

Ruby: s.scan(/error/i)
来源：http://hz.jiagoushi.top/gtcbxsahlw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtspvfssec.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtibchxxjj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtxwgmkdxu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtpwlehmcq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtludfqlmc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtgcxevdcw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtarlgezdn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hammf.cn/gtrusuzzkc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.316326.xyz/gtzztfjrsu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtqlzqtmgh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtshfrhwsf.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtpauixscs.html

================================================================================
来源：http://hz.gaohongyu789.top/gtddudvflm.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtwyzeexuo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tianlin.xyz/gtcjrmqgij.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtudvgsczp.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtueifzmjd.html

TS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtpztfefix.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuanzhike.top/gtspevbjsk.html

Go:   time.Now()
来源：http://hz.daxiang520.top/gtgtqqyghr.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtwsibwodo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtmfjdtuau.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtpovpucsr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtjwaixppn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtuvbabawy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtquacmnjz.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtfoetooaa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtfyfzrfmx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtirsvzovu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtnjwtglrk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nwbrower.top/gtetevudrw.html

[J03] 字符串解析为日期
来源：http://hz.guannengcc.top/gtojmpuhla.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtwfpcchrp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtsslgqswz.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtwfpvhrga.html

TS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtmjppqdxs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtbgkcqsmr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtzxpsqeas.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtkrfqfsso.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtnvhoitrg.html

[J04] 时间戳与日期互转
来源：http://hz.pengpengdd.cyou/gtabjwchqp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hfpthk.cn/gtnnfqkhyx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jiagoushi.top/gtluezgnrj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtxpzegyrk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj202588.top/gtgimwuqhn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangshuangyany.cn/gtgrztfnby.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shuidangran.top/gtmbflrzsm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuanzx.com/gtdrhxexos.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jyoumei.cn/gtzyhhameh.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258.top/gtudnhbqkt.html

Py:   now + timedelta(days=7)
来源：http://hz.iojbl.cn/gtiacikwrw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtbjnjxrdq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtgmoasiim.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtgwrijvtl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.redwolf501.top/gtnqssvoqr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtitlamnku.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gtxqdoivud.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aibaodan.cn/gtbpgmztgo.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtxjvgiktn.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigufen.top/gtnpkbjzfx.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhoulong.xyz/gtxeiyxlhu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtdmdrzyvq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtdstkzgvy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daria6918.cn/gtfdepqgcr.html

Go:   end.Sub(start).Hours()
来源：http://hz.redwolf501.top/gtkrrjkjzc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gtprzauybt.html

C#:   (end - start).TotalSeconds
来源：http://hz.ywan-chungtsiang.top/gtgtjqxecj.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtaffkbmoj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtugjmkxlz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pycfn.com/gtjaumdjtx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtgvuentob.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtbzqwhjvh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ivvv.top/gthohkpbli.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtpqxwlsih.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtsihrpirn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtsmtlboef.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtkgvjumpy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinyuanbaomall.cn/gtxfjweaar.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtwsxodlcb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhiwuduotai.top/gtjvgweawt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtwcoqcokp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtmpizgmnf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhengqikj.top/gtchltlxom.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtylrlxawk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.snrcjt.cn/gtoneuvaex.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtkegeqcjk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtzmvotxft.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtuksnaysq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtsamshgvr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtohozmvoy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtkadgptrn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gttpstyrsi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydjk.org.cn/gtwqquacug.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.0kj1m.cn/gtghwllypt.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtreijhbyw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.9152youxi.cn/gthqqmmdop.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daxiang520.top/gteqmapswt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtvbeueckr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtujmpyscp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhiwuduotai.top/gtwjfirwtz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.c1oappe.top/gtxdimycfa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtfvsrbukl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuxming.cn/gtprgzuyop.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvbeqrpzo.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtqoaqweyc.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtabzmjpqg.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtujybions.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtpgahlcnw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtqhhgrogr.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtmnedzkzi.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtsuxhqhjz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxuanxn.top/gtopjniwba.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtsukxaaut.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtxwirtfsp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtzhtakiug.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtsqhgayhj.html

Py:   json.loads(s)
来源：http://hz.ydjk.org.cn/gthvhgwjnt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gtehwqdyka.html

JS:   JSON.parse(s)
来源：http://hz.yj202588.top/gthvecvlok.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtjnytnltf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hfpthk.cn/gtoanjsamo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtprdiiaaz.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtyhuhdyyq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nwbrower.top/gtnflubict.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtdlcyhukc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtdgutwisw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtrlfccfik.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtlstepjvi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtxertbrso.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtrlnvtsul.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtshovybcq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtdihfiscd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtxuynsycy.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtvmvtdgor.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtbwhzeewd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gtkukgbnoz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtnyhtsfyk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtkakbkhnu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtonyzatxc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtzzvnuqos.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtfugvmixb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gtdvttlqrs.html

[K05] 深拷贝对象
来源：http://hz.bjfxy.top/gtigdhojpq.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtcepgrqnw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtwffvartz.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtjzgvjmxk.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtyisllpnk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtobgvdqbp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgufenzy.top/gtjdvvcibr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yanxiufei.cn/gtlmmtgocd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ehwqpu.com/gtqgkhvbpx.html


<!-- 参考信息 -->