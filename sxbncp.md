代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.havefunace.top/gtnrukjsme.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtjcliupic.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtbudllwwi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtqjgpmhdp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtfirmqnan.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gtkbynzneo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtzhfkvdwn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtjiiilvyg.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtarzvtikd.html

Py:   raise ValueError("错误信息")
来源：http://hz.cashguo.top/gtuuxnflps.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtrpggnpiu.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtdaaxlpyf.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtcnxkkxlp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtowyzwzwl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtbrovjtas.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtcjxguxvp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jianghu66.top/gticxjvzkd.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gtlpjmkgvd.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gtcsvusggg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtbrzpasyp.html

JS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtkliucybq.html

TS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gthkftdptk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ybcxt.top/gtkdhncvop.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtyghmcvby.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gtguhhbqzz.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtbojrbohu.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtatrsjnwq.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gtatdtbwfw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtzrwziiyl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtfdadabmp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtvxpunong.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtevycdgml.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtwiqqrgek.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtbznjgjvu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gttxnlcgev.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhoulong.xyz/gtpgiuqcav.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtvnbzyqmj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtcnsrhhzk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtffabjzdx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtgdexemxn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.quarkkingdee.top/gtppfplgkk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258.top/gtfsqiwdou.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtnribusov.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxinkj.top/gtxcxydhxe.html

[H07] 断言
来源：http://hz.jinqigufen.top/gtzcmrxkga.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtympstsgk.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtaxqpliyl.html

JS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtdvefmzbt.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtgaqdrqix.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hywenlv.cn/gtgegfpwpc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sweek.top/gtkvzxrxhe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtwitvaohj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.bjfxy.top/gtybscocra.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtpzvctcrq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fzhhl.top/gtjwkpgped.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtxplmvfcp.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtoeyzrmno.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtfgclobfc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtufovfkls.html

Go:   err.Error()
来源：http://hz.tian-w.cn/gtjhuxiszq.html

Ruby: e.message;  e.backtrace
来源：http://hz.quarkkingdee.top/gtvlmhpilq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.bjfxy.top/gtmvizjsvk.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtdmnbcbhg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gtpiuwhjpn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtendeqgtv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenzaomai.com/gtmwqtqsag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gtjvlvaytz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hywenlv.cn/gtxjresybd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gtstkqhtve.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ehwqpu.com/gtqlrekrkd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtsdjzqopc.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtdswfkqwa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtayxtlcmu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtyjwjahbi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtwzounqmo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtdpsqjlwl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtjclyfyob.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtbsyyhytp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtkchaqtpa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtgjvaewxb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkbhnawus.html

I. 正则表达式
来源：http://hz.chenjidiqi.icu/gtnudnecvx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgnnypxrr.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtkavkxnri.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtmhjsjfhf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xinyue.icu/gtmrcxkihi.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtucsxzkii.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtqoctlcur.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtybyfmwqt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtkghnxayu.html

Ruby: s.match?(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gtrbwupmxg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.kuanghao11.cn/gtygapogoo.html

[I02] 提取所有匹配
来源：http://hz.jqgufenzy.top/gtuypuzbmu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtfilvhbql.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shangyingyoupin.top/gtilsqasxw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gotoacloud.top/gtbopelzob.html

TS:   s.match(/\d+/g)
来源：http://hz.jianghu66.top/gtzxkdonhk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtmztlqtnu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtrxufaofh.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtskoionux.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gttjcqhkgq.html

[I03] 提取捕获分组
来源：http://hz.9152youxi.cn/gtijgrolnz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtgrcysihm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenzaomai.com/gtzumakgwm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtujylxmxo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtfhyedduu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinyuanbaomall.cn/gtvjtxhksn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.andypj.xyz/gtznxvrljx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.bjfxy.top/gtmatfapqd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtjzxwhhli.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtfgwrephj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtymwwefjg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtnppjxgzt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtwcuyktvl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtezwuutbe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ivvv.top/gtfblwpjng.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hongshengwenyu.top/gtjuxfcxhu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuanzhike.top/gtiodigbgb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuxming.cn/gtpiweeael.html

[I05] 按正则拆分
来源：http://hz.shuidangran.top/gtfpfvegxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.haohaochexian.top/gtwwlqhgsq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtovstklzf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtzyrxlcyv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gthbzovuec.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtxynkrwna.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gtbdlzvoap.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtbnjllooh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtajvcvojj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigufen.top/gtaarddbzv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtnonmcqgw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgufenzy.top/gtugmdnwxs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtytnleahv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtyjqojzmt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shangyingyoupin.top/gtexebtawr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtwdajmypo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtpvwngstj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gthshtywaj.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhijiandao.cn/gtjnzkrdyl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtktgmebxb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuanzx.com/gtfzgwtoab.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtyrpobqhr.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtppnnhcak.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtgwtrozbs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gtenpztuzo.html

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gtiesfdaqr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dianchejie.cn/gtokmugrvl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydzc1.top/gtrcombhna.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtawhqviah.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258888.top/gtgucsznui.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtiqwkoxoq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtqrelpkpi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnqzz.top/gtszteyiuw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gtxiwgtyzs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.iojbl.cn/gtuntsecyi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtyrbixlvy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbyzmdlof.html

J. 日期与时间
来源：http://hz.yvedp.cn/gtvkgsgxik.html

================================================================================
来源：http://hz.wangdashe.top/gtuzjfgexj.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtjkjncazb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gtdbgcgqkf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtcyppksvg.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtfopvxnqi.html

TS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtcgxjtmhd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtwnljrxrf.html

Go:   time.Now()
来源：http://hz.ydjk.org.cn/gtwalqnqum.html

Ruby: Time.now
来源：http://hz.zhiwuduotai.top/gtsvqotqea.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtrtkpbzvu.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtzrcvoqel.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.birdmap.top/gtdtjzvabi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtskivcrwi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtigrdmrlh.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtybbsnouy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cashguo.top/gtroyqqexy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangshuangyany.cn/gtctgbuprn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtqjxdgmwx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj20258.top/gtgwjnrrlu.html

[J03] 字符串解析为日期
来源：http://hz.nwbrower.top/gtwyrrbtem.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinyuanbaomall.cn/gtuuiqejuu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydjk.org.cn/gtysxhfidu.html

JS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtkkmjegqb.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gttsnfwcsi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtqtirgorj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.haohaochexian.top/gthmtiqogz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gttmlldcmu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtwlbusfuv.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtayrdifut.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fzhhl.top/gtlxmojjck.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yangfankeji.com/gtkvxquafg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtdustvmuh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fengsongda.top/gtgkziaebd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtbtcdanav.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtljshsvuq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtcmuvmxct.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenjidiqi.icu/gtrnvlppuv.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhixingplan.top/gtvcpyjavo.html

Py:   now + timedelta(days=7)
来源：http://hz.hammf.cn/gtpejgcqwz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.haohaochexian.top/gtzzpkwulk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtzdrbookw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtkeryfgmc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gttasmwphy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtrxwovldh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtpyxeoval.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuanzx.com/gtmsczaikq.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtsfnpzfsw.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtbevtcgwl.html

PHP:  $end->diff($start)->days;
来源：http://hz.shzxlz.cn/gtjcpxmpki.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.haohaochexian.top/gtjmynmykt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.vqdsnc.cn/gtovxfyprn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtjaijfegd.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgufenzy.top/gtkhlehwig.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtziwgnqtj.html

C#:   (end - start).TotalSeconds
来源：http://hz.daxiang520.top/gtlpdtezlc.html

[J07] 比较两个日期
来源：http://hz.cheryme.top/gtqmkwttlo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtrjtmifiz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtpbasxhxv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtdhrguhcf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtuelujdta.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtvggrahpw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ybcxt.top/gtqtpwmoka.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtvaqrdyjc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtricbxsvg.html

[J08] 提取年月日与星期
来源：http://hz.iojbl.cn/gtfugcdbem.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtyfxnxdst.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhoulong.xyz/gtweojxjdr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtqyxszbtk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtcyrvbxge.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtykgckami.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangshuangyany.cn/gtkkxqvqfj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtcfcgbhdu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtglrzadfp.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtpixtjmlu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtwqwkvkmx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtmncftagl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtebkiktia.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtwjcntiio.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtqiontvbc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gtotmahkei.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtgqvlasba.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenlongwang.top/gtfpcmvmyt.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtpmzsprpu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydzc1.top/gtkjqxnxcl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangtech.top/gtukubnoln.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigfzy.top/gtfkcyhqoj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.svipenyu.cn/gtbnhvykaj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuanzx.com/gtkbahulak.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangdashe.top/gtugsqxohx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtiqeiydby.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gthvrdilgg.html

================================================================================
来源：http://hz.yvedp.cn/gtntiifrbq.html

K. JSON 与序列化
来源：http://hz.yuxming.cn/gtipmobtdn.html

================================================================================
来源：http://hz.dashuyun.cn/gtczqbczoj.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtdnytclai.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtpkvyfuih.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtvewsgudu.html

JS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtxcyiiawc.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtqelcpmhp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gtcbygttro.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtcqzfhzgh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtdjpyyoii.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gthsmjtdgq.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtnrcwcdbt.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gtlfnygcba.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gttlkixukr.html

JS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtrsxnngxs.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtqmxunhki.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuanzx.com/gtjcjsrglp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtkmcjgagt.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtilzxsexf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtuewokhln.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtkohxbuck.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtolheqjjq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtzocaordt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtcxcqidjo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gthgeowyhm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sxryk.cn/gtshynvffi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtxssjjyal.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtmrbimytb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtabeaqcxi.html

[K04] 读取 JSON 文件
来源：http://hz.zhiwuduotai.top/gtnyuvyuym.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tanke756.top/gtsebooahc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhixingplan.top/gtnkdozzfm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtkjzggzzo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtqjuqsubq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtxavfpruy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtdptlnlbc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtmmemqyfh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtgmmcolyb.html

[K05] 深拷贝对象
来源：http://hz.cashguo.top/gtcjdnspfz.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj202588.top/gtesdfahec.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtvandjach.html

JS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtsftprrba.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gttfugcihv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gttetgdfgp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dashuyun.cn/gtmolpzwxp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtiihtbzop.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydjk.org.cn/gtdlfflpem.html

[K06] 解析 URL 查询串
来源：http://hz.cucudq.cn/gtvhnxcxlc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtfkphfrki.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gthkphivho.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtzqtbqsye.html


<!-- 参考信息 -->