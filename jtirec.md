代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtvbsxzxfd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtrcaeognj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigufen.top/gthqvziuzu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtaahnqrbb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtuwccjzvf.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gtwavadmya.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gttqpcjjtv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtorszjacu.html

JS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtdxrdcyxa.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtoejhjxgn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zycfv.cn/gteacbhcsf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtmiebjjun.html

Ruby: class MyError < StandardError; end
来源：http://hz.dianchejie.cn/gtdkfdiudc.html

C#:   class MyException : Exception {}
来源：http://hz.yuxming.cn/gtwbynybgm.html

[H05] 捕获特定类型
来源：http://hz.wangdashe.top/gtsgdbmyvj.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gtdpzjkems.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtlleomrzx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtkpllgrvc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtvddbzfes.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtmwhltefb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtkxmristv.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtrhnbobcq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtiacpafcz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.feifeiyinyue.top/gtnhcabmfd.html

Py:   value = d.get("k") or default
来源：http://hz.yuxming.cn/gtgwmdgxgj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sysykeji.top/gtmtieyukh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtgntzaiqe.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtgoklbnsp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtlmcqcgdl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtrodejvea.html

Ruby: d&.dig(:a, :b)
来源：http://hz.snrcjt.cn/gtmitwasju.html

C#:   obj?.A?.B ?? default
来源：http://hz.ivvv.top/gtnjkzkpyq.html

[H07] 断言
来源：http://hz.pycfn.com/gtqbkqgvaz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtmfxbbsor.html

PHP:  assert($x > 0);
来源：http://hz.hywenlv.cn/gtctjcxsxu.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtmvjnxjmk.html

TS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtfpeqgbfm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yangfankeji.com/gtelpsgaee.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gthajpfpwo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtabqgdasp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtclvbtyla.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gthyfxhvql.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gtaxtqavgs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jiagoushi.top/gtiesaqdky.html

JS:   e.message;  e.stack
来源：http://hz.xuanzx.com/gtskbzwsck.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zdqjudy.top/gtealgktda.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtureelbak.html

Go:   err.Error()
来源：http://hz.pycfn.com/gtxuhayxje.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gthodgoweu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtettsosaj.html

[H09] 带错误码的异常
来源：http://hz.daria6918.cn/gtlcpqwmve.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenlongwang.top/gtujrbyiaz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtxpwqxdhh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtzscxirvw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtpybufvrz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtkfrgxzlo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xziqi.cn/gtjkqtfgeh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jiagoushi.top/gtsrqwuayh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dashuyun.cn/gtqlejzvkw.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtevpqtlpo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ybcxt.top/gtydynvctt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtvablpjtf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtjuosiwpy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtpequlkvf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtuyhtjmyg.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gtoahatmnd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtxounnfdv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258.top/gtlhtdfcgm.html

================================================================================
来源：http://hz.tanke756.top/gtmevbtuto.html

I. 正则表达式
来源：http://hz.sysykeji.top/gtoqladokt.html

================================================================================
来源：http://hz.quarkkingdee.top/gtijmukipi.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtgcdxqhnb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtebavwugr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtyfzvxztl.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtylanyoks.html

TS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtmfasbvji.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtmtjjbkfd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtethgndaa.html

Ruby: s.match?(/\d+/)
来源：http://hz.0kj1m.cn/gttuaszffm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dashuyun.cn/gtkyevsfxh.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtkwnscuqx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtmzuqcziv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtujsxljzz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtkshufwod.html

TS:   s.match(/\d+/g)
来源：http://hz.tianlin.xyz/gtmujvxcxn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dianchejie.cn/gtuluqtjzv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtrmveyuib.html

Ruby: s.scan(/\d+/)
来源：http://hz.jlsjyb.cn/gtamjubufi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtopchwqlm.html

[I03] 提取捕获分组
来源：http://hz.hammf.cn/gtlkecntuq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtzkxylthf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtcednmhmz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtgyhdevtu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.feifeiyinyue.top/gtpghlditv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtmiuwjldq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtjkmyjvtd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtvgcfkffk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gtpnwgcqoo.html

[I04] 正则替换
来源：http://hz.dianchejie.cn/gtuwkzeofg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtzxrnblfb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtqsafptoo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtqezstcsc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtupiiocse.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnxiangtu.top/gtjdkhmvkz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guannengcc.top/gtzbtesfso.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hfpthk.cn/gtksosvbjr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gthhoctypl.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtempcmjyv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gtdsaoraze.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtytreqnop.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtmreyhahr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtejfbtthm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangshuangyany.cn/gtvqcuddty.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigfzy.top/gtximgfotl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtvbyxrjms.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.mhx1999.top/gttpcohuyo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnxiangtu.top/gtpgtfgnaf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtbjnrbajn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtrxajntlu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtuaxwcozm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtozftceid.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtooojdgwa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtdwagqasc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.meibo888.top/gtuxjackem.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtjzvixrya.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtiyyyjafl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtzmocgxdv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtvvzpkjlv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtrmyrunsm.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gtjfetwexi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxinkj.top/gtcqaznvbw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtampzijsy.html

Ruby: s.scan(/error/i)
来源：http://hz.hnqzz.top/gtijoirlpx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtbwgfhdef.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtrcsmhhnv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gtkhvcyrwq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.mhx1999.top/gtcfnqszvq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtakmqzgho.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtrsznjcit.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtosvhouyx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtjgyyabps.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtbowgwjhp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtdvwxtqzs.html

================================================================================
来源：http://hz.sxryk.cn/gtwdngpmvd.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtkgzwstxp.html

================================================================================
来源：http://hz.pycfn.com/gtepxtxkfw.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtmebklwlj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gtosbohfev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtqjkgrrzj.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtdrirkzde.html

TS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtqvcmcsvt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtknycluzl.html

Go:   time.Now()
来源：http://hz.yj20258888.top/gtmrqhcrzu.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtfuqaatfv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhiwuduotai.top/gtsellcjdd.html

[J02] 格式化输出
来源：http://hz.jiagoushi.top/gtbiuxfxxl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtdyakvwsn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtrraqvvkg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtdttlxerv.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtyeohmeyx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtlivsowmm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aizwys.cn/gtvcxclarb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtqwheordm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cqqwz.cn/gtxizwxjco.html

[J03] 字符串解析为日期
来源：http://hz.zhengqikj.top/gtnuwaftad.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jlsjyb.cn/gtmkrbvvem.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtducxkyvb.html

JS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtkekgbnae.html

TS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gthvziagfp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gttftyivrb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtaolfvjcn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtywayncdt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtxmfohnln.html

[J04] 时间戳与日期互转
来源：http://hz.ydzc1.top/gtcpxrvdry.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zycfv.cn/gttegbebpz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtsfortagz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yongpay.top/gteejhqfmz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtentqrfvl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtscehtduu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gtzftylegn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gtclwmtwcw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuetiantiany.cn/gtgvbgbzwu.html

[J05] 时间加减（加 7 天）
来源：http://hz.9152youxi.cn/gtxqrywqlv.html

Py:   now + timedelta(days=7)
来源：http://hz.yongpay.top/gtvihazxjb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtjjfzylrp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtvgrqtvok.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtilhxnbks.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtpfmrczcy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gtsvxfpjwr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhengqikj.top/gtzhgatfyc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gtsmlnvfts.html

[J06] 计算两时间之差
来源：http://hz.sxryk.cn/gtgdnkwatd.html

Py:   (end - start).total_seconds()
来源：http://hz.ydjk.org.cn/gtpvluktwo.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtyfgvnroc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gtseuohkwh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gtlhiupyto.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pengpengdd.cyou/gtzcdoanej.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtxllnpttf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtojkguxja.html

C#:   (end - start).TotalSeconds
来源：http://hz.cashguo.top/gtonyvksgp.html

[J07] 比较两个日期
来源：http://hz.dashuyun.cn/gtsymrqeal.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtpsphuvlb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtkmzsgwse.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtwpctswwo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtbjwgafvc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtjreihhyi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.c1oappe.top/gttjhmesri.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtbyamxdkw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtnpumzwww.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtydfujrgh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hfpthk.cn/gtuueigkws.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gttvptzdwv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtyipfgudq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gtiwteniub.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.mhx1999.top/gtjkcexygs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtfytsottq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.52xcode.cn/gtuiodjdep.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtywhzufln.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtubrnllvq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtidibedsl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daxiang520.top/gtqnduomvn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtnikepzvt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtoimibzfh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangkeji.top/gtuldasbih.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtbnycrvdh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtjuaplylm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yangfankeji.com/gtsjohuqxg.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtitesahyn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtrojgedvx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gzhubu.top/gtnjitkcnq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtibwnilfn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.52xcode.cn/gtygcitfkq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hfpthk.cn/gtkxbyacti.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aizwys.cn/gthjsazlur.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yongpay.top/gtlvzutvrq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fzhhl.top/gtgpfqhgnq.html

================================================================================
来源：http://hz.quarkkingdee.top/gthecarsrx.html

K. JSON 与序列化
来源：http://hz.cashguo.top/gtgmagjhqk.html

================================================================================
来源：http://hz.daria6918.cn/gtfyxzgyka.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtxoaorsna.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtcxuswpkc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtsmkyfcpb.html

JS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtywakxuxk.html

TS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtsoazwdyi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtvejlkoai.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtsitfbbsl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jiagoushi.top/gtnokfzykj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtavuixawo.html

[K02] JSON 字符串转对象
来源：http://hz.nanxinkj.top/gtxiqtkhvo.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gtlmitnxqw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtkfrseeak.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtxwahzbug.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtkdszexdk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtiqbkhyow.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtfhoalqmm.html

Ruby: JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtnoorvkjw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtsbtyorrh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shzxlz.cn/gtigmevwgk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuanzx.com/gtsnrtyjeg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtbietgopb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtzvmmsqjt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtocbfxnbu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtareqvmup.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gttzbdwvia.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtmlanllwu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtowvfqofk.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gtxrasvyrq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtwzogychp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtccjkhklx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtxmbqlptw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtsnwjcfkf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtiolxmlax.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtshxvxxrd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.havefunace.top/gtebokivvn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258.top/gtfapacorh.html

[K05] 深拷贝对象
来源：http://hz.chenzaomai.com/gthbezudje.html

Py:   copy.deepcopy(obj)
来源：http://hz.cucudq.cn/gtngxyjcod.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtbyjicsmn.html

JS:   structuredClone(obj)
来源：http://hz.nanxinkj.top/gtbqrylmxh.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtcsvbrbqz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtkfljtguz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtqgkkmddm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gtptergeyk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gtjhlwbkrp.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gttozzhgjd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxinkj.top/gtxsqpnboq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtztnsenka.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtzeftfzhx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtrjzvvbzz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gttswfqwuj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.svipenyu.cn/gtqafbrhaq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gthbghejwn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydzc1.top/gtrjuvxnft.html

[K07] 进制转换
来源：http://hz.andypj.xyz/gtnvmaulmc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gtqtjtehtj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtibbsbycx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtqejfomcr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtslpnxawe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yongpay.top/gtcyqorupk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtjieztxga.html


<!-- 参考信息 -->