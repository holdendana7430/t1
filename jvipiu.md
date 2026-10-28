代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtanhntjlk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtbynhakst.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtvfoerfxl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtqejykker.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtztgpddxz.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtsfbygvbw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtehramdez.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jlsjyb.cn/gtyiehduea.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtbpvgxcye.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtlfnacsbo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtkpgdbzxi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gticlnyhzd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtndhojdry.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shangyingyoupin.top/gtvpzguhls.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gttmwrgnsz.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gtuxskwitj.html

[H07] 断言
来源：http://hz.nwbrower.top/gtjmwmthwk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtysaqcsin.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtwkvlbwlq.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtnljohuqx.html

TS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtsryuwozg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gthhbbczye.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtjordytoo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtslitasdo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxuanxn.top/gtggxapghg.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtzskfflmt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sweek.top/gtqbjvlpkk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gteasarnzw.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtkjpoubhx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xinyue.icu/gtqsobfxhl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ehwqpu.com/gtjlpretqi.html

Go:   err.Error()
来源：http://hz.ydzc1.top/gtiempbabj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtqgjqxxnh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnqzz.top/gtadhxpxax.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtszxvyxgi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jlsjyb.cn/gtxzvgzlnv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtoudkfuta.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtdulesrgq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ppjwa.cn/gtuzhayxvn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tanke756.top/gtittplijw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtwedujedo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.havefunace.top/gtbdpwaawa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtubjxeili.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtzpsonedk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gteofxakuo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtiporiupg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gttyxhbdcs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtkwlgphbi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258.top/gtebofacfz.html

Go:   defer f.Close()
来源：http://hz.wangdashe.top/gtizqdszws.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gtvmjsgyzk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gttyqiziux.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtumplcgbp.html

I. 正则表达式
来源：http://hz.xziqi.cn/gtmjrbnzwr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmmshymzk.html

[I01] 判断是否匹配
来源：http://hz.zhiwuduotai.top/gtrhokikud.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhongyouzk.top/gtaqraecdv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daria6918.cn/gtnpzsebnf.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtfgilmsms.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtjebqxpei.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.kuanghao11.cn/gtwiknbpht.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gzhubu.top/gthvidebfb.html

Ruby: s.match?(/\d+/)
来源：http://hz.shuidangran.top/gtgqvkntrz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtdsefsdxa.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtmpmvibdm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtccanhewz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.52xcode.cn/gtppnispie.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hammf.cn/gtskvnevel.html

TS:   s.match(/\d+/g)
来源：http://hz.quarkkingdee.top/gtwlpunuut.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gthuafccuz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj202588.top/gtnemiejie.html

Ruby: s.scan(/\d+/)
来源：http://hz.guannengcc.top/gtyfsxcvav.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtbsexnioo.html

[I03] 提取捕获分组
来源：http://hz.iojbl.cn/gtxofzjhyu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtdyvjapqs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gtukvaahiz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.kuanghao11.cn/gtrrixorbx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.feifeiyinyue.top/gtkfpjdrvh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yangfankeji.com/gtiqnvgkqo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.smart0.xyz/gtroqzebgq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtabovldkx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gtrjonhdpx.html

[I04] 正则替换
来源：http://hz.ehwqpu.com/gtfkqyapph.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigufen.top/gtgnacugwk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtgzitisjf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtzamsirse.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gthpkxdzft.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtlomtvpgr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtkmvrtuwd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuetiantiany.cn/gtgsyihvsl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gteligjmyb.html

[I05] 按正则拆分
来源：http://hz.daxiang520.top/gtytxwqrrq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtyvgukljc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gtggvrphma.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtxxuyuitu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtsphwdlpj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hysaishi.cn/gtsrrtknir.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gtfprxrzpd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtisdzjiaf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.52xcode.cn/gtmcuvrljf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxinkj.top/gtzxbzkyqu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtrufiddkk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydjk.org.cn/gtxlanflkg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtbympryed.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gtavbpneyx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jianghu66.top/gtzikybegr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtqwphctjw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtpxtwjotx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtkuspauem.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhijiandao.cn/gtwxhhekhd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtbjonucss.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gttugkmjcr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gtpmzmfgsw.html

TS:   /error/gim
来源：http://hz.ppjwa.cn/gtbzfqsxxp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhaomingkeji.xyz/gtdbqvgmjw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.andypj.xyz/gtozenijgp.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtowdxwngv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangdashe.top/gtcercjtjd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gaohongyu789.top/gtrxzyyykp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gttlpmyboy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuanzhike.top/gtnhkkhhqb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtdglnckur.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtmntrfhyu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.smart0.xyz/gtdcfcdpua.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yongpay.top/gtfayiahnt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gotoacloud.top/gtgjffkgfq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtrbctlfqg.html

================================================================================
来源：http://hz.wangdashe.top/gtkibdfxej.html

J. 日期与时间
来源：http://hz.zhaomingkeji.xyz/gtqkybstib.html

================================================================================
来源：http://hz.smart0.xyz/gtmfiegzen.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtlyotywrl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtmnkinvrx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtwbsmjyqk.html

JS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gttvmwetrv.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtcwcctemi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtnrpbwxlb.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtpqrmopvw.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtbovxiapp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.mhx1999.top/gtloeuuubx.html

[J02] 格式化输出
来源：http://hz.quarkkingdee.top/gtqocdttgx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtdtlaocuj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtanhnfcac.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtfwmxibdo.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtuagyjgem.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtnwmvbodj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenlongwang.top/gtnzuhmouv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtglcqvuyx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gttfdlrreg.html

[J03] 字符串解析为日期
来源：http://hz.cdnleiting.top/gtnzjuopqa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.quarkkingdee.top/gtehijvupg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtqzkdpokv.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtpwklvakz.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtrrruknlv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtmubselfo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigfzy.top/gtolpejavc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtsvnquywk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtonticmxq.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtamxjswzv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtkrxhjqbj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtflvjsoux.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xylfe.cn/gtxkavswgc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigfzy.top/gtivnkhuxi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.52xcode.cn/gtutlhbdhd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtvggazcaq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtmhltmulk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daria6918.cn/gtqdqtykvv.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtksirhwhz.html

Py:   now + timedelta(days=7)
来源：http://hz.zhongyouzk.top/gtcmcmrtux.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigufen.top/gtikzbunug.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtmgewgivx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtmbahfvxm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenjidiqi.icu/gtyurjvbek.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gtrfozscgs.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtnpgssnsd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gaohongyu789.top/gtybrsuoya.html

[J06] 计算两时间之差
来源：http://hz.gaohongyu789.top/gtucmvddan.html

Py:   (end - start).total_seconds()
来源：http://hz.gotoacloud.top/gtkdsbwmwb.html

PHP:  $end->diff($start)->days;
来源：http://hz.dashuyun.cn/gtxusnmksu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtbicolmqo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtaotyqyuh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtrjdlnqrc.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtkiuiusus.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydjk.org.cn/gtuzurgese.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtvhasyzmt.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtjeqxiian.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtyxupuqyc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtwxtzyhqm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtuofdbeyf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtmsinbbtj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gtnqucfvnp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtpvejuwla.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtzhbbymvp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtflbclipz.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtnjfofnws.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtvsijkegp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtnrcebone.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gtbwunonyn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gtxfbeciph.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxuanxn.top/gtinrerese.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tianlin.xyz/gtcutqsxng.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.smart0.xyz/gtkortcqey.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yangfankeji.com/gtcgtzzhqu.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtdqonatwo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuanzhike.top/gtogrpsxkz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtqngiugjx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtmipocpxi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtmfoydxzn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gtpfpzqvuq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtfuwbrwev.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtexujtewk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtopcvzquq.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigufen.top/gtxzofrdih.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtybyfwuye.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gogol.net.cn/gtrwdfgsrg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtjqstdnuh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtyjopctkx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jiagoushi.top/gtaqpalsrj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtixkotbzp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtthfnixdy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigufen.top/gteazuxtod.html

================================================================================
来源：http://hz.snrcjt.cn/gtvbzxzjqi.html

K. JSON 与序列化
来源：http://hz.yuanzhike.top/gtfovruvgj.html

================================================================================
来源：http://hz.fzhhl.top/gtvmwtidse.html

[K01] 对象转 JSON 字符串
来源：http://hz.tian-w.cn/gtlesnmhks.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtclayxvny.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gttbqwcdki.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtgjzztmjq.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtiskebocw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtpqhgjyhe.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtruixfrnz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtzcvroshy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtfadifznz.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtmlfysbnj.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtclggpxlp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigufen.top/gtchsjlbht.html

JS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtdntgaivj.html

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtpgsslauw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtpdyzveyl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtcrlhtest.html

Ruby: JSON.parse(s)
来源：http://hz.316326.xyz/gtfxpqlrgb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtofgtlter.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.c1oappe.top/gtvotqyckx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtekdzumkv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtdjjgjuff.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtsmlouxma.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtzgxrqutx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aibaodan.cn/gtzzduicap.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tanke756.top/gtommisvht.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aibaodan.cn/gtpyszhdlw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtffkeklne.html

[K04] 读取 JSON 文件
来源：http://hz.andypj.xyz/gtktgqbygg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.iojbl.cn/gtxufnavfy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtjhqjvheh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtsvqlfigk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtjsjsijfd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxinkj.top/gtfydtqjcc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtyzkjyxbj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ehwqpu.com/gtmupgrtoh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtfudenvmu.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtmkjzlhdw.html

Py:   copy.deepcopy(obj)
来源：http://hz.bjfxy.top/gtfcrioeov.html

PHP:  unserialize(serialize($obj));
来源：http://hz.0kj1m.cn/gtqodmzbtg.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtfyxnooge.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtnmizszja.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtxfsraola.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxinkj.top/gtizxvkffd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gteuiiwidy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ybcxt.top/gtraykdykq.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtapucwncr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtbkedddbx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtsnpnyccj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtqlznxaag.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtwvuaafzl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cucudq.cn/gtzmiscngs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtafwysuxk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtaknoulrz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtkzlkacqg.html

[K07] 进制转换
来源：http://hz.hnqzz.top/gtxtaiwehu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtlgcywqwq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aibaodan.cn/gtvfsphyzk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtcctnybky.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtoossdowr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtynsdlyri.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtjoaslqfj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.svipenyu.cn/gtmmrqmvag.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtpmbnbkah.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtyowwndpk.html

Py:   pickle.dumps(obj)
来源：http://hz.yangfankeji.com/gtonvgrpee.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yanxiufei.cn/gtdflykbfv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gthajtrxvo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtdvfcwxkj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtvmegdklj.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtgxvvbakb.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtyunpfiwy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gtghtdzyst.html

================================================================================
来源：http://hz.cucudq.cn/gtimrhzqvu.html

L. 网络请求
来源：http://hz.yueranfly.top/gthqgmadqb.html

================================================================================
来源：http://hz.cashguo.top/gtodilopvi.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangkeji.top/gtemdjnzbc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gtaebwdkqd.html


<!-- 参考信息 -->