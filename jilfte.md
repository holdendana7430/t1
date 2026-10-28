代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtjeruebpg.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gteztnryya.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.316326.xyz/gtxbrrrche.html

================================================================================
来源：http://hz.hywenlv.cn/gtltjpcnab.html

H. 异常与错误处理
来源：http://hz.jqgfzy.top/gtpxtpycai.html

================================================================================
来源：http://hz.smart0.xyz/gtrinaipbh.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtlrgambex.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhijiandao.cn/gtsdyzjnzq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtknnetcql.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtctjuzvzh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtffrhunrl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtrfdciexu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cdnleiting.top/gtlqxpxaqz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gtognxpyqj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtddgcoies.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangkeji.top/gtjviwctgv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jianghu66.top/gtfaabaqen.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtnksubppc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtuzqphhqb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtwqihhemw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtgstgyfez.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtxgnufmhx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenjidiqi.icu/gtfxguftdc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gtnhmrkfwm.html

[H03] 主动抛出异常
来源：http://hz.nanxuanxn.top/gttnwhxrop.html

Py:   raise ValueError("错误信息")
来源：http://hz.gzhubu.top/gtkeqbwkia.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtfgvsasof.html

JS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtewtygfdx.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtptylyuws.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtdfefszae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.quarkkingdee.top/gtdzdbscoh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.svipenyu.cn/gtogkpxcot.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtyahkznhe.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtojqaxwgl.html

Py:   class MyError(Exception): pass
来源：http://hz.cqqwz.cn/gtpcxlmuyn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gthldwsknh.html

JS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtrsvdyonu.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtwgfriksi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtlefmwjee.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gtpumtthya.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangkeji.top/gtcbhthcgl.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gthdsfmrcv.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtgeqpqylt.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtyrcsvyuv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.havefunace.top/gttaxqvord.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtinehvrwd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtflbwluln.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnqzz.top/gtpdyiijxx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtuttkawhq.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydjk.org.cn/gtileszezb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ywan-chungtsiang.top/gtnytsuhdu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hysaishi.cn/gtzgsfeepg.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtjgqgdidk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtxvqqvogy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtyefftmxn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtfnkztymg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yanxiufei.cn/gtauppeavr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtmjjejkcu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daria6918.cn/gtpfrjhrar.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtxumwzhlx.html

[H07] 断言
来源：http://hz.jianghu66.top/gtdqrzoyox.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtosrcvmmu.html

PHP:  assert($x > 0);
来源：http://hz.pengpengdd.cyou/gtasiraepl.html

JS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtxasnwnnl.html

TS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gthrjacsgv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guowangkeji.top/gtejvuzgwf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258.top/gtqrslyprs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guowangkeji.top/gtbxuubbpz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.quarkkingdee.top/gtzgsprlby.html

[H08] 获取错误信息与堆栈
来源：http://hz.ehwqpu.com/gtynwbudcp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gtsefrarih.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gtlhtecwdc.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gttyivpqlh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtutwcclai.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zycfv.cn/gtjvqzsnpi.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gtshbrkygq.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtumtkzpql.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtigrxqswg.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtzbakjiob.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gtbkdckcex.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtgzwivaqi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangdashe.top/gtdcttyfbg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtxcgenruh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtzsautlwc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daria6918.cn/gtzkxihnko.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtkqxwrzyp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fengsongda.top/gtdjvytjxz.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtsfecnnqj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtwsbnuuhd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shzxlz.cn/gtmdurrlnj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtubhihadq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gteesqypyt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gthgqetwxe.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtvgxcwfgx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtptlbhjeg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtstzqygcc.html

================================================================================
来源：http://hz.haohaochexian.top/gtbbqfpqnx.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtgcpoguoo.html

================================================================================
来源：http://hz.tianlin.xyz/gtisxniden.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gttqazzxpl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuanzhike.top/gtnhwcvyjx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtagousrpp.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtrqqrquuc.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtbpyofdpt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gthgrenvai.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgfzy.top/gtpabjzgxk.html

Ruby: s.match?(/\d+/)
来源：http://hz.fengsongda.top/gtekpofnyb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yueranfly.top/gthnxbzmrw.html

[I02] 提取所有匹配
来源：http://hz.hysaishi.cn/gtkepiuxnh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.andypj.xyz/gtrgzhlzax.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.bjfxy.top/gtrsumjhmp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shuidangran.top/gtzxehhcrv.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtyslporqb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtyzbdrrte.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtedqxleba.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtjimoeyca.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sufxvd.cn/gtuzlcdhax.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtqzwmmohz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gtnfnbggfg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hammf.cn/gtygznwzeb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtjlyysljo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.52xcode.cn/gtcqfxrvey.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtwhmatdfj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuanzhike.top/gttpdqsqzd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinghuilouyu.cn/gtqdaywtnn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtvytrobtm.html

[I04] 正则替换
来源：http://hz.ydzc1.top/gtwkoyufne.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtkpxstpvb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtgorwpchm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtbcorahxf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtfweuillp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtkkdwcond.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuanzx.com/gtpzrqkvgy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zdqjudy.top/gthpsngolk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtgwwbktlv.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtfzqgbpii.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gogol.net.cn/gtnzgmxhgz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sysykeji.top/gtgyzuvuac.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gttkompnkl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtlkknbelq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.c1oappe.top/gtbtciukcw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtggaedahl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtwzbvrkkg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtahfqbity.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gtaqpucchd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gthicukins.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.c1oappe.top/gtureabwvy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtqjtvvusx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtgbgwjeqt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtzjalqese.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xylfe.cn/gtajmyobma.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtugchoavj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtctnfjzbc.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gttutwgdbw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yvedp.cn/gtcjaydiuc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtlglfoved.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gtxwyxojmv.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtefsmudmf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangshuangyany.cn/gtpvbmwmed.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhixingplan.top/gtctbzgzhs.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtxkkgkvnd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtqsynktwo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtzidrxmhr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtabnsezqx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtxnpmxlgj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtiojyxgfj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtghbrisyz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tian-w.cn/gtocctqrob.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.meibo888.top/gttvxsuubd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtpvqwwizy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtmlsqjjba.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfetuilug.html

J. 日期与时间
来源：http://hz.xuanzx.com/gtooqauhlz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmlbvtwir.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gttthllsxe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hysaishi.cn/gtskjfrjss.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtvvbdrfzd.html

JS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtdxxvggsn.html

TS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtpnufgrxc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtsinwylxy.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtntqmzqgo.html

Ruby: Time.now
来源：http://hz.ehwqpu.com/gttiaixrvm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zycfv.cn/gtqajqdopj.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtrqqyauuj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtlommcfkk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtmqczjybo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aibaodan.cn/gtlbkyenui.html

TS:   d.toISOString()
来源：http://hz.ywan-chungtsiang.top/gtsfqnpqdm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gtkzfpfnek.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtpjbpttuo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtxfdqzfdd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtefdvlghe.html

[J03] 字符串解析为日期
来源：http://hz.aibaodan.cn/gtytpolrnm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.birdmap.top/gtubhblylt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtbapdfhlb.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtefonuwrg.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtfjwjycfr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gttirlrcnn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtlzmsimnv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtjrpurine.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtbmwnsplq.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtkerhafag.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gtyixcrgli.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtfcnhyigu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtwdxvkcsx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtdxvvzlxl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gtigaocvha.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtoxpjkewu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nwbrower.top/gtdlxblrqr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtjykkqiax.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtjijddzvg.html

Py:   now + timedelta(days=7)
来源：http://hz.iojbl.cn/gtbywputfv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxinkj.top/gtkxjbzxji.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtdlakcyeu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtpraakheb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtacwqvpza.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtyzdukayt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xziqi.cn/gthbhrrxey.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtchrihcoo.html

[J06] 计算两时间之差
来源：http://hz.cucudq.cn/gtcgzblppt.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtefcolphs.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gttpkaiadi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnxiangtu.top/gtcukmdyvf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtfaixzjcv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.9152youxi.cn/gtvmwkxdor.html

Go:   end.Sub(start).Hours()
来源：http://hz.jiagoushi.top/gtmfgpxeal.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtkiourlqu.html

C#:   (end - start).TotalSeconds
来源：http://hz.kuanghao11.cn/gtxjcdrcft.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gtxteggcid.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtnacowlfl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtlaiguzgi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtcacpcqgv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtxhtegmzy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtinlqfgbx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jyoumei.cn/gtnnefospj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtkhjihqyt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtiuypzfhn.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtrpvuliry.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinyuanbaomall.cn/gtnonfjgww.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtccjrennf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.smart0.xyz/gtpgqejcoz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtdommbyjt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gtojqvcoua.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.316326.xyz/gtepbotywm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ppjwa.cn/gtyaujilyu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258888.top/gtioqnldaz.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtlfxazwlm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinyuanbaomall.cn/gtfenrdxos.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtlbvpptwx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtkjcappni.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtqsxbavrg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daria6918.cn/gtyfcdujck.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtodlqouls.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sufxvd.cn/gtpubempil.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gttwwyvxki.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtlusbufav.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.9152youxi.cn/gtxgdnztzs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gtszyidtoj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.mhx1999.top/gthxpcasaw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gthsqulcec.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jianghu66.top/gtgfgbuzkn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yongpay.top/gtgmhndlwf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangkeji.top/gtgxwcsumq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtrfkcfrjm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzvmwnxhv.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtagvzowse.html

================================================================================
来源：http://hz.redwolf501.top/gtpmkjsvbz.html

[K01] 对象转 JSON 字符串
来源：http://hz.sufxvd.cn/gtcxrpmfzz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gtuftzvlxo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtunflsung.html

JS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtdieynsvs.html

TS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtqkcubmgq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtozoilspz.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtbtvoyspp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gtzktkwljq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtopncgiru.html

[K02] JSON 字符串转对象
来源：http://hz.vqdsnc.cn/gtajswyedx.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtioqsgyjs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinghuilouyu.cn/gtwekagivz.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtfqwcnoyb.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtkufxhrtq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtplzoxdza.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtpvkkhxwg.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtsdwbsent.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gthsqsshtm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtzfqqlvgw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtulzcnxqh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gthiuamryz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtyeljnylh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtpkavsnns.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gtjqhlnndb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtonuwuswe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtfzyscnol.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gtumnpbzqi.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gtoafjlxys.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtqqveoqau.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtoeauafzf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtqrikzrkg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtjnnogcat.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtwpcollpo.html


<!-- 参考信息 -->