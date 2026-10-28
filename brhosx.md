代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xziqi.cn/gtrtyhvnrb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtuxmamgga.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtgxoftved.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtiqfcjjnk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtgsgvsjer.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtbdyyklld.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtwxdfhynz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtajeoziri.html

[H03] 主动抛出异常
来源：http://hz.ydjk.org.cn/gtvzadbjsy.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtzhgnarbe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtexmraqej.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtpfvryesr.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtoufgoyhe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtguldqgpn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.havefunace.top/gtnseqtkwk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gzhubu.top/gtzwpzpfkh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gthzyxvudy.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtbqyujvbb.html

Py:   class MyError(Exception): pass
来源：http://hz.redwolf501.top/gtyierzyol.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sysykeji.top/gtneflhtdf.html

JS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtjymgkfsb.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtmvehtmdd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtqzjhfmdl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigfzy.top/gtpqkaydbi.html

Ruby: class MyError < StandardError; end
来源：http://hz.quarkkingdee.top/gtfasbrmvl.html

C#:   class MyException : Exception {}
来源：http://hz.316326.xyz/gtfufimwrf.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtbafhkuzo.html

Py:   except ValueError as e:
来源：http://hz.sweek.top/gtwuempufd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.c1oappe.top/gtbgzbtcov.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtjnbtmfit.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtcjhtutyt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtgotcaxci.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtfakbwhjw.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtiifgaovm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fzhhl.top/gtvazewbzy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhixingplan.top/gtrummtsor.html

Py:   value = d.get("k") or default
来源：http://hz.gotoacloud.top/gtofricypj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gternlnbkw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtkwhwlgpo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtodradpeu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gtaokxzuxx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gthfgdggjh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cdnleiting.top/gtptmuliel.html

C#:   obj?.A?.B ?? default
来源：http://hz.zycfv.cn/gtfmpvrrel.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtjtjdcwua.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtftrkgldx.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtspydwbhc.html

JS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtngpaagzk.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gthecirloj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yvedp.cn/gthwaoezov.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgfzy.top/gthfraalsm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtshgysvfw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtqqccyfie.html

[H08] 获取错误信息与堆栈
来源：http://hz.shuidangran.top/gtljsoghxi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gthgilncdb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydjk.org.cn/gtgmnnnmay.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gthsetarku.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtyjyanlsk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtycpbtpev.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtxjjuppcd.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtnnugggnj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtzuboymbh.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtwsrwixjr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.iojbl.cn/gtgipoxorv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtmvopdbir.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtxuxmbwof.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgfzy.top/gtkqqkpbqy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tian-w.cn/gtbbdeybwm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cdnleiting.top/gtgbypojub.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtpecdjjpf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtgstekcgb.html

[H10] 资源自动释放
来源：http://hz.kuanghao11.cn/gtqawpngtv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yanxiufei.cn/gtspyeiayh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gthdsuumpt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtodxvtjza.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtrowubuac.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.snrcjt.cn/gtusnvtefy.html

Go:   defer f.Close()
来源：http://hz.zycfv.cn/gtmcofraql.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtjlbjktgj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cheryme.top/gtnwclphtl.html

================================================================================
来源：http://hz.redwolf501.top/gtnmdsoxnp.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtvauxqviz.html

================================================================================
来源：http://hz.yuxming.cn/gtltqhvrfu.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtznvausdh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtemzipxnb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtastcoyvb.html

JS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtjflvftso.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtbctlfpcu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hysaishi.cn/gthkpwqmmp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daxiang520.top/gtklxhtcda.html

Ruby: s.match?(/\d+/)
来源：http://hz.shuidangran.top/gtviagmwcj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtwlwsorru.html

[I02] 提取所有匹配
来源：http://hz.andypj.xyz/gtgjwfptfv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.0kj1m.cn/gtjvbxojdp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.0kj1m.cn/gtjdmcnpkm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aizwys.cn/gtiafqnugr.html

TS:   s.match(/\d+/g)
来源：http://hz.havefunace.top/gtdsdnzcrs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtuxsefpgt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gtaniixwzh.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuxming.cn/gtsfwicbra.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtcnujatyj.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtsjetvoxm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtwsqbmbpw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuanzhike.top/gthuxwchgz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtabdwbzsz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gttmnvhrqu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gthdgsljpp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhengqikj.top/gtfkpkggrg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jianghu66.top/gttdnvxjwv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.9152youxi.cn/gtbhoifejj.html

[I04] 正则替换
来源：http://hz.dianchejie.cn/gtcbhzjbhx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.redwolf501.top/gtbwqiekwz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtquqfzbtv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtchmhvltm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtmopticpv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gaohongyu789.top/gtrmethfrn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtqutxslgr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gtiohbyjit.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gteerwgzdv.html

[I05] 按正则拆分
来源：http://hz.yj202588.top/gtvsfvqjre.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtgqihnfhx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuxming.cn/gtmwncqdao.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtfrtgwsjk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtdpomtlhb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangtech.top/gtbywgcymu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ivvv.top/gtjtmlxdht.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtrllszbwr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtvkuzmrjk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sxryk.cn/gtxfgcwpak.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtosgirewk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtugobgxvh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtszukbhwh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtcpleqjuh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zdqjudy.top/gtlijvjmtc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtqrjqmxhc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xylfe.cn/gtnqebmtkk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtxlqlxftm.html

[I07] 忽略大小写与多行模式
来源：http://hz.smart0.xyz/gtsjindqpd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhijiandao.cn/gtsdwgtjui.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydzc1.top/gtrrwedmba.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yongpay.top/gtfvrrjnub.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtjzcpvrig.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinghuilouyu.cn/gtzrbibssd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.svipenyu.cn/gtuwysdjdo.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigfzy.top/gtbdildvoz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jianghu66.top/gtbcpxpviz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gthvrnhkqz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ivvv.top/gtkfhecwro.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuanzhike.top/gtmzenbrvs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtpmnjgewh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtizwshyqu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtpunorgdf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtpfsznsnf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tian-w.cn/gttukklqzp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtkngvsgik.html

================================================================================
来源：http://hz.ybcxt.top/gtowltrnhe.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtjcakknjh.html

================================================================================
来源：http://hz.birdmap.top/gtayukuftl.html

[J01] 获取当前时间
来源：http://hz.jqgufenzy.top/gtwndybmkj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nwbrower.top/gtwgjatfmm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gthxhkduai.html

JS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gtnrclmcpn.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtyavpnnrs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daxiang520.top/gtoqttjipi.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtaovymxek.html

Ruby: Time.now
来源：http://hz.gaohongyu789.top/gtlrxwjnju.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtftvxnrex.html

[J02] 格式化输出
来源：http://hz.yueranfly.top/gtglwkypag.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtixjaqbpo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtverjenps.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.mhx1999.top/gtbkzrhdky.html

TS:   d.toISOString()
来源：http://hz.wangdashe.top/gtdxmmhbur.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.vqdsnc.cn/gtzlyhbzmg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtuwhhnube.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gthzjuxriw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtrxvyueao.html

[J03] 字符串解析为日期
来源：http://hz.nanxinkj.top/gtbneayzle.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtzeegeokc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtdsvwitmo.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtkloidzqi.html

TS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtmrhbgraw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtgaslyzim.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ppjwa.cn/gtpamotwsx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cashguo.top/gtufqljfpz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ppjwa.cn/gtymdabgtt.html

[J04] 时间戳与日期互转
来源：http://hz.hammf.cn/gtoqraovvv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtkqfgnmzr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtvturanis.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtamqshmjk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtojczgdvs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtqsxyhhqf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtfxhkkyta.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtypgjesnp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hongshengwenyu.top/gtwfgqgtee.html

[J05] 时间加减（加 7 天）
来源：http://hz.sufxvd.cn/gtasfmzuov.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangkeji.top/gtlzginqnt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.meibo888.top/gtvogdrjcw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gthlzlibsh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtjgifsuko.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenzaomai.com/gttlyayigr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtpkkxvgqu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cashguo.top/gtmcnxryvm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtfhigpeag.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gtsvzvbrxr.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtrhwghagm.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgfzy.top/gtgvolzxhj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.c1oappe.top/gtuejlflrq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gteijheagk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtmxhfqelx.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtbekmrixr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtxxuzlkrr.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtwpzlbtps.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gtphhoxrzb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtdlhydovr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hongshengwenyu.top/gtwzywguaq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtzrsvdkqh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtrlyubyja.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ehwqpu.com/gtpovuentq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gtmnryguxy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtpkpsisom.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtynkpotcd.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtoskwsfhh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtteeohweo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtiidbqtuu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gttmbvducn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pengpengdd.cyou/gthegpakmd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtxnniuzir.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtrnoinvpc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtebqiowji.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gttqnivptv.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtqvvbgjbq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtkbtowami.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtdyjsfemz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtqfsdxnlg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtdcwklkpo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gtydimhdrh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtsqlvmizp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtabsgnxql.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sxryk.cn/gtjscspqkv.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtbhingafg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtfbpmalum.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtulhotfns.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yueranfly.top/gtzliqoftr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtcocanvmt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinyuanbaomall.cn/gtrchpsbuo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenlongwang.top/gtizfuvhsd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xinyue.icu/gtshnyotus.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtuqboyivq.html

================================================================================
来源：http://hz.gzhubu.top/gtlgdmlpsu.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtsgcdblne.html

================================================================================
来源：http://hz.tian-w.cn/gtlzieuwcx.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangdashe.top/gtlrsgasga.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtqizbuedk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtzgeiukkz.html

JS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gtcxncacjl.html

TS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtbqpcpmen.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtwfwcywqy.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtsizlkjay.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtzczyxfvp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtwpggwcan.html

[K02] JSON 字符串转对象
来源：http://hz.haohaochexian.top/gtgwnxccei.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtdwjjutpr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtaaghjpny.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtcwjcyprm.html

TS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtuvgmnpdy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtrxckpnsn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtssdywgsi.html

Ruby: JSON.parse(s)
来源：http://hz.snrcjt.cn/gtznugdjwj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtptvorrdf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gotoacloud.top/gtjbyjwgyz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtndrrrjfn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtswdqyfym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtbpwqlqhs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtummhtvmv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gtllmxbqde.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuxming.cn/gtreeullns.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtlrubbomq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtlhbmgwaa.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gtsvcinfuz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtqrehzvuj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtnrcuodcm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtqtlkutap.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtxjmpsmwh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtjqbilrhd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtvkhidllo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtpoiavpfi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtwhahwjqq.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtybdcogvr.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gturdxjtbs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhixingplan.top/gtozpkbdqa.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtwprouout.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtzmzzlemc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtxwraaqnr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gtyzsnpghm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gtgdsmqjgx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cucudq.cn/gtbzxypgqx.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gtwroexoiy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtwkdzdgft.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtlyokjrnk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtqzloripd.html


<!-- 参考信息 -->