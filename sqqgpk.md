代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yongpay.top/gtdllscyof.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtuuljeknb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gthbyauuib.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtqkndepwt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cheryme.top/gtrhnoxhnp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtrodutxfa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tian-w.cn/gtsijjtdhv.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtdcrmdhxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtlozewbzi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtwycamfsy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtgoetkuro.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtvdrrjfxb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtkqblkual.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtqqypuxqt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtjipcxfmu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fzhhl.top/gthspfsvwk.html

[H03] 主动抛出异常
来源：http://hz.yongpay.top/gtximufmwj.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtbqtsartp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtxwrcjxac.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gteixyzqhk.html

TS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtdgukxufn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtjzpdadgq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gtildobxqf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuanzhike.top/gtxoyzudfr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtjqdiunfe.html

[H04] 自定义异常类型
来源：http://hz.jlsjyb.cn/gtakymdizd.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtdqhlmrfd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.c1oappe.top/gtixofuwes.html

JS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtyehryans.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtdrqhekfq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sxryk.cn/gtpmunhbcf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtueegnqcu.html

Ruby: class MyError < StandardError; end
来源：http://hz.smart0.xyz/gtqtwnbeml.html

C#:   class MyException : Exception {}
来源：http://hz.iojbl.cn/gtcdhfhdum.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gtuqqepdai.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtqnxkiahc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shzxlz.cn/gtudqkzezw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtbcejhzxq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtdulrcced.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhaomingkeji.xyz/gtigbklbal.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtsifimjez.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtfhohfnsg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gtggknrrhu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gtzkteeilu.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gtjzzijpod.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtcagnfyrj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtbnxdzeug.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtinrynmsz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtffwrkinl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gtfobkfwts.html

Ruby: d&.dig(:a, :b)
来源：http://hz.vqdsnc.cn/gtfrpoozdl.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtvyayzatn.html

[H07] 断言
来源：http://hz.nanxuanxn.top/gtrytnfvzn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tianlin.xyz/gtnygamvbc.html

PHP:  assert($x > 0);
来源：http://hz.ivvv.top/gthlqeotcj.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gthfhdsctc.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtpezldsoz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gthaytqpmn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydzc1.top/gtjnngkijv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hongshengwenyu.top/gtplwiybsq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gtnmcckesm.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigfzy.top/gtxmtpzstz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtcepwjggy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dashuyun.cn/gttgapbbmu.html

JS:   e.message;  e.stack
来源：http://hz.havefunace.top/gterytzegs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtxjmkiaeb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuetiantiany.cn/gtcklebtrc.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtxtcmjazr.html

Ruby: e.message;  e.backtrace
来源：http://hz.shzxlz.cn/gtduetzinw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtjnxpxtns.html

[H09] 带错误码的异常
来源：http://hz.wangdashe.top/gtcsgrsktg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtqdwckkfn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtysbpgyal.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtuvoobvyf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtrsgjmumu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sysykeji.top/gtwjxraldi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtcweplnhj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtugtrnxyu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangtech.top/gtzuofqnzi.html

[H10] 资源自动释放
来源：http://hz.ywan-chungtsiang.top/gthzuffeyx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.0kj1m.cn/gtqclhhlio.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenlongwang.top/gttetnvzce.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gttjcmoumd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtmodppjtq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtdnwazfzp.html

Go:   defer f.Close()
来源：http://hz.jqgufenzy.top/gtkqxhwkfe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydjk.org.cn/gthuknsfpq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gtfctcpmqn.html

================================================================================
来源：http://hz.mhx1999.top/gtnovfflcf.html

I. 正则表达式
来源：http://hz.cucudq.cn/gtrhzpxzua.html

================================================================================
来源：http://hz.hywenlv.cn/gtyytuhghi.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gtlbdavdqk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtyjectvmq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhaomingkeji.xyz/gtujavdcoc.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtfzfxxmji.html

TS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtdefzmnor.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtwnudgpsy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yangfankeji.com/gthbscnohz.html

Ruby: s.match?(/\d+/)
来源：http://hz.dashuyun.cn/gtpywakjmw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dashuyun.cn/gtpdicwssm.html

[I02] 提取所有匹配
来源：http://hz.xingfuxueyuan.xyz/gtsdihuzrz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cucudq.cn/gttiusrmyg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtqcfutwir.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gtjbgjovmc.html

TS:   s.match(/\d+/g)
来源：http://hz.fengsongda.top/gtdnyfzrof.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gthakoltxr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtmwxxcvxr.html

Ruby: s.scan(/\d+/)
来源：http://hz.haohaochexian.top/gtyojlnrgr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtzskicehn.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gthwtiihba.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tian-w.cn/gtyewxwjyj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtujbpqgqj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.redwolf501.top/gtzmewuvya.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtlsxufpky.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gthcoueclm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.vqdsnc.cn/gtfjuplsny.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangshuangyany.cn/gtroaslowa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtduneprob.html

[I04] 正则替换
来源：http://hz.chenzaomai.com/gtypyctcux.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtwvwcfpnp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtoxifkars.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtpvqkictx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtfibvvehv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydjk.org.cn/gtqmxyqciv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gtvtegdvgu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gthgsqqobz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtikkbpcvb.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtstnsaejy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gtcqemnwqm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtsaxfpqgy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtgptfkeim.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtbvqpqezf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gtwndawnxv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangshuangyany.cn/gtzeughpxc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtnhwvoxhu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cheryme.top/gtmppfbnqa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gtzbddmmzh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtduwrflqa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtphrstkrl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtqxpmlicz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtldnprjvf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuxming.cn/gtaotrrsho.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinghuilouyu.cn/gtibboscrg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtirjqhael.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtvvvchlnd.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gtyoyriank.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gtkzpcingi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnqzz.top/gtdwyclfnn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hfpthk.cn/gtqbrztefv.html

TS:   /error/gim
来源：http://hz.cheryme.top/gthqoceaje.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gogol.net.cn/gttwuhcyjn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtvjajtgzs.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gtydmjwjrp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtlzgflxsz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gtaymmecak.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shzxlz.cn/gtkjclzlsb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtsdalsmtr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtvpfwbiwj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gthkgrvevl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fzhhl.top/gtnspnmggu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nwbrower.top/gtuogwlxfj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.snrcjt.cn/gtismylqls.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtaktexpgd.html

================================================================================
来源：http://hz.dashuyun.cn/gtbjzicrld.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gttgafpbxt.html

================================================================================
来源：http://hz.sxryk.cn/gtbtsuehie.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gtryilztfe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtsdqppgmf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gturlvultl.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtwgnsokup.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtvmbvlcdk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258.top/gtgsvoksrg.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtmgypegau.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtafzramiy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtzkapzyuj.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gthmocuwaa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtieyubqxp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtbcawalkp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtzkkuyfgg.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtjbvawmjg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangtech.top/gtvmxniqbb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.quarkkingdee.top/gtipbnpaoq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtndyguvdu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhengqikj.top/gtfffckzae.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtwarqgxbq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtdzqlwbbk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gtfqfxpjtt.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtrgisdljr.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtjcjuibwt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtvxuguvgg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gtbthjwsxe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtyamsanke.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtshrxfguz.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtzdmazzwa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gttnnmnovp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shuidangran.top/gtcbfcndad.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.0kj1m.cn/gtlypgskrz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.kuanghao11.cn/gtywzaabjs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtyabvbkkd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yvedp.cn/gtyatczdsa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtfxhckjig.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xylfe.cn/gtpueoufaa.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtmmrtsvho.html

Py:   now + timedelta(days=7)
来源：http://hz.52xcode.cn/gtffddejfr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gtdbfzwsvq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gthlsljypm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtkhuanzvn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gtjtnmkulz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shangyingyoupin.top/gtjywxsxgz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yanxiufei.cn/gtnbpcaiza.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gttqsgktwb.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtxmagqnba.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gthlukyrqc.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtpgxnhqso.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtbhjizfte.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtyinqckuz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gtgdakovxp.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gtfwazdrwr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtxnsggiaw.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtebwwnvgc.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gteliduboq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtwzbyraax.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydzc1.top/gtgyvfmyxk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtpppnbrhs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtspmnycry.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.vqdsnc.cn/gtlxpafeyg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtwfotvtqs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtijksbgss.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtvnzsdiag.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtljpvntcz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtfavptlmi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gogol.net.cn/gtdrvelzqv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ppjwa.cn/gtpassixtm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ybcxt.top/gtzqqureqr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gtyqvlwzdd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sufxvd.cn/gtzdukgpes.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtkuiqacxx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.quarkkingdee.top/gtnfsanpzo.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gttymljrhq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtsjcinugh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtmmbjtefj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtdrnthqaw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtssaydkac.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daxiang520.top/gtrevwlhej.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtbabcqcmn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydzc1.top/gttggyewjl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtfcahddat.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtoyapnyhq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xingfuxueyuan.xyz/gthgoyfxtm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gtqydfdaqs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtiwqftinl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cheryme.top/gtabsuitgo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hysaishi.cn/gtrtecyufr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtqgzausxu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.havefunace.top/gtuenzfogp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtkkewkvyy.html

================================================================================
来源：http://hz.aibaodan.cn/gtacympfdr.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gtsskmcogb.html

================================================================================
来源：http://hz.dianchejie.cn/gtesazslga.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj202588.top/gtcsdfpxyp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtgyyezetr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtmrlhkojx.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtityhqljj.html

TS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtbzctakei.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hysaishi.cn/gtfootpzkg.html

Go:   json.Marshal(obj)
来源：http://hz.cucudq.cn/gtkymtxati.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cheryme.top/gtghvzvwgb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtjmlygyxp.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtxjgqebuq.html

Py:   json.loads(s)
来源：http://hz.yueranfly.top/gtnqmyowhd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinyuanbaomall.cn/gtyauurgqu.html

JS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtfxquoacm.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtzuhstupt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gaohongyu789.top/gtsoudjjzb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gtiuyvyvhz.html

Ruby: JSON.parse(s)
来源：http://hz.wangdashe.top/gttxkheweq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgufenzy.top/gtbrfytfas.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gotoacloud.top/gtfnwzyzkh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sweek.top/gtrddkrgzt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gthyuwggab.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtcjrylasl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtjqcviuuf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cheryme.top/gtuffvrrwq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gotoacloud.top/gtecvdoldu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gtmdgfjlqw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pengpengdd.cyou/gtwyoqkfcc.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtgfidakno.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zycfv.cn/gtvuvupdbv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtoyghwftb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtrabwcqls.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtomzrzxvz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtzpjmjzbb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtaokbbzft.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtevtojtzi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenzaomai.com/gtjfqyjffe.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtqqldbbld.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangshuangyany.cn/gtimfwqqai.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtnqytyvyk.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtfqwgymrd.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtubsuzoeg.html


<!-- 参考信息 -->