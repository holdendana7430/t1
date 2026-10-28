代发 wailian999

H. 异常与错误处理
来源：http://hz.hnqzz.top/gtzmwbojdd.html

================================================================================
来源：http://hz.nanxinkj.top/gtycvtrmco.html

[H01] try / catch 基础
来源：http://hz.chenlongwang.top/gtwvkldluy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cdnleiting.top/gtshideovf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shzxlz.cn/gtxadddhlx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtwobtlndh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtbcqbduba.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtvrvxaduy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yvedp.cn/gtpomtenbp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtbgnhgpff.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hysaishi.cn/gtdwbhcmlx.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtwbniwscm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtxlbopqkm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtxhafemov.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtpjiiqvcg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtkcnrdqsy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtdszhpthi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.316326.xyz/gtugoqjhbf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dianchejie.cn/gthneyectt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtjwpnsqwa.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtmmypbztn.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtoiemyfql.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtkibywlza.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtcpbswziy.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtgbzyaqhu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtqxrnerkn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtlrnrctit.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtuqytyory.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtjjhrwqoy.html

[H04] 自定义异常类型
来源：http://hz.gogol.net.cn/gtdjumhllb.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gtchywqtdr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cdnleiting.top/gthfkvokke.html

JS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtwniithyc.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtiykinwpd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtfrlpmwid.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtkwupyqox.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gtsbwxnmdr.html

C#:   class MyException : Exception {}
来源：http://hz.cashguo.top/gtmzwhaavc.html

[H05] 捕获特定类型
来源：http://hz.svipenyu.cn/gtoqzkgipc.html

Py:   except ValueError as e:
来源：http://hz.vqdsnc.cn/gtfqvcuzkp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.kuanghao11.cn/gtuowhdotc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtxtjisteh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtxnhqvctg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtjbjboxmi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxuanxn.top/gtknjbimns.html

Ruby: rescue ArgumentError => e
来源：http://hz.yongpay.top/gtvphtjgvh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtpzisvsbv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ppjwa.cn/gtnalvbgui.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gtbrapnxmf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xziqi.cn/gtqhedqaeh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtkppcxdfc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gttumlgtru.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hongshengwenyu.top/gtmsvvmyys.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pengpengdd.cyou/gttehjeyga.html

Ruby: d&.dig(:a, :b)
来源：http://hz.birdmap.top/gtyrmhghlt.html

C#:   obj?.A?.B ?? default
来源：http://hz.ybcxt.top/gtbabrluhi.html

[H07] 断言
来源：http://hz.cdnleiting.top/gtremirssz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pengpengdd.cyou/gtjpgavxxa.html

PHP:  assert($x > 0);
来源：http://hz.havefunace.top/gtdrnswoxu.html

JS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtpuqzswru.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtwelykpro.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yangfankeji.com/gtxnmzwrgy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ppjwa.cn/gturphcnsu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gthxsuukwp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtujhndpxi.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigfzy.top/gtkfxjwtdv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhixingplan.top/gtakzzcsmw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydzc1.top/gtmykcnxqv.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtyrrfiygl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gttdfwvzlt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jianghu66.top/gtsacdpcxy.html

Go:   err.Error()
来源：http://hz.yj20258.top/gttabedxom.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtibmpukln.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtwtyjbxho.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gtlsuosbkj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtszejuosn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtuavxhzjp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zdqjudy.top/gtefgnthzv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ywan-chungtsiang.top/gtztfqmlpq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.havefunace.top/gtupulvnns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.c1oappe.top/gtyxlzgfff.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guannengcc.top/gtjykpfaov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtncmvewfi.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtbtljskff.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtwuyhrfpk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtddvyuwsx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtdmzafrbj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtssyrgnom.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtimujbotd.html

Go:   defer f.Close()
来源：http://hz.zhiwuduotai.top/gtmuklphqi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zycfv.cn/gtleqexsdx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fengsongda.top/gtxvalwocf.html

================================================================================
来源：http://hz.yongpay.top/gtssbicvch.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtgkdknnyw.html

================================================================================
来源：http://hz.iojbl.cn/gttjaidoel.html

[I01] 判断是否匹配
来源：http://hz.yuanzhike.top/gtqqrzwjhz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtuwyokdpi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangdashe.top/gtqcftqidv.html

JS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtaiobeixh.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtgoidnuaa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxinkj.top/gtdbihjwum.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aizwys.cn/gtrhdeztmu.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtgylppogm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yongpay.top/gtvopjjyor.html

[I02] 提取所有匹配
来源：http://hz.chenlongwang.top/gtuabrzcpc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnqzz.top/gtipcpznaa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtffnmfepy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gttelcvttt.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gtnnayjnpo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gtvxoonhjp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtguzyhubr.html

Ruby: s.scan(/\d+/)
来源：http://hz.xinyue.icu/gtaavvwhfi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtrgqwmccv.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtlyxxpzpb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtbnixdhew.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtcdynktze.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sxryk.cn/gtebzljwzi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtcvtfmgla.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangkeji.top/gtbibpjgcm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gtwfraxkip.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtiaowealk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtjyxkiqfe.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gtehbuqwbt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtkueqrvnk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtrhfxabzx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gttctaagur.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtuetjvnpz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtiqrlerts.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtmwkcghuc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gtevkaafko.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gaohongyu789.top/gtxcjfmqxw.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtcmnmqesg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtklbjhreu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sweek.top/gttypifgkv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtymgospkz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtfghgezrq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtrbemwily.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtlbkzedav.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtfiqqmglu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtadlxvorr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tian-w.cn/gtigrzaazc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtiudpvpif.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.andypj.xyz/gtweiwhjrp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtjeqtvjnd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtqdkxuzwg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nwbrower.top/gtjwxpylys.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtbsvewiyp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtlcckkifh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtkkamivtb.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtjupctafg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xziqi.cn/gtzcnzzjny.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtigpfykbg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtshrmpbig.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtvegwcaac.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ivvv.top/gtylgwouzz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gteejfvfec.html

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gtkovplmoo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cashguo.top/gtdxlzdyae.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtepamhvtc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtyppblrsh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tianlin.xyz/gtnfnrpfka.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtewizftrm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtzmooepxp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtlajaxwiy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gtuttwivsh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtebcnyjkn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtofnimiir.html

================================================================================
来源：http://hz.xylfe.cn/gtkcnkuizo.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtivgvyedc.html

================================================================================
来源：http://hz.jinqigufen.top/gtgletvvqy.html

[J01] 获取当前时间
来源：http://hz.gotoacloud.top/gtyqvdmfvw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtgejrsryw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtyjwkipmd.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtujmnweie.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtpvhywmkb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtpkajfwyp.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtgncevjik.html

Ruby: Time.now
来源：http://hz.jlsjyb.cn/gtzhpxdsed.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gteifaqhyf.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gtuyydcayh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtykazldfn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtbvyrvhix.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.havefunace.top/gtivnqssjz.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtldfbwunt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jyoumei.cn/gtivspimrf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtlctysmad.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gttwdezddj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtaacilenm.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gthgdjfixd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhongyouzk.top/gthvnjmpvo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xylfe.cn/gtxbvplakj.html

JS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtenrtkrxf.html

TS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtguqzshux.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtxleyavtt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtdkegatvl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtezkrlowo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gtizqhtmim.html

[J04] 时间戳与日期互转
来源：http://hz.zhiwuduotai.top/gtgcbrwerd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtdonajjop.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtkjxmpqxw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtqctrwepk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtjnwevrqb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gaohongyu789.top/gtuudmqodf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtjgeoxuvg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.havefunace.top/gttivsucru.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtjjwcbavw.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gttkrvxzjw.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtfvnhbacx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ybcxt.top/gterujknur.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtcxcewpqd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtosbrgadu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gthvzubtdg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtyrmmbght.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenjidiqi.icu/gtqpvstflb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtgpurudmv.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtteabneeq.html

Py:   (end - start).total_seconds()
来源：http://hz.andypj.xyz/gtwdvpramz.html

PHP:  $end->diff($start)->days;
来源：http://hz.yueranfly.top/gtmqoziwea.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtxsbdbfoe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhiwuduotai.top/gtpasdgthn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ybcxt.top/gtybwtadkv.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtvbfdekfo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tanke756.top/gtqhgupyvs.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gtlriuexzf.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtldmuejzn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtskaiokue.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtmtcqjuye.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtoecixfyu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtjsukyzjn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fzhhl.top/gtmiqrllkz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtzcgzcrqs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtrkqpcfra.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtgghpulsq.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtijavccmf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fzhhl.top/gtewowebgm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtrvlqgcxe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtfmmjtgmm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ehwqpu.com/gtcyizwnhm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtnzfdbnqn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtbydthaxs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtiunmmmlk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.feifeiyinyue.top/gtbjslaiui.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtfloskdjl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gotoacloud.top/gtbrytpstp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtlkhkpbpw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtkeilexff.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtznubivzd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtbrxogqni.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangdashe.top/gthpvwxicv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guowangkeji.top/gtzpvguyut.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtyalaeymo.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtzhhbudvv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtzaiwdegp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gtfcpsmbbv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinyuanbaomall.cn/gtlrseslvn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinyuanbaomall.cn/gttiguufcb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtuybmvkzd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cqqwz.cn/gtmnxthsqz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gteowcxxyj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gticggpmet.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdqkcxjsi.html

K. JSON 与序列化
来源：http://hz.fzhhl.top/gtoobowpaw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpieunlds.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtscmeafqm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtyxnnchns.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtumvzyucj.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtziezniwg.html

TS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtdqdpqwsk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gtoijpzpbg.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtvyowokxv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtljdozkbn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtjvwsszrc.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtyjaodrpn.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangkeji.top/gtgratqklf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cucudq.cn/gtfopvxsuu.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtzzchdlaj.html

TS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtgciickto.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gotoacloud.top/gtbzjqixhk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtnqjtiksh.html

Ruby: JSON.parse(s)
来源：http://hz.gzhubu.top/gtcgadvyrb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuetiantiany.cn/gtaubruxeh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.quarkkingdee.top/gtjukkphrt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.birdmap.top/gterfegfxf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtgubjfjsl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtmzorsxhb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtojpbuqze.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gotoacloud.top/gtcakxlvjk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258.top/gtdcbbpqzl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtjkvrkzji.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtzfmkbmbz.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gtclfpvbno.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gthgoocqoq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtjxempaof.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtysmmnwdq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtyvhnriwo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgufenzy.top/gtudokpzir.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtnhqugiwf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtlbifudcd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtjbzmnouc.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtzfekqqdk.html


<!-- 参考信息 -->