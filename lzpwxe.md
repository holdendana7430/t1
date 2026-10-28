代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtihqkufyj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtsqzawgkw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gtlxdbcmbf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gtazwireph.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.redwolf501.top/gtevbefvtn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtqxrhpkqx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.snrcjt.cn/gtcaohsvde.html

[H02] finally / ensure 收尾
来源：http://hz.vqdsnc.cn/gttoloifvj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gtwyxsohwo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gturforuvc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtfvemwiro.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtscjyqpli.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtkdzscbnj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtkyjwuhdq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtnydagsnd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258888.top/gtzgzebwdq.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gtmiwobiqb.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtbiutpmlu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gthimsngkc.html

JS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtznqlkxir.html

TS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtrsmgghvu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtwtixpcuw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtxronkehl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenlongwang.top/gtzigipqsf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtnfglxtlc.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtzsntrram.html

Py:   class MyError(Exception): pass
来源：http://hz.cheryme.top/gtehdipobs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtpkztdwom.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtvhdsxehe.html

TS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtdtkizbnm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtcjrklcwk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258.top/gtcgcdcnqa.html

Ruby: class MyError < StandardError; end
来源：http://hz.guowangkeji.top/gttzodccmp.html

C#:   class MyException : Exception {}
来源：http://hz.yangfankeji.com/gtdzfbvioa.html

[H05] 捕获特定类型
来源：http://hz.ivvv.top/gtniycegwn.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gticlhhwro.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtxmktlxfw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtvkgfngjk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gteusrgmoo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuanzx.com/gtedpxopuu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtzbzrursq.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gthrubaxna.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtctyhfmff.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hammf.cn/gtnaltvxxu.html

Py:   value = d.get("k") or default
来源：http://hz.haohaochexian.top/gtvlytface.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtzdicfciy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtdkgbsalf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtglvistov.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sweek.top/gtbfamrybh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtuszywbhs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtjaeyypoa.html

C#:   obj?.A?.B ?? default
来源：http://hz.nwbrower.top/gtcnjkoeyg.html

[H07] 断言
来源：http://hz.tian-w.cn/gtbzonjdqe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhixingplan.top/gtgosgmifp.html

PHP:  assert($x > 0);
来源：http://hz.chenzaomai.com/gtqpxwfaig.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtqhlidqok.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gttgisgicb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xylfe.cn/gtznxyolgq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtskbiufhh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.52xcode.cn/gtayncuptx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtjnlzywvq.html

[H08] 获取错误信息与堆栈
来源：http://hz.svipenyu.cn/gtcyxnudij.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yueranfly.top/gtervxqlob.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gaohongyu789.top/gtmyerhpje.html

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtivxceujm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtnqsplboe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigufen.top/gtrdcaugmp.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtcqgqbfzq.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gteuuvahpv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangdashe.top/gtkkwpgqti.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtrnvwboce.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtmmvervro.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtfvsxeoye.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtaqiesvyd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.vqdsnc.cn/gthvkayyif.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.iojbl.cn/gtbkpronvt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gtwqcwsirm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gtitrjmdmj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuetiantiany.cn/gtkjdgaxaw.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtmrwibltl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtmnjikakx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yonumen.top/gtzqebplzc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gteapzmdbq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtjrlyhyog.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtzkrmgyld.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gthrqcmcai.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydzc1.top/gtkkbcpdes.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gthntyrbpw.html

================================================================================
来源：http://hz.fengsongda.top/gtqvgyezmz.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtmrjdhfsf.html

================================================================================
来源：http://hz.andypj.xyz/gthexvlgds.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtozgnklkf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtfosthqha.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gtuaezpead.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gttftjsodq.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtgsyjkaok.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nwbrower.top/gttyjophls.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gotoacloud.top/gtaownvbrx.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtetmzqrwd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtjlqopjke.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtupwgrkwz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.0kj1m.cn/gtovxvmjyg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtzlsbibmj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigufen.top/gtiomiyryg.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gtqwqnwxzi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgufenzy.top/gtclixfynw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gtonicrrtw.html

Ruby: s.scan(/\d+/)
来源：http://hz.cucudq.cn/gtfvexypws.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtnyxcmypw.html

[I03] 提取捕获分组
来源：http://hz.meibo888.top/gtpxgxeooe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yongpay.top/gtinliuzgo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.vqdsnc.cn/gtddiyufag.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xylfe.cn/gtdxhsiwge.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenlongwang.top/gtqgojqsyv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yonumen.top/gtniccxrza.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gttljfnkje.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ywan-chungtsiang.top/gtrguiqrzz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gtyctufmvd.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gtbqzbgdop.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtwzzfysit.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtrgpanzeb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtuyjjtkwt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sysykeji.top/gtwzsujwpe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtfqponaqr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtyhujdmql.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pengpengdd.cyou/gtzaadpapn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daxiang520.top/gtxmsymlge.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gtluediiss.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gtpydqybdn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtqxesjwry.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtifbhhaek.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtevhahdxi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtkfmbnqwl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.andypj.xyz/gtytepabmp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtqrhquwvf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuxming.cn/gtnwinmubi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhiwuduotai.top/gtpjqhkwzd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gttescnanb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gticmmnlrj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtyjdcrtpg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtkhjasvab.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtglzllzyf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuanzhike.top/gtdgufymeh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gthscxgkdp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtmbyxmqhg.html

[I07] 忽略大小写与多行模式
来源：http://hz.ppjwa.cn/gtqdhngyix.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenlongwang.top/gteazncfpe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtemvgmagj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhiwuduotai.top/gtlrnprigx.html

TS:   /error/gim
来源：http://hz.zhixingplan.top/gtokdenmgz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daria6918.cn/gtvgierqvc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tianlin.xyz/gthqbpdqvr.html

Ruby: s.scan(/error/i)
来源：http://hz.snrcjt.cn/gteizqqsmf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhixingplan.top/gtbhpqxtim.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtbpmtmrrb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuanzx.com/gtbthounuk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gthldyaokt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtbdahacpp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtwbqzmnqy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtitbaxevy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gtyhrjdwxs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtoedrqrez.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtefajyzyp.html

================================================================================
来源：http://hz.yangfankeji.com/gtoyxmcyle.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gtdczucnwt.html

================================================================================
来源：http://hz.svipenyu.cn/gtddtkuiyu.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtasaxdrnn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.quarkkingdee.top/gtmuhmbmht.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gtpthczrxx.html

JS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gthtjvmcdg.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtajlcobzv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.havefunace.top/gtnxemoute.html

Go:   time.Now()
来源：http://hz.zhixingplan.top/gtisoixklu.html

Ruby: Time.now
来源：http://hz.tianlin.xyz/gtzrgjmpuw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtnsejhxnv.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtknzfsrzs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtpmxefqtv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gteeficjic.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.feifeiyinyue.top/gtfxgujbap.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtjmnfdjoq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gaohongyu789.top/gtooquxpoc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtnnlzgmfu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtlsqebqgs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.redwolf501.top/gtxqvrovya.html

[J03] 字符串解析为日期
来源：http://hz.yongpay.top/gtcayejliz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtojjyyygp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtxpcvcxgu.html

JS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtpusjaqvd.html

TS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtwfnaottj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtctkxhhlo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yvedp.cn/gtjsskbpkv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtefyoozzw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtxafpqlqv.html

[J04] 时间戳与日期互转
来源：http://hz.gotoacloud.top/gtoajqepda.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtmmexuogj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shangyingyoupin.top/gthzzfogaq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtivyidyry.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gaohongyu789.top/gteurpmgkj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gthzvuqctp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gtkwzerwfb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gtlgerezdk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtzczuzvny.html

[J05] 时间加减（加 7 天）
来源：http://hz.feifeiyinyue.top/gtlkxxsdcy.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtsuljncvz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnxiangtu.top/gtqezzhzpe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtnwcponeg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtvlplovnt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtqgebiqqj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gtrxcstsyn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtwobtjlui.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yonumen.top/gtmgcgykax.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtdofdhzhr.html

Py:   (end - start).total_seconds()
来源：http://hz.sweek.top/gtrsvrqphl.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtvhnvdmjj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtwdxnarof.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yonumen.top/gtaoiybsac.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtzvgovstw.html

Go:   end.Sub(start).Hours()
来源：http://hz.snrcjt.cn/gtsbhujwcb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtybkcbwdk.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gtpupesvqf.html

[J07] 比较两个日期
来源：http://hz.yj20258888.top/gtoynephrj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtsktsgsrd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj202588.top/gtoxucytms.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtyvtbqqru.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtpygpipjj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gthvmxmcav.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtfwlrjsoa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtplqoqmas.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtxvymswdz.html

[J08] 提取年月日与星期
来源：http://hz.daxiang520.top/gtqksihyup.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hammf.cn/gtowcvvzsm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangshuangyany.cn/gtfjtwhvuo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zdqjudy.top/gtlxyznvmu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtkuoenvkr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydzc1.top/gtinsaueqp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sysykeji.top/gtkyqpfrpz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sysykeji.top/gtygatqjkl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cashguo.top/gtkwkeidtt.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtzvmzrvbi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtytqdzrzo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nwbrower.top/gthcsemvnu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtcdqckfko.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtarllgzts.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtebeqwwoi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuxming.cn/gtabekiare.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jianghu66.top/gtvtrihivz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtrdkhvefa.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtjrcoxctl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhongyouzk.top/gtbldrvmvb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.birdmap.top/gtcxiwnixu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtsxcrdkpw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtashbzifn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sxryk.cn/gtmivwkgaz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gttiqytude.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.c1oappe.top/gtniqpzeqk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhiwuduotai.top/gtsihtdypu.html

================================================================================
来源：http://hz.yonumen.top/gtvkufroqp.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtzbvltjwf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdgmnmgsb.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtqogbcybs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtdnimdnrj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtvkzfsexc.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtismqmqni.html

TS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtcgvkbmtd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuetiantiany.cn/gtekmqypwe.html

Go:   json.Marshal(obj)
来源：http://hz.hywenlv.cn/gtafcxocjy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtwrkdyobs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gttxdfalrl.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtqgjeaxso.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtjfnrdpmp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtkznomqfx.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtjhmexyix.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtboegmohq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtivpbvvvg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtdqtytqfw.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtgvrulptp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtljgkpihb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yanxiufei.cn/gtkvwhdpte.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtcjlaivux.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtajdztwjg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtswaqbbdy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtbvfgwpez.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtkmibevbf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.0kj1m.cn/gtlbfhqldz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtgsnoyfdo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenlongwang.top/gtwixmjeaf.html

[K04] 读取 JSON 文件
来源：http://hz.yueranfly.top/gtawbmgmdr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtvcazzama.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtoioegnoz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtpwfdqqco.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtyuxvzglq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hammf.cn/gtpqbdfwjf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtzwgktxlz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtfmbamgxr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.bjfxy.top/gtxjbescuc.html

[K05] 深拷贝对象
来源：http://hz.hywenlv.cn/gtvqunjqga.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangshuangyany.cn/gtmaoogopm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtmmfojmsk.html

JS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtfmhfzkln.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtjkejidgm.html


<!-- 参考信息 -->