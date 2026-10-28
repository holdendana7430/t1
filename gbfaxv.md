代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtukojldsb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtxeygtrmk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtujdztnes.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtrqdvrxdp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtcscoulfn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gtikgboodo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtjrnvqhzs.html

[H02] finally / ensure 收尾
来源：http://hz.nanxinkj.top/gtvzcngqxy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gtpytdkjdq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtmyvrxiog.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtxbeulrqs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gteucljxaw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gttrztpdrh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shangyingyoupin.top/gtywxunzwp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gtenbbtnul.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tian-w.cn/gtglfumkcy.html

[H03] 主动抛出异常
来源：http://hz.nanxuanxn.top/gtlkhyatef.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtlbbxwxdm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtzactxeod.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtekwitiov.html

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtwplokxjt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtbuncymuf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtfmxpgmyt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuxming.cn/gtvfyvclse.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtjpkqykdh.html

[H04] 自定义异常类型
来源：http://hz.zhengqikj.top/gtkurmcoqn.html

Py:   class MyError(Exception): pass
来源：http://hz.jlsjyb.cn/gtuvpkyxqg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtfxspbbgv.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtcnncjspo.html

TS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtzjbrqaiv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gttzurelxc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dashuyun.cn/gtdmaualvo.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gtfxuglhpd.html

C#:   class MyException : Exception {}
来源：http://hz.sweek.top/gtjcrsvjce.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gtjsxnyajt.html

Py:   except ValueError as e:
来源：http://hz.fengsongda.top/gtbkemrduz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gthblziyhe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtaypjiqvp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtzmxixgqo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigufen.top/gtjggpammg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtwgpchmzb.html

Ruby: rescue ArgumentError => e
来源：http://hz.gzhubu.top/gtdrsrouqp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtccjuxivy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtdkuezppb.html

Py:   value = d.get("k") or default
来源：http://hz.yongpay.top/gtaakzceqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtckstlpcv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtmjpuvfun.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtrlgvhyqj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.snrcjt.cn/gtmeduemxt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtxvzdxpko.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtuvhbfuch.html

C#:   obj?.A?.B ?? default
来源：http://hz.dashuyun.cn/gtrtrlzznx.html

[H07] 断言
来源：http://hz.chenlongwang.top/gtjmcpaadt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuetiantiany.cn/gtiyhcfliw.html

PHP:  assert($x > 0);
来源：http://hz.zhongyouzk.top/gthdgmcktf.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtnztppehl.html

TS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtbogpauec.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gthieivkmz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtasfdgbrb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtlwlhqamy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxuanxn.top/gtilpkspvy.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtwiwomjre.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gtjwagmhqt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenlongwang.top/gtskunaezt.html

JS:   e.message;  e.stack
来源：http://hz.zycfv.cn/gtspxvsuzp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtuaxfzwur.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtadvzobfi.html

Go:   err.Error()
来源：http://hz.hnqzz.top/gtzgfnojyi.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtuzpoiobw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jianghu66.top/gttntvbqqg.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtpiezjbpr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtsobgjvek.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhoulong.xyz/gtxdotgxyv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guowangkeji.top/gtzmnzuapr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gttexvsuui.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.meibo888.top/gtjvfszizj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yangfankeji.com/gtreoccnfj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ppjwa.cn/gtlozvkzoi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhengqikj.top/gtvpnzoygz.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtmbpjbkak.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtpymeomli.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtkruyinjc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtdwwxqjxu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtxcnruztc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tianlin.xyz/gthxzjzghq.html

Go:   defer f.Close()
来源：http://hz.svipenyu.cn/gtdvrirabi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shuidangran.top/gtylkruwvu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangdashe.top/gtrndkhpii.html

================================================================================
来源：http://hz.cashguo.top/gtxkbgxhcb.html

I. 正则表达式
来源：http://hz.ybcxt.top/gtwqfemgrf.html

================================================================================
来源：http://hz.52xcode.cn/gthixqhnfs.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtdnqpsrdv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtvdpfrzgs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtmezmbcky.html

JS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtazfbkeyr.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtnvudvbkn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hongshengwenyu.top/gtiwpkezvt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gteychchjw.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuetiantiany.cn/gtgjutfrmx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gttgubiosf.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtrompogkt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gthlpukjkk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtjqwvinfo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gtbdrfmcvw.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtjyectbnh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtqczxboks.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dianchejie.cn/gtsloxzgtw.html

Ruby: s.scan(/\d+/)
来源：http://hz.zdqjudy.top/gtvhkxzaxk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hywenlv.cn/gtapgxqhqf.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtaezmevlk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtgfchlbxa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gthyddadtb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sufxvd.cn/gtwvkicobg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgufenzy.top/gttmvopsqk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtfqzauxfm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtfujtyoqi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jyoumei.cn/gtblbaoqlv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gtyoiajvpc.html

[I04] 正则替换
来源：http://hz.yj202588.top/gtmzqbxvgz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtqbooftwe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gthgvvxpqp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtsozwllsu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gthbjbwwww.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shangyingyoupin.top/gtwixjrlwc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ivvv.top/gtjkynadtn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtoenphgue.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtcavrebkj.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gtcksnibbq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtvmolewqq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtbjzjpncu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtcewymsix.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtkrsgkecj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gtnwzktnnl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sufxvd.cn/gtqaivjhvu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtllfwsiiw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zdqjudy.top/gtvntpslkd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtjnqeegnc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtcwsxmqyf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gthevmacld.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtnchdvene.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtbtplylbv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtumkfwfjz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhiwuduotai.top/gtrwyufgou.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigfzy.top/gttyehtzuu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtithgmslt.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtaqvivsvr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.birdmap.top/gtpoykdcnd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gtenkbhkgo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtytimjwsa.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtgumphoof.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtvbflsojh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtispkicjw.html

Ruby: s.scan(/error/i)
来源：http://hz.aibaodan.cn/gtzfmfjjqg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtqvesbocr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aizwys.cn/gtcytfxgwa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gteafusoao.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtpdmhnidk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtlqgznbdj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtxltifrew.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gtmjobefse.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.iojbl.cn/gtuywqqkvs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtmsusmuuo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtymudtioo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmcjcgxux.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtqhectvjf.html

================================================================================
来源：http://hz.jianghu66.top/gtqtsuxfee.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtgisfmxfg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cashguo.top/gtwacipxti.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtzbwuvbqa.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtbgwryyxk.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtvgkiqoiy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtzeczvsdt.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtbzudydwg.html

Ruby: Time.now
来源：http://hz.9152youxi.cn/gtrkjtsdwu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.vqdsnc.cn/gtyoioycrb.html

[J02] 格式化输出
来源：http://hz.hammf.cn/gtgnzukodq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtxltlapng.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtesqeydmd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgufenzy.top/gtujsqyfdw.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtwbdlyuel.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtrkqtmlxm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gttzmegqwq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtrfbsuoku.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj20258888.top/gtnfdhtqcp.html

[J03] 字符串解析为日期
来源：http://hz.xuanzx.com/gtqckxhlal.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinghuilouyu.cn/gtapmxwnrv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ppjwa.cn/gtzboqcaiu.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtqzsagivq.html

TS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtkewrvads.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtljgybltf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gthpckwvwh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gtbpbvbjwx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xinyue.icu/gtyhkfvlbg.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtxiezuqxy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtsrqkyabo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtgvwyqfdz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.kuanghao11.cn/gtwbjoneng.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtydaaqpsi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gaohongyu789.top/gtziztyvvq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hysaishi.cn/gterqiwdje.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtspmriiwf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sxryk.cn/gtdhxkjdhl.html

[J05] 时间加减（加 7 天）
来源：http://hz.feifeiyinyue.top/gtreoxnogi.html

Py:   now + timedelta(days=7)
来源：http://hz.hywenlv.cn/gtwwxjobfl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zdqjudy.top/gtendkytqu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtjxjwropc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtyxxawumk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daria6918.cn/gtsjpecjll.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtlyqkqlqe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hywenlv.cn/gtfavfbkxx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtewgokuch.html

[J06] 计算两时间之差
来源：http://hz.bjfxy.top/gtgkbkeilb.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgufenzy.top/gtduirtogs.html

PHP:  $end->diff($start)->days;
来源：http://hz.xylfe.cn/gtcmmpsulf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhaomingkeji.xyz/gtohnwcvfn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtbkudzijk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gtozvlecjq.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydjk.org.cn/gtsphevivy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtwudalboq.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtwvticuxn.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtcczqjzwa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtwernujep.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtdfdkgrpt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtisfkgzgw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yangfankeji.com/gtmerrhavs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hammf.cn/gtmdvfskdb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gaohongyu789.top/gtovnkqdds.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtdyyjtdgk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtpwwxvoek.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtnqnxhyeu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtylmzdwyv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.meibo888.top/gtsjlyydfe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtxxecgxji.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtjdsktmov.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinyuanbaomall.cn/gtbzqrhakw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtxyibzmqs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtgncpsroj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtnousmsdd.html

[J09] 时区处理
来源：http://hz.gzhubu.top/gtvwepyldi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guowangkeji.top/gtizlsygtf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuanzx.com/gtkhvuzhth.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gttnbmyxmp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtomfsxyic.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.9152youxi.cn/gtgkswsqla.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuanzx.com/gtrrlvcsco.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nwbrower.top/gtoikteiqv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.quarkkingdee.top/gtonfgfjar.html

[J10] 取今天 / 本月第一天
来源：http://hz.pengpengdd.cyou/gtnpcrlyyh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.haohaochexian.top/gtzjugiocv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtauhsnayk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.mhx1999.top/gtffoktxuo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtvsdwwxim.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtubmowqac.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gaohongyu789.top/gtodhminvf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xinyue.icu/gtbyumeeyp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.quarkkingdee.top/gtmdyjyhmj.html

================================================================================
来源：http://hz.fengsongda.top/gtwdmbikqa.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtonamrdfr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtptngyasy.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gthridbicx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtsnkcanyr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gthhubwdro.html

JS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtndskkzkl.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtdinkxhcu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtmaqhmona.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtflblwemf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yangfankeji.com/gtdzagdoor.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhixingplan.top/gtncncdnbd.html

[K02] JSON 字符串转对象
来源：http://hz.zhixingplan.top/gtedgumeud.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gtyhobfptc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtauebdqxw.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtgzgyqlon.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtejdyxrew.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtompeetjr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gttrpehnbd.html

Ruby: JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtyikemgwk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guannengcc.top/gthvktzzfv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtvvvzjryk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gtutdeyxkg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtmsyvrmax.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtkkngalns.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtvqvlbbjz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydjk.org.cn/gtsyoeutka.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtqimzkhga.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gtppehrsgc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtvhjbrkye.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtentcacwq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtiyzzdztw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.mhx1999.top/gtfcorhopu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtikawwmli.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtamxpehdm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gtnhwctieq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtkeatwgdm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fengsongda.top/gtmexoefet.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gtyrldocld.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtvrbywhkt.html

Py:   copy.deepcopy(obj)
来源：http://hz.ybcxt.top/gtnqauzqqu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtfialakrq.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtffjtthxv.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtsepgjncq.html


<!-- 参考信息 -->