代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shzxlz.cn/gtpfhmaszn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtzmbnupzj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtwetfgmbf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jlsjyb.cn/gtofmraszl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hywenlv.cn/gtyxjjoyyr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gthdhejkef.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtvixrznaa.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtrxlzmqzc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgfzy.top/gtbdgizevx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtcquomrqt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtzrssmniz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtajxvtbyz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtjscedwum.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtdhagjpmz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cucudq.cn/gtlmwxegxw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtqxvfuxqp.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtjeywpcpd.html

Py:   raise ValueError("错误信息")
来源：http://hz.cdnleiting.top/gtbvufjrub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtuukuajpa.html

JS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtstbzgdlm.html

TS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtwberqodm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtmguzusju.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xinyue.icu/gtenpguyib.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtrhvacrhc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtmqtinlwt.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtrsfnswqx.html

Py:   class MyError(Exception): pass
来源：http://hz.birdmap.top/gtbzhgcznz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cucudq.cn/gtzygcbinc.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtpbojwrlx.html

TS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtfbrqghxq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtaeuejmck.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ivvv.top/gthlprxulh.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtyvioxkga.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtipysuqlo.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtpigacpik.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gtufnwderk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gttyuygkph.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtdbuegqio.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtgudufywa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtswzoawcg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yonumen.top/gtoymejrgp.html

Ruby: rescue ArgumentError => e
来源：http://hz.quarkkingdee.top/gtjxspizqx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtttuqgrml.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tian-w.cn/gtxyihfcqi.html

Py:   value = d.get("k") or default
来源：http://hz.smart0.xyz/gtirszypae.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtsyckbunh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gteghztihv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtfiqixfbt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtbbevmlvo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zdqjudy.top/gtqsrqkdeg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtjravzaus.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtlfkmwfta.html

[H07] 断言
来源：http://hz.jiagoushi.top/gttgosazol.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuetiantiany.cn/gtqczqjltx.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gtgawskjcc.html

JS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtghhrvwqz.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtzrnmwkbh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guowangkeji.top/gtjeltcyic.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenzaomai.com/gtgnkssaot.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258888.top/gtfkwjxbob.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtrfeucczy.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtspywbwtx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj202588.top/gtuwpoefyk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhoulong.xyz/gtgiofggdh.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gthggrusfj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgfzy.top/gtwanlxlso.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ybcxt.top/gtulgshxsg.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtodcuiyqh.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gtqrivczjj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtwrnojahj.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtvilrfgua.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fzhhl.top/gtjsntmflc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtttiabtoz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtbstihbpw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtabdtzbzq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tian-w.cn/gtfcgnxlsf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtggoqeqcq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtbgqmudme.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cashguo.top/gtnwcvtjyj.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtmmslecqg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigufen.top/gtgwleocpw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gtdwzvqgts.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtchvcccju.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtetcnsjos.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtwghnywhb.html

Go:   defer f.Close()
来源：http://hz.cucudq.cn/gtdykupmpu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.kuanghao11.cn/gtneciwhdn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jianghu66.top/gtrfxtbbhh.html

================================================================================
来源：http://hz.nwbrower.top/gtuqhgbrts.html

I. 正则表达式
来源：http://hz.tanke756.top/gtetwaawbu.html

================================================================================
来源：http://hz.havefunace.top/gtbavrzfxn.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtbnhcspfn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.andypj.xyz/gtgjiwzpnw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gtkfzagnhx.html

JS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtgjztxoor.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtfebzwbpw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.meibo888.top/gtjcsrgqub.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fengsongda.top/gtzqursafq.html

Ruby: s.match?(/\d+/)
来源：http://hz.jiagoushi.top/gtwlwfbgbb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtzkschffn.html

[I02] 提取所有匹配
来源：http://hz.zhoulong.xyz/gtwbqxisfl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.smart0.xyz/gtpxvgydyy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gttlhqgdfd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hongshengwenyu.top/gtzblodbql.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtgpkrtfxr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gtqfcignuc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gzhubu.top/gtanlybaix.html

Ruby: s.scan(/\d+/)
来源：http://hz.dianchejie.cn/gtupbytdcv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtqctkjpaq.html

[I03] 提取捕获分组
来源：http://hz.hysaishi.cn/gtlzrlpwxw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gotoacloud.top/gttqkpocak.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jiagoushi.top/gtfsmlando.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtomjqaoua.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtohmqivry.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtbueiytlj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xylfe.cn/gtpcjjxksv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtghzjllea.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hfpthk.cn/gtxcqezbhb.html

[I04] 正则替换
来源：http://hz.sxryk.cn/gtdcnbdnlh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtnpapaotl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gttqjioeaf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtkhroqpov.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtwhzvltak.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtgjrpsbxk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtvhvnyqdm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xylfe.cn/gtxtqvukvb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtxfdeatwb.html

[I05] 按正则拆分
来源：http://hz.nanxinkj.top/gtzlkksnpg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gtctflrfzp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtwbbcmnsr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtcafjcjru.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtwcquzgvc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtexizdepf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gtplyxglxv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtklbthhuy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtdiiryzrq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gtnpaxmgzv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtlbbeynno.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtzkdbaohs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtdbmdjmfp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtrijjtgxr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtrrvzgbow.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.andypj.xyz/gthzzttsxq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtabgkorjd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxuanxn.top/gtsvgxysrr.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtenubjkqv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gtxuftiszh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cashguo.top/gtgaeqzcjw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtbcswdauz.html

TS:   /error/gim
来源：http://hz.ppjwa.cn/gtaqzunexb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhaomingkeji.xyz/gtrcpyxmtz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenzaomai.com/gtalpyoymr.html

Ruby: s.scan(/error/i)
来源：http://hz.tanke756.top/gtndrxcddy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gtzsbjfjyb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gogol.net.cn/gttqeryqrd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinyuanbaomall.cn/gttcsrfspx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ybcxt.top/gtypuyvsrz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtpbqycdpj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtcoylyegx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtquvhubai.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtyilecyel.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gzhubu.top/gtzaswvule.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtivrcmwsh.html

================================================================================
来源：http://hz.tanke756.top/gttabazneo.html

J. 日期与时间
来源：http://hz.gotoacloud.top/gtjmyqcksw.html

================================================================================
来源：http://hz.tanke756.top/gtipbmidun.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtgwjnlmwf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtcmmhotbb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtmtccdivk.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtyedrglvu.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtojpzcrnz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtjxzjjwiu.html

Go:   time.Now()
来源：http://hz.yj20258.top/gtdmdqjgxr.html

Ruby: Time.now
来源：http://hz.c1oappe.top/gtrlensjim.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtdcxloars.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtumcppkyu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtsshlmgir.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtbidjmrmi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.haohaochexian.top/gtwxtqsika.html

TS:   d.toISOString()
来源：http://hz.nwbrower.top/gtqewzhkkv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.birdmap.top/gtpibvaddi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtczgkmjby.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtwydzvmnr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.fzhhl.top/gtnijxmwik.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangkeji.top/gtpwbdxyxv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtnyhqwman.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtxvymsido.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtjceanbpc.html

TS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtkxhupkls.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtizzjjpbb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenzaomai.com/gtllrokenx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtlcenxqpf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhongyouzk.top/gtjxdmxidw.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gtqidjxhoe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gthpjxflcd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daria6918.cn/gtxmzsrmxo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gttswxkxvq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.iojbl.cn/gtksqqhzbb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtxddbnfgn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtydhfjgfp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtkswoocuo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgufenzy.top/gtwcjrdapi.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtxpjjxohd.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtsibrfrhq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtygxchcgb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtcrzvvpvh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtlblirdpp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydjk.org.cn/gtqjklujdk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtyxfberzp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtbivmqdcb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtmsbdkcfx.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtszeygexf.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtvxttrpdq.html

PHP:  $end->diff($start)->days;
来源：http://hz.ywan-chungtsiang.top/gtzqarenqm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gttnxkrhsy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtgzaktcdx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhengqikj.top/gtfmdjwohb.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258.top/gtieijcyde.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtkdtoxjef.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtptncyhsy.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtbczrdiib.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtvpundqst.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtheykvnvq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtbkubgndb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtvttlsbau.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ywan-chungtsiang.top/gteztxybqe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ybcxt.top/gtszyzskca.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtkteoxykx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtjkgbdmzs.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtlyraemlg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jianghu66.top/gtvxfqmkxl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtgodqozwz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtfxkiovze.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhongyouzk.top/gtdjrnvukj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtqcjsbyay.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinghuilouyu.cn/gtchvuohcp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jianghu66.top/gtqbwmrytm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydzc1.top/gtqssgmwci.html

[J09] 时区处理
来源：http://hz.jiagoushi.top/gtxtbpeozp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aibaodan.cn/gticxgbgye.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtzfwntlno.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtscgoapnt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtferszzau.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtzqzqxxom.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtdqhqzwns.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtktgvlgcq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gttqcjthcu.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtyqqqosxp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtpxrxyvul.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtfgahmzqi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtcmhwschd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtqdklgmlo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtmnyqmmri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtvzoujbmm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aibaodan.cn/gtkxhgiich.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtipkdtvnx.html

================================================================================
来源：http://hz.zhixingplan.top/gthoasuyih.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtsebxhlrn.html

================================================================================
来源：http://hz.hfpthk.cn/gtqonvooyh.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtnueromnf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gthnshzxvg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtilrouizr.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtxpjkwiaz.html

TS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtehfkirhf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ybcxt.top/gtynitabxt.html

Go:   json.Marshal(obj)
来源：http://hz.smart0.xyz/gtlatokxeg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtpdvtlama.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtcmqfutkm.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtlatzkwhg.html

Py:   json.loads(s)
来源：http://hz.aizwys.cn/gtdlsceuza.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtcevdjwwd.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtfymworwr.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gttruxhaab.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtjcrcpomu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtvvdqzsll.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtgwloatjn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangdashe.top/gtairyozci.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shzxlz.cn/gtpqwssqnd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtbvdmvxly.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gttyxupzvo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtheclcflr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtzvsqstrd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuxming.cn/gtifhsarih.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtwnwfufns.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenjidiqi.icu/gtugzgolau.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gtrewtfvng.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gthibllayn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtftzghyxa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gteiccshvs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtmjejsdzm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtpcxbxvbm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangshuangyany.cn/gtvqtnvbyi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtzcwiqpeg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtgdbwuwns.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxuanxn.top/gtztoucwwy.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gttjypojff.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gtvpjraksu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtlsnustnq.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtqnxihtvj.html

TS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtcnculzcq.html


<!-- 参考信息 -->