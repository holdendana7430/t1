代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gtwapeltpr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.52xcode.cn/gtfewxkygz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtbqybozya.html

[H02] finally / ensure 收尾
来源：http://hz.yuanzhike.top/gtoptqgubt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtgnjrnich.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtfmsfilxh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtnmpoztmf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtkocfpaup.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gthstyslaa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtjmhptpbs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nwbrower.top/gtmisknamh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gttlqsgfex.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gtdqbrhcvy.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtnfyhywox.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtnqupjnnn.html

JS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtolngicbz.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtslmedlle.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtsanqtwis.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxinkj.top/gtueylkfhc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jyoumei.cn/gtoavudece.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtuqomtrew.html

[H04] 自定义异常类型
来源：http://hz.ydzc1.top/gtrbjhbotp.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxinkj.top/gtsrrgzist.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtackqykya.html

JS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtypdotvlp.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gthussmilj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtywctbita.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtchowpspn.html

Ruby: class MyError < StandardError; end
来源：http://hz.yvedp.cn/gtxsyqysou.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtggnrucmh.html

[H05] 捕获特定类型
来源：http://hz.cheryme.top/gtnrokeqtx.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtwpsukkwg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenlongwang.top/gtebemfnyy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtdsvlnmni.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtbyixqiyd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ehwqpu.com/gttfrcvnzb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtlqvrozsl.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangshuangyany.cn/gtzkjxpbst.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtlhhoiybb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtabswdtyx.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtogeeickf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.pycfn.com/gthfxxvcco.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtmshxpfsg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtbtralwof.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtwkvindxl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhengqikj.top/gttwlgvmgc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtvyvwppot.html

C#:   obj?.A?.B ?? default
来源：http://hz.fzhhl.top/gtfcduhuqs.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtlmwihqwl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtetasrjrg.html

PHP:  assert($x > 0);
来源：http://hz.vqdsnc.cn/gtyrzlcdvz.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtrsmcneax.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtbfbvwswm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sweek.top/gtejvbzfer.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gthuzgtxtg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shzxlz.cn/gtnkwbuqny.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtsbpvcyuh.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtbueyfrif.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.316326.xyz/gtoxbaukjb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtzkcxjdei.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gtyqlndoeq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dashuyun.cn/gtnfsszssq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.bjfxy.top/gtnpnomrhj.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gtxrpowtbv.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gtzycansbs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nwbrower.top/gtkjmxcawh.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtptwvtybs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuanzx.com/gtcokgumob.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.svipenyu.cn/gtjjxfbszo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.andypj.xyz/gtuahgnlpt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuanzx.com/gttgkcjnil.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangkeji.top/gtiiofcqbz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtaabqlaoo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtsqqgrzof.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shzxlz.cn/gtmungcfzo.html

[H10] 资源自动释放
来源：http://hz.jinghuilouyu.cn/gtkhljzmdx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigfzy.top/gtdopaxmdw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yongpay.top/gtqvzplqbj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtxtekttct.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtkiqyfwtd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtchrglrzf.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtzetjrfyt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtcswevwzt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtungobbhl.html

================================================================================
来源：http://hz.chenzaomai.com/gtxywdiutz.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtnsyyijhf.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgrlopnde.html

[I01] 判断是否匹配
来源：http://hz.zhengqikj.top/gtqlessyjt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gthiosmera.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtjvuvmgzo.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtjfedlcbb.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtoauowuhl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nwbrower.top/gtgllmlzwt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gtpwgzgjkv.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtmfwouugk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258.top/gtayupxytz.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtfipchbqn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtjqrblabf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.havefunace.top/gtzjqwgnhh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jianghu66.top/gtddasgsti.html

TS:   s.match(/\d+/g)
来源：http://hz.hammf.cn/gtfmsdqjik.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtzgvttvqr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.kuanghao11.cn/gtbinylxlb.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtrnmbgixs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zycfv.cn/gtcnurnhxv.html

[I03] 提取捕获分组
来源：http://hz.cucudq.cn/gtgootsmoj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigfzy.top/gtqvpnaqms.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtihozgrgc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cucudq.cn/gtvusxpbxk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtqbivvyjg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gtceofukhc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtkcmhuipk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cheryme.top/gtxdcxpxye.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtbdfoomcj.html

[I04] 正则替换
来源：http://hz.yangfankeji.com/gtclpwbuib.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtvrqtxrrk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtkwppzooq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtaxwsltah.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtcpvfagdm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtpplpvgqp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pycfn.com/gtiroaqjzw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtnhlhbazb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ybcxt.top/gtlqqxlfcl.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gthitrsujm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtowlaautw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtxmlnicvw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtfloqoheh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtgvhpoeoz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtklufelua.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtzfovcyns.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtiizglows.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.redwolf501.top/gtmrgsjwiv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtbdsjdfaa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtcbowuyjt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj202588.top/gtskdlsvxu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtmolihojc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtrbiwghho.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sweek.top/gtpbxzdfiz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtxeaobkjo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigfzy.top/gtmqxongjt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtexlvquad.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtlsuuevad.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtupjknchb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtxvkwtgyk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtuijtsupw.html

TS:   /error/gim
来源：http://hz.havefunace.top/gtuvvgxbzn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dianchejie.cn/gtwcepvncv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gtaivoihwx.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtnxjqjwtn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtpnqnslyx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtcyvjyden.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhaomingkeji.xyz/gtjcfacawl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xziqi.cn/gtfnyejuma.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtmpkbxxgj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtrstzlcca.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtrjzwmsuw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtrggvzykd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gtltyajegf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtkbsjluuo.html

================================================================================
来源：http://hz.zhengqikj.top/gtfvgnddst.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gtpbthyjsy.html

================================================================================
来源：http://hz.tian-w.cn/gtsfpfzlfx.html

[J01] 获取当前时间
来源：http://hz.jinghuilouyu.cn/gteqemmors.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hysaishi.cn/gtuustzyxa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtpcplgmpq.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtfowtpbwf.html

TS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gteqlfgoyf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xingfuxueyuan.xyz/gtknztqxrp.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtnufvyfhj.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtlprtfdgs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenzaomai.com/gtgojnzeuc.html

[J02] 格式化输出
来源：http://hz.ehwqpu.com/gtfrxtgpsp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtakrdcoij.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtlceorutw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cheryme.top/gtqzcwtvoh.html

TS:   d.toISOString()
来源：http://hz.cashguo.top/gtuwazbgvl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dianchejie.cn/gtmumifcfv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtnxipehxq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtrajeyrlg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtdcgyuzij.html

[J03] 字符串解析为日期
来源：http://hz.meibo888.top/gtoquwdcls.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtuakulwzo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtszwllxge.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtgmauknap.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtalnbmyfe.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtlflcztgj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gtabzhpldr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtwgasrzpx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gtcchhhpmp.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtgerkwhhy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shuidangran.top/gtjhhhicby.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gthamrmgir.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hongshengwenyu.top/gtbcbhilyl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xylfe.cn/gtaldhduhk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtbcgzwasc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gttqgymzbw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtpaqglisb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtlummsluw.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtkplvymqm.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gteunqvfbm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cashguo.top/gtztzqouwe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtcpuoipre.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtnpacpxfn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtkcydbjcb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtcduclxft.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhaomingkeji.xyz/gtcevsaspm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jiagoushi.top/gtepdktjpm.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gthaqxuvdv.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtobzgowwf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jyoumei.cn/gtddhsdtnw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xinyue.icu/gtbpjsrpro.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtnhucenxc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtghnqijzc.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtrjeyssye.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gticjftqov.html

C#:   (end - start).TotalSeconds
来源：http://hz.cashguo.top/gtkvncvvwj.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtmdpmebec.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtjyohntqy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cdnleiting.top/gtzvfiqkvq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gthnmhmjrp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtipsolyag.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtrblolnzf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtdypndyxk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtrwtswqgp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtsmjbesrl.html

[J08] 提取年月日与星期
来源：http://hz.redwolf501.top/gtchjiqiyz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.andypj.xyz/gtvblkyrek.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangdashe.top/gtbieoyzmd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtwumjnpfk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtwzbogmtn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgfzy.top/gtiakewded.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtvpufdzjr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gtyvmxumaj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tian-w.cn/gtrozifxxc.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtxuoawwpl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtarycqibq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxinkj.top/gtqfhgraha.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gtmydojlpo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtmhtexmfh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtajhtleab.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhengqikj.top/gtnainryny.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtlkuewfmk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtgbvsubxh.html

[J10] 取今天 / 本月第一天
来源：http://hz.ppjwa.cn/gtxdppczuz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtkycadkwr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtcdxvolse.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ywan-chungtsiang.top/gtcfbjoamr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtenkragfo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fzhhl.top/gtbjmriohr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.0kj1m.cn/gtzaadvedh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xziqi.cn/gtsdovjbys.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.c1oappe.top/gtghreocsd.html

================================================================================
来源：http://hz.daria6918.cn/gtcpwtsedj.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gthtdxbahk.html

================================================================================
来源：http://hz.cqqwz.cn/gtsurpmdff.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtwhwspiqc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtbonhltmx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtphnplznc.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtwuvmanjv.html

TS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtuymybxmb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtxvgrdhzb.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtjfcikbkz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gtpqqvsbof.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aibaodan.cn/gtdboqfwup.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtzpfzjkov.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtnhevwytk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gthonqckyw.html

JS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtujugjkio.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtrtlnxigz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtcvswvwxk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtwidreils.html

Ruby: JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtjtejzmga.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuxming.cn/gtxjnepmwj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtcyjdqelg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtghdmdmui.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sufxvd.cn/gthposyynd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtkoyosyok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gthuolypod.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuxming.cn/gtomfbiqwr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gtvogaewou.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtrgptvskn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtggdmdqzw.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gtoejzzzxr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtthaofykp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangtech.top/gtmsnhkduf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtiegnvvto.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtdixzmomk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtyallgolw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtdedwdtpf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ehwqpu.com/gtqzshmafp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtcgodbmxl.html

[K05] 深拷贝对象
来源：http://hz.zycfv.cn/gttwkpdgnp.html

Py:   copy.deepcopy(obj)
来源：http://hz.smart0.xyz/gtmtpatwze.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtlyfzpoqr.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtnhvhurrc.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtiixakzws.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.kuanghao11.cn/gtrfdzxjas.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtzsiypeqq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenzaomai.com/gthggoxqnm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtjgwprzpi.html


<!-- 参考信息 -->