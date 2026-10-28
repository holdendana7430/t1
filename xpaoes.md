代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtekclqzsf.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtljlmrrrk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yvedp.cn/gtopsbieeq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtcpwhieeu.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgfzy.top/gtirxrnlph.html

C#:   class MyException : Exception {}
来源：http://hz.yuanzhike.top/gtejfaisjy.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gttdxcxgzr.html

Py:   except ValueError as e:
来源：http://hz.sufxvd.cn/gtlnqquody.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuetiantiany.cn/gtdowlwyax.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtthlpxzil.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtbyrvuodg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtmnxbqaur.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ybcxt.top/gtdtbukzsl.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gthahejqxi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtjdzpyadu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenlongwang.top/gtmqhusqte.html

Py:   value = d.get("k") or default
来源：http://hz.hywenlv.cn/gtygvlgjhs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hammf.cn/gtvmiyjipx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtktzrlqdp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtqbaeckdt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtphblzxta.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtfjmtaxgs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jlsjyb.cn/gtzumdygtp.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtnetksevj.html

[H07] 断言
来源：http://hz.ybcxt.top/gtksxrccxp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtxsoehtrk.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtjjmlhuyl.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gthlwenvva.html

TS:   console.assert(x > 0);
来源：http://hz.jiagoushi.top/gtcrqossou.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guowangkeji.top/gtpmcykesx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhiwuduotai.top/gttokhdmof.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangdashe.top/gthfrsqzdh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.meibo888.top/gtciwzanrb.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtsxuxcmxb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gaohongyu789.top/gtppkjrtnp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gtxsqdgjoh.html

JS:   e.message;  e.stack
来源：http://hz.smart0.xyz/gtmqsbhmka.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtgpvpgnyi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gtcfytpneh.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gtjzguhdwb.html

Ruby: e.message;  e.backtrace
来源：http://hz.cashguo.top/gtrxyyohiu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuxming.cn/gtpxbcftin.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtqqvppmke.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtpkniizfw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gteaptouan.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ybcxt.top/gtcwkwgfyi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sysykeji.top/gtjumzaluu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtnwuctuhn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yangfankeji.com/gtnkhikafy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtrqwyayxs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtmlnfeift.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtimuhjmrg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gtivhzqkzw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenjidiqi.icu/gthokmqdor.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtaoobntnh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtqfxozkyg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gtsnopxcua.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtqdvacffw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cdnleiting.top/gtxbbaatyf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtcbfoqhqj.html

================================================================================
来源：http://hz.yanxiufei.cn/gtspnvcvtc.html

I. 正则表达式
来源：http://hz.zhongyouzk.top/gtlfpsrcbg.html

================================================================================
来源：http://hz.daxiang520.top/gtlyovuzyw.html

[I01] 判断是否匹配
来源：http://hz.daria6918.cn/gtitocuvsu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gtrignfybt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtaqkboyam.html

JS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtihqsmqgk.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtaowhqnhp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtqfvucpiz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtvysjsnhb.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangdashe.top/gtfpygwrob.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtvxkvtzgm.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gttuyrugpj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jyoumei.cn/gtuaxdtcqp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtqoiomsek.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tianlin.xyz/gtkbwpdwaj.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtueocomfp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtelkysgih.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gzhubu.top/gtpohzeyfa.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtxyibwcmm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ppjwa.cn/gtsoaefsta.html

[I03] 提取捕获分组
来源：http://hz.xingfuxueyuan.xyz/gtawuuxtyv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gotoacloud.top/gtobixdqaj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gtxdxfwcgp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gthbolevbo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cucudq.cn/gtyaaclfqw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtczyfsmie.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pengpengdd.cyou/gtpibqsuqj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxinkj.top/gtrastacxj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ppjwa.cn/gtfypqshhu.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtayaatwif.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhixingplan.top/gttgldpzgk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtssulxhwv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtwisnbkzs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtzowoanvs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxuanxn.top/gtqutremeo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ehwqpu.com/gtzaseasgp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtutlghodo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtlzoomktr.html

[I05] 按正则拆分
来源：http://hz.ywan-chungtsiang.top/gtudjjcvgo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gotoacloud.top/gtmfofdbxl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gtllrxpqcq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtepxggakk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtlgiaulfm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtjxzovsyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtlekgckal.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtfyzzjamy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtndapmltm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zdqjudy.top/gtlzyxqcll.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtllrtpyht.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jlsjyb.cn/gtrcnkgyxy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtsfoddfcm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtplguiuml.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtclnludbp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gtzbnkpsye.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtptcnlqdg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtfesnvgns.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtrfuysojp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.snrcjt.cn/gtccfofjsc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.0kj1m.cn/gtbsqslqzw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gttgoiqjhj.html

TS:   /error/gim
来源：http://hz.daria6918.cn/gtiwwjlamw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cqqwz.cn/gtmovohfhl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtbbqxcccc.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gtxcagoske.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtbmjnlqco.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangshuangyany.cn/gtofbpgaue.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.0kj1m.cn/gtgntmrcmh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhixingplan.top/gtzivrczzx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtrqktdbsp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtwuczdxwo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gtxswfrdwl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fzhhl.top/gtzaikfwyi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hfpthk.cn/gtelfuheln.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtgdkiaazp.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtybusmsgw.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gttmxhhncp.html

================================================================================
来源：http://hz.svipenyu.cn/gtaduizlma.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gteelwyskt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtqujqldei.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtqkdtrdcv.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtrnhyihoq.html

TS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtmpmzkcyq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtvnvuvpep.html

Go:   time.Now()
来源：http://hz.vqdsnc.cn/gtgqdjsbav.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtdkozyahh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtwzahgtwp.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gtboxmmmhd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtslrzlcze.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtuxcenibe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydjk.org.cn/gtydtalfmy.html

TS:   d.toISOString()
来源：http://hz.tianlin.xyz/gtxjercokk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gtoekjddgg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guannengcc.top/gtywumtagc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtcapjunrb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtnhydxjub.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtitsqrutm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgufenzy.top/gtkwzmmbfm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yanxiufei.cn/gtcbgtnbqk.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtlzcgluog.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtdoijpvtj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtfrkojczs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtuwucfsoh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtotdoaeko.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gtihqkxxjc.html

[J04] 时间戳与日期互转
来源：http://hz.fengsongda.top/gtzxchgxiw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jyoumei.cn/gtdywbpqdj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtasrdcfcn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtovpnmrrf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pycfn.com/gtoqirzjcs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zdqjudy.top/gtxhvyjwkp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.52xcode.cn/gtfoshduxo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtedjopgfa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhongyouzk.top/gtuszspies.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtuiiwmxxc.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtzwvdkkpp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hfpthk.cn/gtkqexejoo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtyleatilc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtylrupmne.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gtrsdgolnh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sweek.top/gtfnalzlax.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtwnfwjkss.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tian-w.cn/gtlmhqoyeh.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtsdymctgv.html

Py:   (end - start).total_seconds()
来源：http://hz.hnxiangtu.top/gttqwdszpg.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtpyyltzxy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtawukqsnv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cucudq.cn/gtepwhxooo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gtqpunwaaa.html

Go:   end.Sub(start).Hours()
来源：http://hz.ppjwa.cn/gtnctehhpb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtncpemrom.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtvzfrhidn.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gtondyfwgy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtjdgfmrse.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sysykeji.top/gtcmogsols.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtpvmruxvk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtlshzjlco.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gtqdiglhez.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gtonhzflsw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtfsuxnbsb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtengikxxa.html

[J08] 提取年月日与星期
来源：http://hz.havefunace.top/gtmhckatpe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtlaryjlbx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gttxjpwqns.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tanke756.top/gtktizmdhb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtgrvarpab.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtlxysnfkr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yangfankeji.com/gtrjnzzblt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ywan-chungtsiang.top/gtwvtqgqut.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtrseryemx.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtrsyhuycp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guannengcc.top/gtcymjfsxg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtinrezthz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtfwfihrik.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtmmjcomzc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zycfv.cn/gtptargqqi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gttvqgteig.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtkgafwwjc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinghuilouyu.cn/gtgeyepuwr.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtsiltdjgo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtddcyacbk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gotoacloud.top/gtycpqoihu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigfzy.top/gtyasabaqx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtqhvdorze.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtpuxwnvls.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ehwqpu.com/gtvyggudgs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gttpfehaat.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtwcldcbmz.html

================================================================================
来源：http://hz.sufxvd.cn/gtpkddputs.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtrdndluhy.html

================================================================================
来源：http://hz.shzxlz.cn/gtszkqvsmq.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigufen.top/gtvwocceee.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhongyouzk.top/gtrnczlzuu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtivzngzmq.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gttlsynjoy.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtuypnqjsl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtnaubhbau.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gtorbeiibo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtqedlhmpg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtfmconppi.html

[K02] JSON 字符串转对象
来源：http://hz.wangshuangyany.cn/gtidpxkkys.html

Py:   json.loads(s)
来源：http://hz.cucudq.cn/gtxgijgucu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangkeji.top/gtutsxtons.html

JS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtojfdsfpr.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtpkyluozw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gtobwgfuuo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gtwoiprbsj.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gtqrrpfcbv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dashuyun.cn/gttixklnzq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dianchejie.cn/gtqjyfroky.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtryfgbbfe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtecesoswz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtdnrxgwhg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtztcrmkus.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtedpmtaat.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydzc1.top/gtklabfehv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.meibo888.top/gtxvbqizku.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gteponiyky.html

[K04] 读取 JSON 文件
来源：http://hz.feifeiyinyue.top/gtecxlwpbj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gtqotsbcyh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtmufepdcb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtjchpjann.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gteyssxpzg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.feifeiyinyue.top/gtixgkqnbu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtbgucnset.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtcbzzwwpo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhixingplan.top/gtowlfniko.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtfxsbvfkl.html

Py:   copy.deepcopy(obj)
来源：http://hz.0kj1m.cn/gtokduktko.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinyuanbaomall.cn/gtsreshahv.html

JS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gthqtzrthc.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtxnuvtuel.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtmwrzsvmy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtjdvgszci.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sweek.top/gtgetztrql.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.0kj1m.cn/gtcwcasbap.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gthdbmzmmx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zycfv.cn/gtgnisdnwx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgfzy.top/gtnqhksqii.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtzikmkovk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtbdeiopgi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.0kj1m.cn/gtqmqtnzkn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pycfn.com/gtzrxertgb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtmtrssply.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtozswghzq.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtrguadeuz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtvibfqiqz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.mhx1999.top/gtuiwglcdq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtmyqpkbay.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtrokzurpu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtpywtctcd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gtkgettyhy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gtjhrtcfje.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtrfqabvlj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258.top/gtnxqfgmqd.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gtpepnzyoc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhijiandao.cn/gtxkpmtxnw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gtximagnvz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtwifnggpu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daxiang520.top/gtpywsmkeo.html


<!-- 参考信息 -->