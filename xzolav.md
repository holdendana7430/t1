代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtcnuzvjzx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhoulong.xyz/gtmdethngn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aibaodan.cn/gtgnhwusuc.html

[H02] finally / ensure 收尾
来源：http://hz.yuxming.cn/gtewivihsh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gtfltrgosw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtjnlhqigw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtqxumofak.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtvrpgoajf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtzwcgfycr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtkjltyiru.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gthcdgrlsv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gtgqfzbdrc.html

[H03] 主动抛出异常
来源：http://hz.0kj1m.cn/gtfnxgtvsd.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gtzlzhhqui.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtqojpnxlc.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtytijnxof.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtmcokhyew.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtzgqdvviy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigufen.top/gtbqxpcgam.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.bjfxy.top/gtqjvmgsqu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtfrgngxot.html

[H04] 自定义异常类型
来源：http://hz.bjfxy.top/gttuynafkf.html

Py:   class MyError(Exception): pass
来源：http://hz.hysaishi.cn/gtvejjeqgo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtljlgqtxr.html

JS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtprsxsgtv.html

TS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gtxvqbvvmn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtqqjrovdi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtarmbptyg.html

Ruby: class MyError < StandardError; end
来源：http://hz.xylfe.cn/gtnllyphgk.html

C#:   class MyException : Exception {}
来源：http://hz.wangshuangyany.cn/gtzjfsmmhs.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtkwpqntnz.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtzwmjftgm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtmusndssf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtjlcdcdrr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtrrniqqhe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtmlacbovj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtugaadhxv.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gtnbrusbxv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.birdmap.top/gtyqszrtut.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yueranfly.top/gtdezllagr.html

Py:   value = d.get("k") or default
来源：http://hz.haohaochexian.top/gtcoznhkea.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.vqdsnc.cn/gtfngsfbhx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtukvljjac.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtmtfeknff.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuanzx.com/gtfdcgrlpm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhaomingkeji.xyz/gtwyydmiyo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtqnmvlxdo.html

C#:   obj?.A?.B ?? default
来源：http://hz.shuidangran.top/gtcpqdndzi.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtzyfqqjbw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.316326.xyz/gtxduhcthv.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gttvczqthu.html

JS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gttrnknleq.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtrijteupe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangshuangyany.cn/gtluhckprn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtzszsqnnn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtpilrjbgr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.9152youxi.cn/gttnzadxuj.html

[H08] 获取错误信息与堆栈
来源：http://hz.xylfe.cn/gtocozknon.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ivvv.top/gtuiztzomn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtkcvokapf.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtpjumcyaf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtevdfzrka.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtresgcaqq.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtqvsrroyi.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtfacrdsjv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtbqdbsuzs.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtanlbqamh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hywenlv.cn/gtiebmlawh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.kuanghao11.cn/gtgkmuzeab.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gtuvbqxlyp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gtxdieesez.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinghuilouyu.cn/gtqpjufleg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yangfankeji.com/gtesiuigec.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ehwqpu.com/gtkfpmdwyp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gtplyvguih.html

[H10] 资源自动释放
来源：http://hz.aibaodan.cn/gtyhgwkjsl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gteuioqzek.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtcoqudgkk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtnawwgimk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtrhomqqaj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jiagoushi.top/gtfnqzbpay.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtpexabsmw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cqqwz.cn/gtonlssgvv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gtvdlpwbsn.html

================================================================================
来源：http://hz.xuanzx.com/gtzefghozb.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtqsnfwubt.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvnmkwjiu.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtopctlkkx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtzdyuqjaa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gttenvfwlq.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtxtzbyeys.html

TS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gttjykizse.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gttjiwmqqp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtpjfhazms.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gthcdalgib.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gtwbgfuili.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtkmggzjqp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.andypj.xyz/gtosptfvnq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gtsiiexjdi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnqzz.top/gtdlmdlfzs.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtgaeuakek.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhixingplan.top/gtxpmopyfz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.haohaochexian.top/gtdidxbzgn.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtttazvsjz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtnstoacmt.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtvcmrzkdx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtqicrigzw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gtjdlrdlym.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.smart0.xyz/gtgbknnmlb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtqatkkbfc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.vqdsnc.cn/gtikboeybs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtgxbyrije.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gtsxejvrfh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hongshengwenyu.top/gtumwjefcn.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtedgdwzyp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xylfe.cn/gtejxtzrlz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xylfe.cn/gtlcymhwku.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gttrmeaaha.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtvonuyitv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtpvqnwgzp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtitcwkdae.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fzhhl.top/gtayqaqynz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gthgcbfkzk.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtkiydrnuw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daria6918.cn/gtozmhjjbl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtebsogljq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtggclgwsr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtrogtkbms.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtvbpeqdip.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtsrqfnzgv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtjhxjyglk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gttjlxpcxr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.snrcjt.cn/gtcaulduus.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtdtnslkgm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hammf.cn/gtnaceuajc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtjnxahayc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtvjarbcxt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.meibo888.top/gttaqccylj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tanke756.top/gtgkwjxbti.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtzudjopqj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gthoeglbah.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gteihorbiz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtjefidycs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtyrjvwhcv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shzxlz.cn/gtpevnkrxi.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtghiftfco.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxinkj.top/gtkqhawrgf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gthdciokjl.html

Ruby: s.scan(/error/i)
来源：http://hz.havefunace.top/gtwslnuxzb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.andypj.xyz/gtkgsykevm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jlsjyb.cn/gtfutkmjbn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtvunawswx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtlxhjcvbc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtpuixpjxa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtbucamtcx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.redwolf501.top/gtpdhyjrsq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtmiqwzuym.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.bjfxy.top/gtymfpkelc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtgvijhrhv.html

================================================================================
来源：http://hz.bjfxy.top/gtkjjrtqdm.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtreadxplr.html

================================================================================
来源：http://hz.pycfn.com/gtpaefwwda.html

[J01] 获取当前时间
来源：http://hz.sysykeji.top/gtemnyuhdi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtezozgzpa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtrcamrrja.html

JS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtharspbvu.html

TS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtfrjekegp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtluyknxcu.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gttrcpvdwm.html

Ruby: Time.now
来源：http://hz.zycfv.cn/gtvghrzmib.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtyhckwgqt.html

[J02] 格式化输出
来源：http://hz.0kj1m.cn/gtrbalrqym.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtqymqbxrj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtapybzecl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.kuanghao11.cn/gtxueyyckh.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtbcykseyi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtioidjejz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258888.top/gtvqsfpjep.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gttgyncltf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtdabkqcsp.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtjgggzott.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.andypj.xyz/gtpksvdcdq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.wangdashe.top/gttevnxnhx.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtzumkitym.html

TS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtskgwuocy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ivvv.top/gtzaaxbvmt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenlongwang.top/gtqycmpuuh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtgritszqs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yonumen.top/gtnjiblfib.html

[J04] 时间戳与日期互转
来源：http://hz.birdmap.top/gttaixthzf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ehwqpu.com/gtuzqherdw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtlhvdpsrd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtghzdzmdj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenzaomai.com/gthsgaewmx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtyfjstuab.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gtoorcdoxk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daria6918.cn/gtmedhmxve.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj202588.top/gtzmaaynmo.html

[J05] 时间加减（加 7 天）
来源：http://hz.iojbl.cn/gtoryjfmyq.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtabhpkssn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtdluhaeqs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtbciqmbwt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtkzjmsrmm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtnlwbsihp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtczncmoir.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fzhhl.top/gtqtfcommz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gtvnvecqsg.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gtkgtahydq.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtvmactitm.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gthdzmjvqu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtwkewnvfd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtimtygkpr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gtspvufico.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtgwvsjpcy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gtuaipcjwt.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangshuangyany.cn/gtyrhqqzsy.html

[J07] 比较两个日期
来源：http://hz.nanxuanxn.top/gtbjihrkoq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtlteiqggj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.haohaochexian.top/gtvxwftiue.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtkmdzetwp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtvkqjfump.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gteokjqxci.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtudopcnkk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtichbsdio.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtoidmmrhz.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtcpvtckki.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtwveiywwf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtolgtteud.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtwvxoqtme.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtnjzchzqu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtbxzljxwz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aizwys.cn/gtcklvhnik.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fzhhl.top/gtegqcuomg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cdnleiting.top/gtadphkjbc.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gthcmksars.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shangyingyoupin.top/gtxtytlkko.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtfgofrcuq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtbybybwkb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gzhubu.top/gtwdpcgfdb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jlsjyb.cn/gtekzmfryf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ywan-chungtsiang.top/gtybrvvzvr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtrxhkafce.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtwqanhrle.html

[J10] 取今天 / 本月第一天
来源：http://hz.yonumen.top/gtehdfirxj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtxkcwlzjy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258888.top/gtevpetdiw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sysykeji.top/gtrtujbxsf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gttowkedln.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtbhxeiaox.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtirretrug.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtcmqttybe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangdashe.top/gtgldttntw.html

================================================================================
来源：http://hz.guannengcc.top/gtscuzcvkm.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtyudslyxx.html

================================================================================
来源：http://hz.aibaodan.cn/gtvuwbnhmt.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuxming.cn/gtriwvfdfy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtqqaifqlq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtcmxhcyri.html

JS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtlrkwkweq.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtkoikzivn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtcnkoysea.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtntjkzlnn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhijiandao.cn/gtevfqifgu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtjjdrkvxu.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gtymyqifyn.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtihgatuxe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtxfhxrcpc.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtlpebehml.html

TS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtsatctkxk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gtqkglxrvx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gteayitaxe.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtegyvbxgr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtxjsngqin.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtghxaaccv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtqnalyjlp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtoyuonahi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtpfkflcgm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtgxbbrvxc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtdouwbqzr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shangyingyoupin.top/gtbttgcifk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gttcixgknh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtxfodiztj.html

[K04] 读取 JSON 文件
来源：http://hz.yj202588.top/gtkmsutbro.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtfuivnnpg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gogol.net.cn/gtyoywzinl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtwitlrmak.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtmxpltafc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sufxvd.cn/gtohcpjkux.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtauplpdoj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tanke756.top/gtyfpzwisw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jlsjyb.cn/gtnrgddkrd.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gtkdbzcxgj.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangdashe.top/gtargkmomb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yangfankeji.com/gtohfpgoob.html

JS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtsigvyyhw.html

TS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtfdykhcsa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ivvv.top/gtxsfclury.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gttfybiucz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtasewwwxp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xziqi.cn/gtmfehfevr.html


<!-- 参考信息 -->