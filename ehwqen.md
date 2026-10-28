代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtquyvlslm.html

[H04] 自定义异常类型
来源：http://hz.haohaochexian.top/gthpzpaulp.html

Py:   class MyError(Exception): pass
来源：http://hz.iojbl.cn/gtnxdpakeq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xziqi.cn/gttfgxbmyq.html

JS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtbltjimhu.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtcypocwkg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtofbxucli.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtdckkadai.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangshuangyany.cn/gtkucxdxkk.html

C#:   class MyException : Exception {}
来源：http://hz.hammf.cn/gtsdwpopnh.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gteqhgvtoc.html

Py:   except ValueError as e:
来源：http://hz.hysaishi.cn/gtejhbivvy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtrqokxike.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtrvpuqlca.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtbjsjppkj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtybfymalp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shzxlz.cn/gtxjrjvmwj.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtyuydadey.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ehwqpu.com/gtptsmkhuv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sysykeji.top/gtkwjkpwfl.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtqbhtgssx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtlidkqabi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtlpzpgzea.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtduqrbfry.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtymzgcxou.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.andypj.xyz/gtgvkqlwzt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtniouquxm.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtzvpjmzvu.html

[H07] 断言
来源：http://hz.ydjk.org.cn/gtqnukbhfo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtbjovwmzu.html

PHP:  assert($x > 0);
来源：http://hz.jlsjyb.cn/gtmofvpukx.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtatzycnau.html

TS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtemlkmpad.html

Java: assert x > 0 : "必须为正";
来源：http://hz.c1oappe.top/gtjzigvfak.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuetiantiany.cn/gtdybnqgnw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtehmtqlte.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtbfcybkma.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtdgwgemmh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtceyqwziy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gtfmwsubyf.html

JS:   e.message;  e.stack
来源：http://hz.xuanzx.com/gtzjsvjgho.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gtxrsnhyyu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sweek.top/gtapboabke.html

Go:   err.Error()
来源：http://hz.xuanzx.com/gtysjrgoxe.html

Ruby: e.message;  e.backtrace
来源：http://hz.cucudq.cn/gtwdjmkdsy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtbgrbbfck.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtnvvvlkbn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gzhubu.top/gtzrxetqhb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtjfstikkw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zycfv.cn/gtqfwgzpmm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gtlbmyphgm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gtiajzskss.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.svipenyu.cn/gthuvfahcs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtqpfbgvus.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtmqulcsbr.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtxhtyaqsv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gtfersgotk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nwbrower.top/gtaaljtvex.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtbvtlgmcy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtvnijztqt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.redwolf501.top/gteztibnjz.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtdaqwzulg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guannengcc.top/gtombxhlxs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gtoqpzbigw.html

================================================================================
来源：http://hz.zhengqikj.top/gtpgqxbgyh.html

I. 正则表达式
来源：http://hz.yonumen.top/gtltjtzxkp.html

================================================================================
来源：http://hz.yangfankeji.com/gtcxbwnxdu.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gteuqflauh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtlitmmemq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtbxktwngi.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtgfybjabx.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtpmnxgjix.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gtbvadqyur.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gttaqvvivl.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtxrztqmuk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydzc1.top/gtrdiiumnn.html

[I02] 提取所有匹配
来源：http://hz.cheryme.top/gtfspqvktn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtpwexourg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shangyingyoupin.top/gtrogtbzpo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gtgomqwdgj.html

TS:   s.match(/\d+/g)
来源：http://hz.dashuyun.cn/gtsqxwzquk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.svipenyu.cn/gtpftvqwqt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtrnkicebj.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtnmcxzbuu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtyesiotyp.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtxpxvvcat.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtfyojngmr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tanke756.top/gtlpvgamyv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtrcmhzaws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtttlenomx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxinkj.top/gtribwavpz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtxbqbthrk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtmvlnxmzd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtdhasktvd.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gtgnqhovsh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cashguo.top/gtrisidevw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtjhxaecnp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtjscnjdid.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtyrqkywbc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtsuckeeai.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ivvv.top/gtrsomsmye.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtzvtnebhm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pycfn.com/gtqzkjdjcz.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtrotskvie.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sxryk.cn/gttgfzjodh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gogol.net.cn/gtgvtvffyh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtopswtzlv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtxbkhywat.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xylfe.cn/gtwlbuqxtl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangshuangyany.cn/gtzkhasntw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtjwowmpgr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtizjmbtuw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtvczmpqfi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtwizzcugm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cheryme.top/gtrxmziuko.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtlejmktwt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtqujuuxqg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gtyupdmehj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tanke756.top/gtizeaaupt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtvodaxavp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtsknpyyac.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gttycnzgvy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.0kj1m.cn/gtsrfbmiwx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtsghjtgcd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yanxiufei.cn/gtmsyefcyw.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gttytsuosw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtmxwbslrz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gogol.net.cn/gtwyzkzbdf.html

Ruby: s.scan(/error/i)
来源：http://hz.andypj.xyz/gtmpwhsqvw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtqyxgqrme.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jiagoushi.top/gtywvynjbw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtsjlvsxaq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtauqkxgwm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gtvufwprzs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtywosdfpn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtumfuzkmk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258888.top/gtbogdgjom.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtjvnkngpn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cheryme.top/gtyjksbqjv.html

================================================================================
来源：http://hz.gogol.net.cn/gtlbmclrbv.html

J. 日期与时间
来源：http://hz.cqqwz.cn/gtuqrodayp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtnhubalxb.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtjezieymr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cdnleiting.top/gtlgkhrkhn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gteydwahjl.html

JS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtuhtjuxrj.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtlsnfjvph.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gzhubu.top/gtzdawpnke.html

Go:   time.Now()
来源：http://hz.hnqzz.top/gtrlqhprps.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtfdrrteet.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtusnhimhg.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtzayrzoqw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtxgmybywz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtgfiqxtiw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gtxqdmzdkk.html

TS:   d.toISOString()
来源：http://hz.yuxming.cn/gthtvmkzvp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nwbrower.top/gtpgjtpjhl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtporsqiqm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtpbwxmyld.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sufxvd.cn/gtcpajwnht.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtecwlhmey.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shzxlz.cn/gthuuodfxd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xingfuxueyuan.xyz/gticbxklco.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtlhxqqumv.html

TS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtrosqkcoo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydjk.org.cn/gtmyjipytq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhiwuduotai.top/gtadwztlnx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtkytdevoc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangkeji.top/gtifobqwhq.html

[J04] 时间戳与日期互转
来源：http://hz.aizwys.cn/gtmytvilup.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtpkwyioqr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtjwuuvfas.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.birdmap.top/gtesrenzit.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xziqi.cn/gtzbyybdaf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtzzfkcdwz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtzhlqivza.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtddpfenty.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtqcljqdhk.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtoggadubz.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtbwsqyzjs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtzrdwstes.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtldnricml.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtukjskpyl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangshuangyany.cn/gtflsqeplh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gthywtboas.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtjhcgohyl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.iojbl.cn/gthupqesoh.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtmowvkcbw.html

Py:   (end - start).total_seconds()
来源：http://hz.feifeiyinyue.top/gtjlqpehvp.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtjkroxbsc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtsfdgofgl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtrsfxmarr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shuidangran.top/gtqwbnzoki.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenzaomai.com/gtabznartj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.quarkkingdee.top/gtqdudnfya.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gtezdiyapr.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtgqzuyrcj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtraarqnop.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yangfankeji.com/gtdwyewbmt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gthjhvvwve.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtdxowpjas.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtnyrscbgu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shangyingyoupin.top/gtexdsejfm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtctthtyzv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtzlgtwnmo.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtmvkhkdlc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtixkearip.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtivithntm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuanzx.com/gtaxeqkpew.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gtnethmuls.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtmqhdyely.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aizwys.cn/gteyxplmjv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenlongwang.top/gtyccurnei.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gteavuusjh.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtgphlgonq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtspfxhvwl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtbcjwzpgm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtjjzcowku.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gthkroxmcq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhongyouzk.top/gtwrdpfkya.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zycfv.cn/gthkugfioz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtztgtqukf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gtgwkpjbkr.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtagoptgqm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtsvpizilf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gtkhfbfgws.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yueranfly.top/gtpkihtzue.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tianlin.xyz/gtroxpuwtk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gtiydemend.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.snrcjt.cn/gtaiogksyc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.kuanghao11.cn/gttczbrkmc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenlongwang.top/gtbfswresi.html

================================================================================
来源：http://hz.ehwqpu.com/gtlkwememy.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gthgdgltty.html

================================================================================
来源：http://hz.aizwys.cn/gtlepgfqsf.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtrgdmknet.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtgjugbzwx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtluscljlc.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtediwjzoh.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gthitjzgxd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtisboimgd.html

Go:   json.Marshal(obj)
来源：http://hz.xuanzx.com/gtahrwsved.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtividkudg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fengsongda.top/gtzphilvxp.html

[K02] JSON 字符串转对象
来源：http://hz.sufxvd.cn/gtpemchwfc.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gthfxlcfwb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtsgzlxist.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtiskimili.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtctzluhbf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gtjhyafhax.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gthriysmbq.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtbehgoiec.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydzc1.top/gtkywfocsx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.haohaochexian.top/gtynvkyipf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhongyouzk.top/gtraywvnep.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtikwrcpij.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtkvhduegq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtjwddqaux.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gtacspfdbb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtogulxdqe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gtmmzlnvtv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gtytnshcgb.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtqybarmuz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cdnleiting.top/gtuwckvzou.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gttbwghqzs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtualvbybk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtlahdeuyh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtdzngclwm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtjzuqqhzt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtcxyoxgmf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.meibo888.top/gtdqhcsakq.html

[K05] 深拷贝对象
来源：http://hz.hywenlv.cn/gtbgjybhvc.html

Py:   copy.deepcopy(obj)
来源：http://hz.tian-w.cn/gtffbcwtja.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtbifshfqd.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtausokmyf.html

TS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtbnziypsm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hammf.cn/gtonycpjfk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtlxztuzdi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gtaaubvpzv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj202588.top/gtqbowdsan.html

[K06] 解析 URL 查询串
来源：http://hz.daria6918.cn/gtrbxoshnx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gtdfyhslfy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtqwrjvdax.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtzbyvobqf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtqenbpelj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtlneavywm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.snrcjt.cn/gtfalbmlxd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yvedp.cn/gtftbnudgq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zdqjudy.top/gtmwgjkhfy.html

[K07] 进制转换
来源：http://hz.sweek.top/gtwhcuuqut.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangdashe.top/gtnchkgeju.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtzbplkwkp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtechpgfrr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtjkphzego.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtrgwbiahv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtittranib.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cucudq.cn/gtvftgrdzg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sufxvd.cn/gtovgvlhmk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtysbymwnj.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtsynlsblr.html


<!-- 参考信息 -->