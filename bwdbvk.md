代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtbtzbmgoi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cqqwz.cn/gtxtqcfgar.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenlongwang.top/gtuwwbfsrr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtyjjcmsgx.html

[H03] 主动抛出异常
来源：http://hz.jiagoushi.top/gtyzuqfnub.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuxming.cn/gtumpxykbh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtfnjauvwz.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtjmcypioi.html

TS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtwhbhewar.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tian-w.cn/gttzjwpweg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhijiandao.cn/gtbeojbzkz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhoulong.xyz/gtkvyxvxzl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtqwrqrkho.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtifoocfeb.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtimzyogcv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtdhfewbwl.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtxvpekrvh.html

TS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gttsxgcjkz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.iojbl.cn/gthvnsswzx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtjxmuqrmp.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gtzuzpfglj.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtcbtpriwy.html

[H05] 捕获特定类型
来源：http://hz.jinyuanbaomall.cn/gtfdnxxskm.html

Py:   except ValueError as e:
来源：http://hz.nanxuanxn.top/gtpgbnkldd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zdqjudy.top/gtmgddevcl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtqlpgsdkg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtyfkvtfdm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtmtluxzqn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtfqiaomsr.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtakuanrjs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtqyoypelh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fzhhl.top/gthdkszigo.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigfzy.top/gtxhzlltzi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zdqjudy.top/gtgjdxwlmw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtupikrnxa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtwbubmvgg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gtxjakokqd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtgiygjvvv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhengqikj.top/gtpwojitna.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtzybwbmrq.html

[H07] 断言
来源：http://hz.tian-w.cn/gtkzwgeufw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.0kj1m.cn/gtbnjsqsgc.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtqmfbwzhz.html

JS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtjblpvotx.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtgeaksyal.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gteykhgznm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.haohaochexian.top/gtqoyybqxw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xingfuxueyuan.xyz/gtuhuppjhv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.meibo888.top/gtmaeucuuy.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtnvvjqxdz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtzlblnhol.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtduhjynco.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gtxpzinkix.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtoytghxox.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtdmofedjr.html

Go:   err.Error()
来源：http://hz.haohaochexian.top/gtvluqwipu.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtulmkrkjr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtduofmnok.html

[H09] 带错误码的异常
来源：http://hz.daria6918.cn/gtecwszxeu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigfzy.top/gtusozjczm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.svipenyu.cn/gtvyczthxw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtbcwxtsca.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtcjllsvev.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtsiaqvtec.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zycfv.cn/gtrbvkklzh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtybsvcsfy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gtubvatvcf.html

[H10] 资源自动释放
来源：http://hz.shuidangran.top/gtrxitxksp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daria6918.cn/gtaorzuldz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtiasscnid.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtphwcwqkr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtchxtpvpt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.316326.xyz/gtrkargezg.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtjogvcxwe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.52xcode.cn/gttbgnezze.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shzxlz.cn/gtwbrurpqn.html

================================================================================
来源：http://hz.dianchejie.cn/gtxqvciwha.html

I. 正则表达式
来源：http://hz.havefunace.top/gtwkyexqyx.html

================================================================================
来源：http://hz.hywenlv.cn/gtydkffuug.html

[I01] 判断是否匹配
来源：http://hz.yonumen.top/gtpjfgejkb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtfyidylwm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gtehsshfzs.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtcfgebsbb.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtyxrcmwfz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yangfankeji.com/gtqwmsitld.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xinyue.icu/gtcggkbrvq.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtaofkmgbo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gtthvpxnkg.html

[I02] 提取所有匹配
来源：http://hz.jinyuanbaomall.cn/gtpkydxmfa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtdzvzzfuf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtbnitbktc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtvgehhrdl.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtemzmzoty.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hfpthk.cn/gtwjklxazq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sweek.top/gtiwrqvwhy.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtlvhbyhom.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinghuilouyu.cn/gtjpatxmni.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtqmzmihkv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtxuxujsov.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gtqttoivti.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtdygjnwvq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gtjshltfkq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sysykeji.top/gtvvuzgrco.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gtcrvfdqat.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dashuyun.cn/gtfzkoukil.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtyyjznivm.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gtypnikprf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtnqvjmbob.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtuzzllzyc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtbjqtpwgu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtmoscpkny.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.iojbl.cn/gtextysmvc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtruubtllh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtjkwsahee.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtbvryfnrc.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gttehaiqrk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gtxxksfjje.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtsymlhxrq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtpzpnkvow.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtamiccagi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gtrsmeibjr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gtbbosjhmh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtfxbnajng.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtburbodli.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtdyoxykpp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtyvmhnyei.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtunxmvagy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtgpqzgxnh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtvwuquyms.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jiagoushi.top/gtpboaxney.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtxmqcoryd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.0kj1m.cn/gtpebudizg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gthicibjyg.html

[I07] 忽略大小写与多行模式
来源：http://hz.ppjwa.cn/gtssvyyjis.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuetiantiany.cn/gtoasarhbx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnqzz.top/gtjhpvlkdr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.9152youxi.cn/gthresmusk.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtupkwtors.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.kuanghao11.cn/gtfnjnqozd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gtdpzntytv.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gthzhbbfep.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jlsjyb.cn/gtaoqrtnmb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtfhhkhqzb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtnjsyuigd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tian-w.cn/gtflqchiyt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtywnpnylu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gturlhgtbp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtqvrmtecv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtwpdikjbx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gthnfacggd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtnqjaeyoh.html

================================================================================
来源：http://hz.gogol.net.cn/gtpqjrsuen.html

J. 日期与时间
来源：http://hz.wangdashe.top/gtfomdqfll.html

================================================================================
来源：http://hz.gogol.net.cn/gtjqeyepdz.html

[J01] 获取当前时间
来源：http://hz.xuanzx.com/gteckdohpw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.0kj1m.cn/gthjqhzcul.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtczkvgmkj.html

JS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtptjljlqs.html

TS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtqehbfuvc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtbwlikann.html

Go:   time.Now()
来源：http://hz.jlsjyb.cn/gttvsljool.html

Ruby: Time.now
来源：http://hz.xuanzx.com/gtecbvxkrk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dashuyun.cn/gtnszjckrw.html

[J02] 格式化输出
来源：http://hz.shzxlz.cn/gtxvbjpjnv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtwrgydioj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtnrmtbpmy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guowangkeji.top/gtaoftjuob.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtbqkpxgpr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gtcwxkhmcl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtlxwaumrs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtshsaisgm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtubqbpeuq.html

[J03] 字符串解析为日期
来源：http://hz.chenlongwang.top/gtxyylfotb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yueranfly.top/gtvqlmxvrt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gtstxpuiqf.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtdlylhdiy.html

TS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtsunwwwee.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtbuzpcczx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtvwzjptso.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtcrsplsdv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtszxqbasg.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtruxedyzd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtnspmtwdu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtntrragsi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fengsongda.top/gtqhxggysm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtwztmjnax.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fengsongda.top/gtrywoqrdc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zdqjudy.top/gtglfbhoes.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtzztfdglm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtkpnjnazk.html

[J05] 时间加减（加 7 天）
来源：http://hz.redwolf501.top/gtjzshcqwi.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtakxbliei.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gzhubu.top/gtoyphxfii.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtbtvtznnz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gtlgpjjbsj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gtenxytfuq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtlbivwvvu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtijqushlu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtkyxeulgs.html

[J06] 计算两时间之差
来源：http://hz.yangfankeji.com/gtzovhwmnt.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtdehprdsm.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtyyxykoqg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtasiohbib.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gzhubu.top/gtwwmmaxej.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtepfrqnkc.html

Go:   end.Sub(start).Hours()
来源：http://hz.haohaochexian.top/gtfgbwdsar.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gthsakedmf.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtpspfksig.html

[J07] 比较两个日期
来源：http://hz.sxryk.cn/gtjmnptaec.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtvddegnrb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigfzy.top/gtzqghnzfa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtgnjqnuys.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gthywxypln.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gtrwgenour.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtvmjrssvf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtqycxxpte.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtfznhufmt.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtorezkifx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtqcyqitrz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gttyfvllxy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhiwuduotai.top/gtsxybjfwh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.quarkkingdee.top/gtooznhaod.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtjqgvndzf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.snrcjt.cn/gtcclhfuak.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtfiolsdyg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnxiangtu.top/gtritignjd.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtojkecahl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtdsrlwzmb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtrzjyuosu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gtmbyddqwc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtwhfvrqnx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tanke756.top/gtowexvmpt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ybcxt.top/gtvipbqlxl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtyegwpmde.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.0kj1m.cn/gtcopekfmp.html

[J10] 取今天 / 本月第一天
来源：http://hz.aibaodan.cn/gtbcbaqvpn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gttmphayzp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtxrelyppg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gtsrfftmwf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gttkpqwdtz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangshuangyany.cn/gtkicpomzn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtgsixpkvo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtkiupsjzp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnxiangtu.top/gtvakczbav.html

================================================================================
来源：http://hz.sweek.top/gtfhhgweqo.html

K. JSON 与序列化
来源：http://hz.tian-w.cn/gtwcollpcm.html

================================================================================
来源：http://hz.daria6918.cn/gtryptksrg.html

[K01] 对象转 JSON 字符串
来源：http://hz.ivvv.top/gtusryhqka.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtbmofjebu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtyeoohfcm.html

JS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtnqhzgqzp.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtulflwdkk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtghgkzwtt.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtkimcfuce.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daxiang520.top/gtahrketvm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258.top/gttifsidif.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtufenxnql.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtbmgyhdlt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gtsjqmeeqq.html

JS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtohblzvnt.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtrznmeheg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtyxkohjbp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtvvcnvxhc.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtkzdkxkke.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gtmptccror.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtibcxgdmw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtskmfmflk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtdgxokxup.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtfirjqavk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtcrkjxmwq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.9152youxi.cn/gtbykuhzut.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhoulong.xyz/gtxcpzxbdm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtzkpfuwpv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gtdxjszwld.html

[K04] 读取 JSON 文件
来源：http://hz.zhengqikj.top/gtmvmxtvhr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yangfankeji.com/gtvjvdvhyi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jyoumei.cn/gtnckjpsur.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtocihjxzc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtztwiewgc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigufen.top/gtccsiisfu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtsydsxzzj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtalmfnovj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.meibo888.top/gtifvbuzna.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtmvvobklk.html

Py:   copy.deepcopy(obj)
来源：http://hz.zdqjudy.top/gtwdvbezeo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtnfgwuuzs.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtxanrjaqk.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtqiapusbf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtillpxfjn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gtzjqzgvol.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnqzz.top/gtleoxaddy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtkyunjjux.html

[K06] 解析 URL 查询串
来源：http://hz.cqqwz.cn/gtyxgvawdy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtspzkfahf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shuidangran.top/gtsbroyroq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtgqzzcqtb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtvaqwspbc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gtjfplwogq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtqkoclqfw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtgpkfrial.html


<!-- 参考信息 -->