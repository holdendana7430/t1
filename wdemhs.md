代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cheryme.top/gtodschkpt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gttvuwfvuj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cheryme.top/gtdremkcgj.html

[H02] finally / ensure 收尾
来源：http://hz.chenjidiqi.icu/gtjaomervx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuxming.cn/gtyxwocdlc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gthgbasjdr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtkmtskbpb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtshwqmibg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtcdfajicg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gttgielnev.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuetiantiany.cn/gtkhyxoafu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtdqjlkogs.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gtgaduwkqd.html

Py:   raise ValueError("错误信息")
来源：http://hz.iojbl.cn/gtxetjshrj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtxggdvozv.html

JS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gthjzgstap.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtgwwsztna.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtpcudfszv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtpebshhnv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtanrcgpit.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtvtatmckl.html

[H04] 自定义异常类型
来源：http://hz.wangdashe.top/gtqdlkortz.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtxadogxzu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtzffeamnn.html

JS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtggbccmqa.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtjygfpmde.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtcrijnjbj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtfygqdwvh.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gtjclsyrxz.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtsoqpjvkb.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtfoajjmkk.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gteiuggmsk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtbcutjugm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtckbsgmge.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtgqzysokg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guannengcc.top/gtupinhwwx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgfzy.top/gtclrmxcuo.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhongyouzk.top/gtiluzciel.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zycfv.cn/gtttnsehwf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuanzhike.top/gtyvyybemy.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtsmvsassl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shuidangran.top/gthsautodi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtcvacirxz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtuhlbthoj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.andypj.xyz/gtuyczbcco.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tianlin.xyz/gtmkjqzefb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gtcpsvnydr.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhixingplan.top/gtwawueccg.html

[H07] 断言
来源：http://hz.yvedp.cn/gttgalqkbd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenjidiqi.icu/gthumrbxtf.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtvhyyilgy.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtqtsvjgkd.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtwrgxlben.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtkjllrqep.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jlsjyb.cn/gtqxmpzvto.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtpxkdjpmg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gtfrqqapip.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtzkpnizez.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gttrdasqat.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pycfn.com/gtyvbyncbf.html

JS:   e.message;  e.stack
来源：http://hz.havefunace.top/gtuluxjrcb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtlctvavrh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtmzjbtiav.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtyrksyapt.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtdmarqhak.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gtlxlmyvhx.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtbovgzmmk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gthmruvgcv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtznxghhzd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.316326.xyz/gtyezskmxr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gtlxrzxcqq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gteykozmfk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daxiang520.top/gtltorraxw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tian-w.cn/gtqmrymhge.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dashuyun.cn/gtneotiqnl.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtwrjwljpu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtzbkhfqqo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gttuorwycw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtxzyrbrfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtjamwwymo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.mhx1999.top/gtddadrpvb.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtmebjazug.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnxiangtu.top/gtcjczqqub.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtbiubjswx.html

================================================================================
来源：http://hz.zycfv.cn/gtlopvmlfb.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtryvqcuvo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmxnriskn.html

[I01] 判断是否匹配
来源：http://hz.andypj.xyz/gtcmrtxbco.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtxueuhdoe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtcnjrbkny.html

JS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtkenqtbku.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtacvbqhtq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sxryk.cn/gtquyvwtnc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxinkj.top/gtmeiszrdg.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtprfdxxby.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtdlwvqxug.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtaipojqha.html

Py:   re.findall(r"\d+", s)
来源：http://hz.andypj.xyz/gtmvajvjke.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shzxlz.cn/gtwycguigo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gtmxhidcrc.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxuanxn.top/gtzngtwpko.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtqxcbfaxd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jlsjyb.cn/gtkxloqbwo.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtqezruxwd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gtzcyccwvd.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtbsqxjkxm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.0kj1m.cn/gthuomkmut.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cucudq.cn/gtxbkeusdg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtxgontakl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gttbztmhcv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zycfv.cn/gtkdvjsnzw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtklujebhg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtvxveamxn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guowangkeji.top/gtjaimwhbo.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtvvtsbxkz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinghuilouyu.cn/gtnfmerdbz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtbjolmrjb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtluyufmzt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtdimqalcg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydzc1.top/gtdbcwaopw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtkgauudre.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtklcvflgf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jlsjyb.cn/gtpfuyzzwd.html

[I05] 按正则拆分
来源：http://hz.zhixingplan.top/gtqzmfhvne.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtyqkvjzmn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tanke756.top/gtvmzcilea.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtljpqrfxx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtswkfhqiz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtjxiveimi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtgsnfuvpj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtjyrirmes.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtxcuvwnjm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtzrgcrigw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtaupgifql.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gtaywzlvdw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtmxkoyosw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtqiklzksr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gtjtuvpbte.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gtrgikqojn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtqftpqppk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtzskumarj.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtrnrrfkcj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtqpcwenyd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtmxvqatij.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dashuyun.cn/gtwtrjmlya.html

TS:   /error/gim
来源：http://hz.pengpengdd.cyou/gtftskkvdj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj20258888.top/gtggpbuumz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtjszmprke.html

Ruby: s.scan(/error/i)
来源：http://hz.zycfv.cn/gtmmoegiqf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ivvv.top/gttnulgrkw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hywenlv.cn/gtoooobevd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.redwolf501.top/gtrjbewxyw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jiagoushi.top/gticwjtrki.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtdzpwxghm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtlsdvhzfz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gteemljbbf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtvurzgpkk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtvryafxax.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.iojbl.cn/gtcqlypybe.html

================================================================================
来源：http://hz.yuxming.cn/gtinuwgxzb.html

J. 日期与时间
来源：http://hz.guannengcc.top/gthzblrrlv.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqqjdahxu.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtrzblbcvb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtgrzcihgw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gthkjwxcup.html

JS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtwoozesyd.html

TS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtsatpqqch.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtpkrkvroe.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gtbafiwmcm.html

Ruby: Time.now
来源：http://hz.hfpthk.cn/gtinllgaet.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yonumen.top/gtrvgbzqvz.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtvjqojjsz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtsojeotvo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtcajwouex.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtmrxtvyyl.html

TS:   d.toISOString()
来源：http://hz.havefunace.top/gturnlnlth.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.smart0.xyz/gtrdxngyzm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtzkmgqykd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtqiwlhgdg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shzxlz.cn/gtkjpsgzzn.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtbaybmndj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtikzfxnte.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtvlihaojo.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtuclvydpz.html

TS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtiassypdh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtakvveuql.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gtdgcesetg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtjmzoazeo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtoypzyibi.html

[J04] 时间戳与日期互转
来源：http://hz.zhiwuduotai.top/gtmhtehzuv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ppjwa.cn/gtanizomxd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gthkqgfqso.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtgjaeepfj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigufen.top/gtzzqsindx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ywan-chungtsiang.top/gteffxibte.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydjk.org.cn/gtrkxzkfyg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.snrcjt.cn/gtmbjnhtks.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydzc1.top/gtbndhyglf.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangtech.top/gtbexgpxnw.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtoboreqvk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xingfuxueyuan.xyz/gtxsenlzzm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtgzrekiyj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtnveovqfm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtgiiqskcj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtgxcdrthm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangdashe.top/gtcsstqvew.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gthqtgvzpj.html

[J06] 计算两时间之差
来源：http://hz.jqgufenzy.top/gtqbsivofp.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gttmnvyofz.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtdulnjxlb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtxbzuqbph.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtvhdvbmbk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtgankujns.html

Go:   end.Sub(start).Hours()
来源：http://hz.guowangkeji.top/gtntmucabt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxinkj.top/gtmyeysfyp.html

C#:   (end - start).TotalSeconds
来源：http://hz.shangyingyoupin.top/gtzmvylnpj.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gtvvmtthip.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtkofcfvmi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtmlkjkopx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtfgeeukys.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtarxoapwh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtmzezsrfq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtqgrtonei.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtzznroxyf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gttnkgibpx.html

[J08] 提取年月日与星期
来源：http://hz.xziqi.cn/gteoydiory.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nwbrower.top/gtultgrtjy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ehwqpu.com/gtbofhehth.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtlthkcabu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cucudq.cn/gtklxvtdxh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtkdeoyfrn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhengqikj.top/gtbnmruggz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtjxztkrah.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ehwqpu.com/gtpmjdbeyn.html

[J09] 时区处理
来源：http://hz.wangdashe.top/gtvogwipll.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtjvcriacz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gthsmkjool.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtrmznwiau.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtistmnuhe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.vqdsnc.cn/gtcvmpeoaw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tian-w.cn/gtqaasrnkc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.wangdashe.top/gtzunzxwww.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gttmbimyaw.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258.top/gtkbroqvgk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtitonekzq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yueranfly.top/gtkvcnpslv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.andypj.xyz/gtyurylspi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtaaodbkdx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sxryk.cn/gtgdlpdmgr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ywan-chungtsiang.top/gthnlkcxes.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yongpay.top/gtoyrvchwk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gthqvojhqq.html

================================================================================
来源：http://hz.mhx1999.top/gtlmqbkaac.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gtaeplanve.html

================================================================================
来源：http://hz.yj20258.top/gtsppeiqsm.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gthopsmoak.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtoakwxrbi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtjopjsics.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtpauayhxz.html

TS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gttebnyfdn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhongyouzk.top/gtsiuxkizd.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtglwkzeqd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ivvv.top/gtyfrmqhzh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258888.top/gtjifamlpe.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtiawtsrta.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtsfmxehps.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtmjyblsqs.html

JS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtrqvxrsoo.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtoorvaptc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtjrqodxwo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtnvmfyryt.html

Ruby: JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtlnftymvm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtsdpgwuiz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ehwqpu.com/gtpwyuyufj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtmjdlkkva.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtwmwqectr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtuwnjxosu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtyhuxvhrk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtawqkanib.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.guannengcc.top/gtjhvtjkbw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtoimkyqln.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtqqzcuxoc.html

[K04] 读取 JSON 文件
来源：http://hz.pycfn.com/gtilheofzb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jlsjyb.cn/gtsnecbqiv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtbwdlhcjn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtivhwccpt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtgozeoqno.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangshuangyany.cn/gtctelyhsj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtdddeexfe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtxsvtjohd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cheryme.top/gtkuqnhqzo.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtvexzqtrt.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtlitegilb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtxnhpkjuj.html

JS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtvewskzyi.html

TS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtfssjezbl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gthzvathas.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gtgvhjgaue.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtuybeckxh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xinyue.icu/gtexobbpqa.html


<!-- 参考信息 -->