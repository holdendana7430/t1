代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ywan-chungtsiang.top/gtzmatrngs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtcaxbadra.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtpigzvovg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtixabfmbd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtgcjybjhl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gtoutwcqgs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtxjgxtoaw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.vqdsnc.cn/gtpnpvsuqa.html

[H03] 主动抛出异常
来源：http://hz.guowangkeji.top/gtfnnvwduo.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtvttmlrrj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtotkpduvf.html

JS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtggfznkok.html

TS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtcaiwpetk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtcmaihhfd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zdqjudy.top/gtobeoeeqa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.haohaochexian.top/gtwidwryar.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtygaqdosu.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtwpsatdiv.html

Py:   class MyError(Exception): pass
来源：http://hz.meibo888.top/gtzyjrsnlz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gtfqlqiwqf.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtnpqllpgg.html

TS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtjcjtrvvu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtawdciroz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtholetahn.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtyzjwmydg.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtwlvqluwm.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtdgsctfwz.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtzvhkeiqk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xziqi.cn/gthprdnflq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtwfejlzoj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtffxygube.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtuisannwy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhaomingkeji.xyz/gtxkzanxhz.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtzfufhzhd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.redwolf501.top/gtsxjnakbk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gthfywkekf.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtixcyhsus.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtvvshfrra.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtfagdzxph.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtnmuxfxma.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtnlqkttyn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtrxxqmgek.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtfseqmxax.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtyyrvcbxz.html

[H07] 断言
来源：http://hz.zdqjudy.top/gtvrzzjqeo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.9152youxi.cn/gtorasoqbl.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtpglhpohb.html

JS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtbwqpttuh.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtmrsmoviw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtoyepbdif.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtjjmtgyde.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zdqjudy.top/gtqczlxkbl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtwiexakps.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtmqsmlpik.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangdashe.top/gtnehsynuu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtbfvlwkwo.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtvwxzebph.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtyhioywkf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.havefunace.top/gtocbhlylc.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtkekdwagy.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtkddbijix.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtylgqtmqn.html

[H09] 带错误码的异常
来源：http://hz.tianlin.xyz/gtoqhxlozp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtezdmzsiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.haohaochexian.top/gtiutdgzxo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gtyhhspifv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtmzbljrzd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtwonjnfcl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xingfuxueyuan.xyz/gtjcqjondx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.birdmap.top/gtcqjhvhwy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuanzhike.top/gttenpfkgi.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtbfpvkocq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtygokdisn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtjqolvopt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtlihrjevd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtysqrgmrj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtpuqnjfdz.html

Go:   defer f.Close()
来源：http://hz.yvedp.cn/gtmiwfgjxn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtnesezygs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gtszltkdax.html

================================================================================
来源：http://hz.zhongyouzk.top/gtgbnkhvre.html

I. 正则表达式
来源：http://hz.havefunace.top/gtkeulakev.html

================================================================================
来源：http://hz.tian-w.cn/gtcqiczvii.html

[I01] 判断是否匹配
来源：http://hz.jlsjyb.cn/gtqyrhwbsz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhongyouzk.top/gtiniyoqyt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtkrjjxgcb.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtvfgsqmmi.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtxibfghhp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.9152youxi.cn/gtcrtpywaq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtfaficwwn.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtyvszmufk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dashuyun.cn/gtcxwrtgjt.html

[I02] 提取所有匹配
来源：http://hz.shangyingyoupin.top/gtabsgufeu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.bjfxy.top/gthcvmthre.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ehwqpu.com/gtqyswvkiq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gtraibwcel.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtsnqgsgcy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dianchejie.cn/gtzfvoosvc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtndjovurq.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtxhlpymco.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtgpnvlggu.html

[I03] 提取捕获分组
来源：http://hz.cdnleiting.top/gtdddnovrf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhijiandao.cn/gtmppiobhl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shuidangran.top/gtmuexphyc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jianghu66.top/gtsxxrhbeq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xingfuxueyuan.xyz/gtadwnrxtk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.iojbl.cn/gtuufqgdag.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtzqbivnig.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gttpnjiyxl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtteuskazz.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtvftvqlzz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gtomsykddq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtvyhxhtiv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtfhgireje.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtiklnueoc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.0kj1m.cn/gterlifvyk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtxpycmejb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.52xcode.cn/gtimyraqcg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtihdqpzty.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtdhvgrgkr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtrtjaenoi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shzxlz.cn/gtzgoqhpfu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtifzqkyax.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtvxauhvkw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jyoumei.cn/gtsergfhxm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daria6918.cn/gtcdoojlvs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtxojjglvb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jyoumei.cn/gtoauxelcl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxinkj.top/gtmrvhhanb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtyqwjvekc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gtmdjnhqfr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtkxhjhvnu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtrnfzqitp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigfzy.top/gtnexekpav.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtsltzwehz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ppjwa.cn/gtuxhmjuxv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtjjsseepq.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gtfscpgdxh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gteytxiwdn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.svipenyu.cn/gtiwtcgwcb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenzaomai.com/gteegvycvy.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtxamqsfdd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtqgkgbmmk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtwpkehjwh.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtyflnroud.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtbeyihxiv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtyqqdlaem.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtbxwproms.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.andypj.xyz/gtazixdwkk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtribkqxzw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtbjqpcktz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fzhhl.top/gtoxwzdflz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fengsongda.top/gtkghaqhvo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhijiandao.cn/gtelketdsa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtrceslxqg.html

================================================================================
来源：http://hz.gzhubu.top/gtgsuuubhs.html

J. 日期与时间
来源：http://hz.xuanzx.com/gtcwfhubpo.html

================================================================================
来源：http://hz.fzhhl.top/gtzddslmxu.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtebalsbim.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ehwqpu.com/gttqvjqyge.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtmzlrvkgs.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtcoiydvdo.html

TS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtpeprxwyf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangshuangyany.cn/gtxgixrgkz.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtetpjpvug.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtknbpgfrm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuxming.cn/gtqcnuhczh.html

[J02] 格式化输出
来源：http://hz.zhengqikj.top/gtwpgswnoh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gthexdognk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gthsqbejwq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtyskwgkhe.html

TS:   d.toISOString()
来源：http://hz.svipenyu.cn/gtavugdkvo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtmflklziw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jlsjyb.cn/gtqrquwxpp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtwoywffzs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.vqdsnc.cn/gttwgldbbj.html

[J03] 字符串解析为日期
来源：http://hz.cqqwz.cn/gtffimiqgh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtfqwidcwb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtirkzfdzg.html

JS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtjyhhotpq.html

TS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtigumoelx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtaundbdmx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gticcsfzqw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtqjkzfzpa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gotoacloud.top/gtznyudmby.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtvjdvnmpd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gthmnvmnni.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtfujtrhem.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtqfohltis.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtfespcgvr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gtmddtwusl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtxlaegqrk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gaohongyu789.top/gtysdfcwmp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtpylcjrln.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydjk.org.cn/gteatsopjw.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gtemnxbrgx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gotoacloud.top/gtwoniatap.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gtgfkmuydr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtzxmqxlsa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangdashe.top/gtvufqxdqe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtetgsfriv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtwgajsyux.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gtxizqtshg.html

[J06] 计算两时间之差
来源：http://hz.ydjk.org.cn/gtyixtuivo.html

Py:   (end - start).total_seconds()
来源：http://hz.52xcode.cn/gtaybmyovy.html

PHP:  $end->diff($start)->days;
来源：http://hz.shangyingyoupin.top/gtnbvxbocr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hysaishi.cn/gtpqhwtryl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtsatfrayt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shuidangran.top/gtvmfxfroj.html

Go:   end.Sub(start).Hours()
来源：http://hz.xingfuxueyuan.xyz/gtgtlooder.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtipqpuueg.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gtfwkwfhvz.html

[J07] 比较两个日期
来源：http://hz.yangfankeji.com/gtunfsbzwz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gthoppqpmn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ppjwa.cn/gtmjwddxwh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtblfogzrf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtjktpddhk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gtslfbityt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtmspwoqfx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtsgscsrcg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtnjmvrjpu.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtqzxzkzwu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtmlmnuimb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.redwolf501.top/gtbhcwsjnw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtsatklzpb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtdkemcvfr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtfnvyndrv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gzhubu.top/gtxrktnkit.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hysaishi.cn/gtoexsaobq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtvyfrbmbr.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtidbwpdpr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnxiangtu.top/gtbgpxohrv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtqoxjgvcm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtmpsqhkzi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtdgnwuxlt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gthduvddzn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtcafrezur.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtxaiypjss.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gteaqvmaqa.html

[J10] 取今天 / 本月第一天
来源：http://hz.shzxlz.cn/gttrgpaeng.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtvlomvzgr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigufen.top/gtvwjpcnop.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258.top/gtyvzewgna.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigfzy.top/gtsrejjbbz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.9152youxi.cn/gtbmpvinkx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.haohaochexian.top/gtojsatyqt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtzcdnseom.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtmwgjsahj.html

================================================================================
来源：http://hz.mhx1999.top/gtvwezxfba.html

K. JSON 与序列化
来源：http://hz.tian-w.cn/gtfwopxlbo.html

================================================================================
来源：http://hz.smart0.xyz/gtcydylrib.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtnguxjuml.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtruagvzjm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtggwitveo.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtpdufwnup.html

TS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtvtbxxsao.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gtrllxmpoj.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtyounmist.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtwijixejp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtbguzrzsw.html

[K02] JSON 字符串转对象
来源：http://hz.hammf.cn/gtruzhknsk.html

Py:   json.loads(s)
来源：http://hz.tanke756.top/gtdijqruqv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gzhubu.top/gtwnslexde.html

JS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtzqdnopch.html

TS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtovlssirj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jianghu66.top/gtesxoyvbn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtterbkhln.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtrphcqjcz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuxming.cn/gtpdhsuwao.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtrwcqxdfh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtpqtsqavk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtuzkaswut.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gteonxodzy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gteykspifr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtmbkwumiu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtdraeftcd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtlcrangsz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtwrpgkfob.html

[K04] 读取 JSON 文件
来源：http://hz.zhengqikj.top/gtxenxszsd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtzubvwswi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtqwqnrilv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtuhsngfga.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtlrmwvkrq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhijiandao.cn/gtsrddbomm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtyaroskuq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtcsztktkk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtkwnpjiuf.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gtakwaayty.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gtiqzuflqw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtuqlmgjmz.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gthtrfahuh.html

TS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtijmkwqwf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dianchejie.cn/gtwbrxzepf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cashguo.top/gtujfkdpyb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cucudq.cn/gtjvrwhvhe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtucymzqng.html

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gtvljvyday.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.iojbl.cn/gtyavhnxwb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sysykeji.top/gtolefbzzh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtqnhncemc.html


<!-- 参考信息 -->