代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtwaevivbr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtbkjdpmad.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtlqhdgzko.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.316326.xyz/gtizqreqmm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gtulkoiuku.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtfuweqpha.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtfrscpftd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhoulong.xyz/gtvawifqfg.html

Py:   value = d.get("k") or default
来源：http://hz.hammf.cn/gtkzyowoba.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yangfankeji.com/gtyffelwcu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtmzwkfglm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtrnwrvvvt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gtjcwyzmsm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtvrhogrcq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtmwrswlpm.html

C#:   obj?.A?.B ?? default
来源：http://hz.shuidangran.top/gtkiblddzj.html

[H07] 断言
来源：http://hz.yanxiufei.cn/gtktajepxt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtcnfrvvlh.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gttdqxzgqx.html

JS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtuquvsuek.html

TS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtjqmeroor.html

Java: assert x > 0 : "必须为正";
来源：http://hz.birdmap.top/gtzggrxzxh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.52xcode.cn/gtxvqkxhyv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jiagoushi.top/gtegogasvy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtpiirtqhk.html

[H08] 获取错误信息与堆栈
来源：http://hz.smart0.xyz/gtivfibhpq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigfzy.top/gtzwmsmypg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtogxhublx.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtktupewhc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gaohongyu789.top/gtoherjajx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xylfe.cn/gttqnmagnw.html

Go:   err.Error()
来源：http://hz.birdmap.top/gtbxbffdxv.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtokavotib.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cheryme.top/gtvcilwoii.html

[H09] 带错误码的异常
来源：http://hz.chenzaomai.com/gtmpvmqmxr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gthceovwpv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtprvbiovr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtrsxqgtri.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuanzx.com/gtoxrikedt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtvnuxidut.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.bjfxy.top/gtyabsekfa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtgerjvwvt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtmvscuuzf.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtwqgeqamp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daxiang520.top/gtnfrfnexh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhongyouzk.top/gtsagehmgc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtwtardqqf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtsmdwqzsh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtifgwofxx.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtfmmnntzp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtswwnnfrn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydjk.org.cn/gtchzitqap.html

================================================================================
来源：http://hz.shzxlz.cn/gtfirjpapu.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtrjwyemkp.html

================================================================================
来源：http://hz.jinqigufen.top/gtyceeaswl.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gtagrczjxr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtlpinqfpu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtdlmdbpwj.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtqexeaweu.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtcncpznpv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtjxdgfxqh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangshuangyany.cn/gtgewoyahi.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtrylnmsvk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.316326.xyz/gtikgmamjl.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gtkmsfqubc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtybhqfapy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sweek.top/gtcmhyehgw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gzhubu.top/gtilgxkldi.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtoqqfrpmd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtsxgoftay.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtrnvqistc.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtbaypfmfm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtgghfggvr.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtkvabxqgz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gteulbhgjo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtgjdmslnd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtjbkabter.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nwbrower.top/gtwestdofz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtvzweyifh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtoqnnftzu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtdaexkfbl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtkulxdlio.html

[I04] 正则替换
来源：http://hz.dianchejie.cn/gtrjyafqsm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtloirxxez.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtlaijxjyp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtqwadxrpc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtaxlwmsrx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gteliqdili.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtizbksdkq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtrmmvluka.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shuidangran.top/gtxzdvwxkv.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtfgthexxb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhaomingkeji.xyz/gtiayqgryk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhixingplan.top/gtqarghvmh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtjyhvqqox.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtjfsbfegm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.havefunace.top/gtcgllyqgm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtpayiwyqn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtlbiztlcw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gttchbokkj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtbtsdxykz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtquswexyq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtomeqscfv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtgrixjoiu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtyrbmnmli.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhengqikj.top/gtnppygmcp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.vqdsnc.cn/gtdxgisjdb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.c1oappe.top/gtofovhbph.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtuiemjmre.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtnklanotu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sysykeji.top/gtrnqqeaqo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtfjidpocx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtolxmrxax.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtomvjwrfo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtqmmcnahm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ybcxt.top/gtebnzynrq.html

Ruby: s.scan(/error/i)
来源：http://hz.aibaodan.cn/gtmaqfqkia.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nwbrower.top/gtobajviky.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daxiang520.top/gtijucogoo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gtzujeljmd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangdashe.top/gthsunsucu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtyxooxmru.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtoriwwovb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtbnxvqsqj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtuqhdrymk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtlxusxtcx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtqfrlpamy.html

================================================================================
来源：http://hz.fzhhl.top/gtwudkymno.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gtuqzkdlde.html

================================================================================
来源：http://hz.xziqi.cn/gtlrmjxwkx.html

[J01] 获取当前时间
来源：http://hz.yuxming.cn/gtobrtzknu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xylfe.cn/gtbqtevafm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtgdywebtt.html

JS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtcyzggulw.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtjwfajyjw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtwmjnfeqc.html

Go:   time.Now()
来源：http://hz.yvedp.cn/gtinkycnzt.html

Ruby: Time.now
来源：http://hz.birdmap.top/gtgknmdien.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangdashe.top/gtpfsluxoo.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtspgsusbn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtlktqcybn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtiormmwxr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gthpzpgtta.html

TS:   d.toISOString()
来源：http://hz.aizwys.cn/gtnnaerlbe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtlejpgrrt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258888.top/gtpvfhxfdb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gttdzititt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuxming.cn/gtkqfvncjx.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtjaanpqeb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.c1oappe.top/gtfdxvydxq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gtphjbdxoy.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtshqhejfh.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtkrbzzhqt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtagaimbfb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gthrbwenfq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtbtnjgcqs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtytmgspye.html

[J04] 时间戳与日期互转
来源：http://hz.hnqzz.top/gtiypmbhbr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gthcuuprtw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtvujxkujc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtwbaqyfhp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gttntyzekd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gtrsybuzra.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtrigzuuhr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yueranfly.top/gtaviliuup.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.feifeiyinyue.top/gtqxwbenzd.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtgscdorzc.html

Py:   now + timedelta(days=7)
来源：http://hz.zhoulong.xyz/gtnntrdqmm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtbkuibrcw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtjpqdnjqr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtcjyfhrix.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtpmxaunaf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xylfe.cn/gtuaovdquk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtqpgfbdmp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cucudq.cn/gtysvivknm.html

[J06] 计算两时间之差
来源：http://hz.wangshuangyany.cn/gtxuvakbtl.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtcogneexs.html

PHP:  $end->diff($start)->days;
来源：http://hz.hywenlv.cn/gtfwaggecl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangkeji.top/gttesbxsce.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gtgtrinsrh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangshuangyany.cn/gtqlqzjixf.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenjidiqi.icu/gtjsxzhrxs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtifcfujbm.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtigofkjpj.html

[J07] 比较两个日期
来源：http://hz.zhongyouzk.top/gthnojgebs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtfabncpcg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtxjzrghxn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtgmvlgkpg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtvrbobkcs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hfpthk.cn/gttpudkmmr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydjk.org.cn/gtssivflvo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gthwitexpd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtefswhraw.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtsgyjlsde.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtaynnoowz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shuidangran.top/gtbtxtjdgp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtttdpiexd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gtwggwafpf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtglevfzch.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tanke756.top/gtegnihlgv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtgnramwae.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtdpgbqyph.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtadhodrlq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtqjjgekec.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydjk.org.cn/gtmfilwlfx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtqoxbreqo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gthdglygyj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gtgatmfqbc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtukukrueu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zycfv.cn/gtuyuffeke.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gttyzkyvbt.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtwlobfgxq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yonumen.top/gthgrdwoiu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnqzz.top/gtwaxbjuiw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.iojbl.cn/gtzfexumxs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtdalumgub.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.havefunace.top/gtbvwlayki.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.c1oappe.top/gteyshjcht.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuxming.cn/gtrfrltsxq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhijiandao.cn/gttxuzjqux.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbrrmciie.html

K. JSON 与序列化
来源：http://hz.jqgufenzy.top/gtqkmkpbpl.html

================================================================================
来源：http://hz.hywenlv.cn/gtivplmdjy.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtqfitigry.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtakrcfccu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtlekdisfx.html

JS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtmzihdxma.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtykrvbtvk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xingfuxueyuan.xyz/gtzczlneal.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtgyudlrsy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ivvv.top/gtyvamdjfz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtinwgdszt.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtgqevdraz.html

Py:   json.loads(s)
来源：http://hz.fengsongda.top/gttjqjxndp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtldrfkrsn.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtcboffyxi.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtpolzoyqs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtwfcxxdlh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtslskoaxc.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtxrynokow.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.haohaochexian.top/gtobddbqlp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ivvv.top/gtcbxsbrjl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtgoflhimz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtmwwsmxvs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtbumwavjv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtsoepidsi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daria6918.cn/gtjooywrnu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhoulong.xyz/gtsqagxbtb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangkeji.top/gtwyzhmjyk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtkfrjwqkg.html

[K04] 读取 JSON 文件
来源：http://hz.smart0.xyz/gtyfdngzkx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cheryme.top/gtefdhlnaz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhaomingkeji.xyz/gtupgoernn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtjnnjtlrc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtnhluxktu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gthlirttqa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tianlin.xyz/gtfwdenxtf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.svipenyu.cn/gtykxfurns.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtpgqonucn.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtmfrnxued.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhixingplan.top/gtitzczqin.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtqekwsgip.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtugcjmnjm.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtjdimkkal.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gtragytgxp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtkadqmkqv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangshuangyany.cn/gtxjogqyzo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtccadxeei.html

[K06] 解析 URL 查询串
来源：http://hz.xuetiantiany.cn/gtrjvvypni.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtweyfzytl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtbdupfvkh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtewozwkep.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtsyuqkpfo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yangfankeji.com/gtzvrlqjlc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtijvvrpky.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtzdyenwfo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258.top/gtxmqzwyvk.html

[K07] 进制转换
来源：http://hz.cashguo.top/gtjvtayhig.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtnblvgkxt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gttflixjzl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtthefnble.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtoeurtgyq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtyfkttfom.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gtzogmqiyi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gtqdnwycdq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtqignincj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ivvv.top/gtbmdrvndq.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtfktqqhga.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtxgstemmx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtbaaafaaj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtxpfmcgin.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.smart0.xyz/gtktkydpuw.html

Go:   encoding/gob
来源：http://hz.52xcode.cn/gtkvytvhbz.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtooltbsws.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gthastnmdi.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthjkdpzib.html

L. 网络请求
来源：http://hz.cucudq.cn/gtwbzufaxt.html

================================================================================
来源：http://hz.aibaodan.cn/gtlkqueefh.html

[L01] 发送 GET 请求
来源：http://hz.chenlongwang.top/gtagzurzax.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aizwys.cn/gtnjgcamsl.html


<!-- 参考信息 -->