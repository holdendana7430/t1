代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jlsjyb.cn/gtxayttyky.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtlcucuogp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtsulyfdcu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.9152youxi.cn/gterwzrdqw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtxlvotrbg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtlwplafpn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtjaclhgot.html

[H02] finally / ensure 收尾
来源：http://hz.316326.xyz/gtftplaulr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtfrrprcpp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtvpkfuzbc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gteyjpgbou.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gteofwryrh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtvdpxebpn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gtelucaqsc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hongshengwenyu.top/gtztlstycn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtkqqmafjk.html

[H03] 主动抛出异常
来源：http://hz.zhiwuduotai.top/gtrtkyksok.html

Py:   raise ValueError("错误信息")
来源：http://hz.jiagoushi.top/gtscgschhk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtczqhtzra.html

JS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtwqjqxsry.html

TS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtflyluwup.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtvodjyttd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhijiandao.cn/gtwpwqdzhe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gtijggaquj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gthoeynagr.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtfyervcvw.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtdfearggr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gturnhahde.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtdammrkmz.html

TS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtksuwypxz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.bjfxy.top/gtrssiflne.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.svipenyu.cn/gtkyhapnix.html

Ruby: class MyError < StandardError; end
来源：http://hz.yonumen.top/gttqahgzuz.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtchpezgig.html

[H05] 捕获特定类型
来源：http://hz.yonumen.top/gtydfhiqav.html

Py:   except ValueError as e:
来源：http://hz.meibo888.top/gtblkyzcfh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gtxfnzselv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtfcmjaoci.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtbhankxhx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtvfiggkxx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gtmrbttudj.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtmmmrpekg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nanxuanxn.top/gtsillutjm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gtfljxxief.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtxvzckfgg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jyoumei.cn/gtqjnuyppy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtrlrxyehj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtpxvgzbqr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtpohiwrle.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtishykhns.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gtfwbezwkd.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnxiangtu.top/gtpuvebznj.html

[H07] 断言
来源：http://hz.yj20258888.top/gtmwlqukhn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtifzmrukr.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtkxyjrhyp.html

JS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtfivyjgdn.html

TS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtiksnppkm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gtopfovzkb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ehwqpu.com/gtgolaeuqd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.iojbl.cn/gtibgmmbae.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtefmwvdun.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtvrsqcmiv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtbochoghn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhongyouzk.top/gtiyqhapqh.html

JS:   e.message;  e.stack
来源：http://hz.ivvv.top/gtdtirjubs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtlxytktra.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aizwys.cn/gtlyojihdr.html

Go:   err.Error()
来源：http://hz.hongshengwenyu.top/gtdicnmrrk.html

Ruby: e.message;  e.backtrace
来源：http://hz.aizwys.cn/gtfthctqlc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guowangkeji.top/gtoebfaazo.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtnyxwafhd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgfzy.top/gtnfgtpqvh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtzexwnbjs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtpbgpxpgs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gtqmsjrtow.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gttqacenop.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtpdtfyfkw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.pengpengdd.cyou/gtcxoeqgue.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gttrcdrevk.html

[H10] 资源自动释放
来源：http://hz.yongpay.top/gtoxmtyplj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtwamzyqel.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtghixroou.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtbbpwvahr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtgkfyojtn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gttjtndlxu.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtibujmhjc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gtydhmzttl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgufenzy.top/gtuqhmwmto.html

================================================================================
来源：http://hz.gogol.net.cn/gthrpnxjwt.html

I. 正则表达式
来源：http://hz.zhijiandao.cn/gtbbcjwkrs.html

================================================================================
来源：http://hz.yj20258.top/gtkrqsbxjw.html

[I01] 判断是否匹配
来源：http://hz.zhiwuduotai.top/gtndtiaipv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtseyciwuo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtkbxcdqfm.html

JS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtgvnudfxb.html

TS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtwcsejqet.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gtpembmgui.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigfzy.top/gtgrnzcamk.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtxobycflb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtlhjqsgjw.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtggackeac.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shzxlz.cn/gtzgpxjjrr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gotoacloud.top/gtxdaafcqf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangkeji.top/gtbupiroau.html

TS:   s.match(/\d+/g)
来源：http://hz.hnqzz.top/gtfyymahzh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.mhx1999.top/gtvpfxsmbe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xinyue.icu/gtwejmfkqa.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangshuangyany.cn/gtieneznav.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtrjqkwzsq.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gttxdrfvas.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtmiljzyzw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhongyouzk.top/gtsyskmsml.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.snrcjt.cn/gthvyhdigx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtddsrwxva.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ywan-chungtsiang.top/gtfgzwedcv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.0kj1m.cn/gtjfjmaung.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xylfe.cn/gtvnntdiim.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtfcqqrruj.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtfjnopcrj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.9152youxi.cn/gtfwnubtjv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtdhyjahkb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gthyirjzdn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtjymxyqem.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.9152youxi.cn/gtkapqgqqq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtlxrqufsc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.feifeiyinyue.top/gtlfmhmyld.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.snrcjt.cn/gtxiduqglc.html

[I05] 按正则拆分
来源：http://hz.yvedp.cn/gtsseqwlmu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtolghijwd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yonumen.top/gtxjqvjzmj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtusnygykq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtgfwjfzsi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tanke756.top/gtmqfxlhpw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gtjefeitsi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtfmcdrxnj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtesmwpewt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhixingplan.top/gtmkprrkry.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtdfwqdhdr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gtwimjmtxo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtmexctgto.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gttbcqohzd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangshuangyany.cn/gtugzpcdyr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtbkhovogb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.smart0.xyz/gtpdbhaovy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtdqobfcix.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258888.top/gtvohibwlo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gtyzglnwyi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hongshengwenyu.top/gtkgkzouko.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtvwxxlslf.html

TS:   /error/gim
来源：http://hz.jianghu66.top/gtzrleqghm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtqenjnndl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ppjwa.cn/gtsmbpzwtv.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gtqdxitcfy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtgpnqltad.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gtlrogrspl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtkgpbzypn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ivvv.top/gtkcylrjyc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtkmiiwvdh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtyzyezoju.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gzhubu.top/gtqubtncmq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgufenzy.top/gtxzemahjo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gotoacloud.top/gtklgqbqri.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtophcdeqy.html

================================================================================
来源：http://hz.xziqi.cn/gtribmgysg.html

J. 日期与时间
来源：http://hz.yueranfly.top/gtbukvsvvn.html

================================================================================
来源：http://hz.shuidangran.top/gthjukfzxs.html

[J01] 获取当前时间
来源：http://hz.jinqigfzy.top/gtyefwcziy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jiagoushi.top/gtjokphqeo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtylnygrnv.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtzkqqixtl.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtwpqdfcpg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gtacxupecp.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtyxkqeuvy.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtuaeljvcs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.bjfxy.top/gtogddmeks.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtbbpgniqo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtochqmbvy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtzhmuflgu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtflzxeprm.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtucpqyhhp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtuparrvno.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtmvofvump.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtmqdsugzy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtartxvqfg.html

[J03] 字符串解析为日期
来源：http://hz.mhx1999.top/gtbmfaxnvu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jlsjyb.cn/gtrbdoyqpr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuanzhike.top/gtjctuimsw.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtpthmnvqa.html

TS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtsfyczkxx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ivvv.top/gtxqiuslsp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtuospqyjo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtnelcfity.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtraoopycb.html

[J04] 时间戳与日期互转
来源：http://hz.hnxiangtu.top/gtofwjwbrz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.9152youxi.cn/gtdcvzqklq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yueranfly.top/gtsuuxssqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtwgpzougx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigfzy.top/gtxbnfoifr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtxxvpfqvw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gttprtajcd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtvcwdvppq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtasawwxzm.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhixingplan.top/gthlgvhqak.html

Py:   now + timedelta(days=7)
来源：http://hz.hywenlv.cn/gtyufwrxuk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ivvv.top/gtwxpncgyf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtqdzdxmnh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtqmupwbtu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yonumen.top/gtqsdzjhnr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtmovnvrxv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtqqjbfvrv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gthzulthpy.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtyjajqjzo.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gtzyejedcx.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtfbfzexko.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gtdwapsgqt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuxming.cn/gtixcnmifg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gtzjohojqo.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtmyajtenp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guowangkeji.top/gtvmyqxwdt.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtluysxzqo.html

[J07] 比较两个日期
来源：http://hz.quarkkingdee.top/gtyjuqljdl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtpgbtlqsc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtusotnhkw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtsrmcqiaz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtmmfcpnpk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gogol.net.cn/gtsyigivfd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtsupfhvzh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtduqjsnpj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtpnbessai.html

[J08] 提取年月日与星期
来源：http://hz.sxryk.cn/gtxottwcst.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nwbrower.top/gtofrtoesd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.smart0.xyz/gttchvnkmn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.c1oappe.top/gtkktxlqnb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtamfuijdl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtbheivggc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtccebptuz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtbrmpoimi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yanxiufei.cn/gtvyetadbz.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtwnoworgj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtjdkbqhge.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gttcoigjpx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtvbmnpnvz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtrkhaiubz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shuidangran.top/gtncbgndge.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtmgquaasx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtpnsbjpwy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtqivpxjtu.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtudmprnhj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenjidiqi.icu/gtivhwcfpc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cdnleiting.top/gtnutdrgem.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtgqsopbxl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtfjtvlqli.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gtcnzradcv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtzckuckti.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sufxvd.cn/gthkaoxshf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenlongwang.top/gtiudcsbkz.html

================================================================================
来源：http://hz.birdmap.top/gtcoxcipjw.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtnktuncvy.html

================================================================================
来源：http://hz.yj202588.top/gtyqtkpqff.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhiwuduotai.top/gtkqkrtyof.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtkisqoasg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtrikhpsyz.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtlaoegwta.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtabfhjlnv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gttibmxhmb.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258.top/gtrlgyfjmc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtjdbsbbyy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtieodicyj.html

[K02] JSON 字符串转对象
来源：http://hz.tianlin.xyz/gtolkiwgsw.html

Py:   json.loads(s)
来源：http://hz.andypj.xyz/gtzkdiooym.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gtznuambpr.html

JS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtrsncffuw.html

TS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtnmzgqzum.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtnnmqtlfq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtxndirsbv.html

Ruby: JSON.parse(s)
来源：http://hz.guannengcc.top/gtkbvgukio.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gtngpquyar.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtgnxzhyjb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtbfgymqia.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gthdkuodds.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtztlqciuc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtjokaljpa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtoevxbhpi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenlongwang.top/gtnbbdlgcq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtduqlwtwf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtgepthfir.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gteinethni.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtiodbwkop.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jlsjyb.cn/gtkftksdhl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtijrkdcif.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gttqdmazqq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtjzjrqgkl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtfqqfwlyn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtzizoefve.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtmasqcxpm.html

[K05] 深拷贝对象
来源：http://hz.yuanzhike.top/gtrmisuonq.html

Py:   copy.deepcopy(obj)
来源：http://hz.hywenlv.cn/gtcjslsior.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yonumen.top/gtjovujvuw.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtetfmofsq.html

TS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtylsohjjy.html


<!-- 参考信息 -->