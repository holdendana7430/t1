代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtbygpwped.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gttlfpvygm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtncmnernm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtreocrfrf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtdpnqrgye.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gtwmuqmuqa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guowangkeji.top/gtzsioorzj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shangyingyoupin.top/gttwyjpxqp.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gtyjfwsoqu.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuxming.cn/gtnbsglrve.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtbafbtetl.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtddbqjakx.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtmpgvfcik.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.mhx1999.top/gttcbxuqjr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtiihqaism.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgfzy.top/gtfvmbtosr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtugssusos.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtvjesyjjp.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gteuidjjiw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtmlccsixn.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtzcdbfonu.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtejudfikw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtbytnlkrs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangtech.top/gtbstrrpch.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhoulong.xyz/gtmwomakai.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtvbkxcscp.html

[H05] 捕获特定类型
来源：http://hz.nanxuanxn.top/gtgnwkmaua.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtjmzlhjzk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtxvhahzos.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtjlkdyxku.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtxvqulssx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtkmjucnzo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtczhtzhtn.html

Ruby: rescue ArgumentError => e
来源：http://hz.gaohongyu789.top/gtrepxfwug.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtampjvfjy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtambfxdyz.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtndivyhgy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtryimsrbw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtisrzyqed.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtxpltfcyu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jianghu66.top/gtkwebnksy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhoulong.xyz/gtwdjkxblt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gtdppptfxj.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtymbdrans.html

[H07] 断言
来源：http://hz.ydjk.org.cn/gtwgluuyht.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gtakongfzw.html

PHP:  assert($x > 0);
来源：http://hz.jlsjyb.cn/gtgffiwqjn.html

JS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtzlnrxrui.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtijblnbng.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgufenzy.top/gthjfcmkax.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sxryk.cn/gtqjsjhves.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtfudmydxo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhixingplan.top/gtltudlblk.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gtlrcoezpv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtcvlncviw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtvuyjbpkg.html

JS:   e.message;  e.stack
来源：http://hz.9152youxi.cn/gtoosdcthy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gtcpcizkac.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtihsrvbft.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtsnmeditr.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gtorkilgea.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtqdzrfjec.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtkppavqlw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuetiantiany.cn/gtmfgvorxg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gtshjbmfka.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shangyingyoupin.top/gtrvuprths.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtpnxcipft.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gthxuhfgvf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtldcvkeom.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtnpwxsave.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xziqi.cn/gtcikiisxv.html

[H10] 资源自动释放
来源：http://hz.yuanzhike.top/gtsthhsrus.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtpwreshlr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yvedp.cn/gttxlpjqeq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtnqqabuvi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtxjbvdlij.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtezslceos.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gtzlbpnonf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtgmmlyhut.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.bjfxy.top/gtpfyyzjfo.html

================================================================================
来源：http://hz.tian-w.cn/gtjvyexgmg.html

I. 正则表达式
来源：http://hz.hywenlv.cn/gtkamqwvev.html

================================================================================
来源：http://hz.zhoulong.xyz/gtljptmyul.html

[I01] 判断是否匹配
来源：http://hz.chenzaomai.com/gtxvefhwwh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258.top/gtkeegwkmr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenzaomai.com/gttdibjdli.html

JS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtgtagfoht.html

TS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtbwvglzue.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtrsgynbmy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fzhhl.top/gtudszkbtu.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhoulong.xyz/gtxfvdpyoq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangkeji.top/gtybgvvumr.html

[I02] 提取所有匹配
来源：http://hz.shuidangran.top/gtvybohofd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtvgyhhjxp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtoixrtuox.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.9152youxi.cn/gtjuvkrugm.html

TS:   s.match(/\d+/g)
来源：http://hz.yonumen.top/gtzxprrsnv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtdemopubx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtdvobsqlh.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtjarjuerk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yongpay.top/gtjkrfyvaq.html

[I03] 提取捕获分组
来源：http://hz.ehwqpu.com/gtxfzofgwd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cdnleiting.top/gtzlcplekc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sxryk.cn/gtfpznekmx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnxiangtu.top/gttxlnpbsu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtkqqvdqex.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtwtfhpier.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtoykwolgs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gtevicuxwl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.svipenyu.cn/gtkajcqndm.html

[I04] 正则替换
来源：http://hz.fengsongda.top/gtxfnhytmb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuanzx.com/gttvokghmu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtktiinonu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtzgrsiunt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtvxsyrofd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.mhx1999.top/gtpxvxxnia.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gtldxtbfod.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtvcfyktee.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtygzsbevv.html

[I05] 按正则拆分
来源：http://hz.wangshuangyany.cn/gtjqyoimtm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtakmmtzzz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guowangkeji.top/gttpdgpcyx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtyjxngesm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtdftzziqy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtljqmvujw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtkofpgbga.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtldmjxhhj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtdmvptnvn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gtvxszlplj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtwsuvupar.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtgcrfwzxp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtxruusjlm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtbvvziadk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtkyabftri.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gttnwcsvdp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtzscakrlx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtseplsigg.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gteitxhhdu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtwlsesmad.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hywenlv.cn/gtbmbpnuzu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtstruqknv.html

TS:   /error/gim
来源：http://hz.daria6918.cn/gtpufdaqpb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jyoumei.cn/gtxoehujks.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.9152youxi.cn/gtymaupybv.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtonhpwchw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtrnxlrxtt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gtgeycwbfk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtkojenhxh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cucudq.cn/gtryapfxyh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtxppkgpnh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtmzbpyvwc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtyactspps.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnxiangtu.top/gtxjbycsxq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtdpodffee.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtqelmykiu.html

================================================================================
来源：http://hz.iojbl.cn/gtflsxqtmr.html

J. 日期与时间
来源：http://hz.pengpengdd.cyou/gtmfujxyrf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtongnjlzh.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtmllocsit.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtqckyneqt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gtsmaqivjl.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtzkvybxxg.html

TS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtipuqnbxy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sufxvd.cn/gtemkywmzd.html

Go:   time.Now()
来源：http://hz.0kj1m.cn/gtuxdqasvd.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtuimjkoin.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtlfadywna.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtkikdqscl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtsraxtiuf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtunasmcyu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gtfxnfbgvc.html

TS:   d.toISOString()
来源：http://hz.gogol.net.cn/gtbpvyzzra.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hfpthk.cn/gtjjkkppju.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gthmmmfmyz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtmjnucscz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yonumen.top/gtkzklljtt.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gtprysbzbm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhengqikj.top/gtksxcbhvf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtojnhcjlm.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gttqeuswrv.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtivsacwlc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtukrfrjsg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sxryk.cn/gtatyqatsf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtannqlozi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtwfikfrmy.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gtrhsogsrs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gttctglfch.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxuanxn.top/gtppbffhpz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guannengcc.top/gtvewziwzx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtygfaxbuv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtuburvpdk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenzaomai.com/gtpdcbpzsb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtvksspozb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtvbagzpvj.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtozoqyrcx.html

Py:   now + timedelta(days=7)
来源：http://hz.xylfe.cn/gtfthrgros.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tianlin.xyz/gtzivixmio.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtxhjtewoq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtlybvkgpz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gtecrmseqy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.kuanghao11.cn/gtqlhuvhdx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gtekqyuayk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtkcuesqbs.html

[J06] 计算两时间之差
来源：http://hz.ehwqpu.com/gtxhkibnxg.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtnclbvvvo.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258888.top/gtzqphrthu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuxming.cn/gtirbftotf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtaarhkicc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtspmguexv.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtnebgkjkq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gtewyqcuqk.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gteulyiqex.html

[J07] 比较两个日期
来源：http://hz.hammf.cn/gtejoceyee.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gttlsbfaje.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtuitryice.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dashuyun.cn/gtkbdskjxz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtxfifyibm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gtkinzxuea.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xingfuxueyuan.xyz/gtpvjbhmpo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtjpnosvqi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gteckjcmyd.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtetwvthll.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtjxsakdrn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhixingplan.top/gtnegjfxsq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gthqkhxfuc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtglofwtwa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtyugwauwy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guannengcc.top/gtdtwbeygx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtzgglfgax.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtaunnpvmn.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gtlrwqzajv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtfvxutdhy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtpqgmifhl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gttesrtmdi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtoykqbucx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtombdbbgy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gtoigyvavv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gtqfmlqlab.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gtxjtgjgum.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtcfyakcgr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtdzjqvzli.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sysykeji.top/gtvgxbcyhg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtexhjqdnf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gtypyprxtq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtsfiztjko.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnxiangtu.top/gtjgqcynec.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtvvpnibpv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gtjnnppodq.html

================================================================================
来源：http://hz.cdnleiting.top/gtdcbmmnnb.html

K. JSON 与序列化
来源：http://hz.dianchejie.cn/gtviithgtq.html

================================================================================
来源：http://hz.cheryme.top/gtrfbuqcpe.html

[K01] 对象转 JSON 字符串
来源：http://hz.gzhubu.top/gtjfgwxeme.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sweek.top/gtqhrtljgi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtbtmsnjyz.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtucfyxydp.html

TS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtywldacjr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuetiantiany.cn/gtknjfooqe.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtqmfssnzo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxinkj.top/gtcosljbvl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtwtekopar.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtdlxlrivn.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtgfakkeuq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zycfv.cn/gtjwhcqzph.html

JS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtjesgaekp.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtobbymztd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gtdrfmszma.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtugvdwsyh.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtqwvxyzrx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ehwqpu.com/gtjjcmffkk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.svipenyu.cn/gthawtbwku.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtzafxkslm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtfgjoxmgy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtyvvntlzw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtzskpnzlg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtoaycqtah.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenlongwang.top/gtzqitfvhh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtxnaxkomn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xziqi.cn/gtlexadbtl.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtojdzuaim.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtvlrlhwzf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pycfn.com/gtizoicdsq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtgbfozbmk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtyksiotnl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtcnmtsjjn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtaenvawpj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtgcfbforg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxuanxn.top/gtzyikpizv.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtjgnefqmg.html

Py:   copy.deepcopy(obj)
来源：http://hz.mhx1999.top/gtqmueliks.html

PHP:  unserialize(serialize($obj));
来源：http://hz.0kj1m.cn/gtkcdykdzu.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtaqmqdpzj.html

TS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtvrenkegu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtqnfzfbze.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtqxxzrftp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtzfqubkkp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtpjesjehd.html

[K06] 解析 URL 查询串
来源：http://hz.ppjwa.cn/gtlvoohhxi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ehwqpu.com/gtpbnmgnkj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gtihttlvrs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gthkexqyky.html


<!-- 参考信息 -->