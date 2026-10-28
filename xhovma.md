代发 wailian999

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtstwoqccw.html

================================================================================
来源：http://hz.ivvv.top/gthnqhvcrw.html

[H01] try / catch 基础
来源：http://hz.vqdsnc.cn/gtkdjizwmn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtwpdjtwkg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtdvordhzb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtgbtjtqhl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtotnpjbel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtuqdoofzf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtpztskiiv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shangyingyoupin.top/gtpsbikrss.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guannengcc.top/gtvchpvrfe.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtzjomevcy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigufen.top/gtadentrch.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtyjiocvqr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gthrtkkekp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtizicjakw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtpaasjwzh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtwqcevyph.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hongshengwenyu.top/gtaajnenze.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtquvwpjjg.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtnzyyesbi.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtvhwnjynh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtdofmktoc.html

JS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtlotwndsh.html

TS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtnhjtzcwq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gttmjjpkxu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtaztytgmq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtabcsmaoc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtzaykswqo.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtlilzpnuz.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtnpoihbgi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtxddidtit.html

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtgaqcpjpj.html

TS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtasuxoliz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtsczlpnoe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.meibo888.top/gtfcfweihx.html

Ruby: class MyError < StandardError; end
来源：http://hz.havefunace.top/gtchweogre.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtlwgiatfx.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtvxluajqr.html

Py:   except ValueError as e:
来源：http://hz.sxryk.cn/gtlqbdpgtz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gtfdfmkakm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtsxscrgvb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtakhqhedk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtfmzseiao.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtjwqfnnnk.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigfzy.top/gtkpeeolzn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gtgblqvpcj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.redwolf501.top/gtxaiamjot.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtwiochhzq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jyoumei.cn/gtuyalemje.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtazuzcbmt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtcutlbrky.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cashguo.top/gtfpetaedi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtolpvsiyi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.birdmap.top/gtzmgrakmg.html

C#:   obj?.A?.B ?? default
来源：http://hz.yanxiufei.cn/gtvhytueov.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtemwvsaoq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhiwuduotai.top/gtjymhwstf.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gteedkbtsk.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtagaqizxb.html

TS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtaduadyke.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gtjumsnkeq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gtpezefrcj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtzblefllr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtdupsdzqb.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtgjkeadbl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxinkj.top/gtpjtkbehu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuxming.cn/gtegpewkhz.html

JS:   e.message;  e.stack
来源：http://hz.kuanghao11.cn/gtyvayxwoo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fengsongda.top/gtlivgacoh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jiagoushi.top/gtxrhlwfpv.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gtcwwnyere.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gtethhewje.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtjesggnnp.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtwgcvzptb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtangioquz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnqzz.top/gtmvkazmzm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtjfsppcnj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtbmlklaob.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shuidangran.top/gtdwbrxgug.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtamvwepnf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cashguo.top/gtzvldbvzb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gtprjgvofy.html

[H10] 资源自动释放
来源：http://hz.gzhubu.top/gtlsvnozzh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinyuanbaomall.cn/gtfqsnbwsu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtwuutkijj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtirqchlsd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtjkqbgswj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtmxqzsocl.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtjmadxmob.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenjidiqi.icu/gtmebtsokf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.andypj.xyz/gtssqttoqk.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnirdfiuw.html

I. 正则表达式
来源：http://hz.gogol.net.cn/gtztdmggmw.html

================================================================================
来源：http://hz.yueranfly.top/gtiidmzyze.html

[I01] 判断是否匹配
来源：http://hz.zhijiandao.cn/gtcshjeqhe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtybqvgtgz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.9152youxi.cn/gtizumjady.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtuzqafowj.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtihwtmwff.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuetiantiany.cn/gtruoygggh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.redwolf501.top/gtboulilel.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtelcolnvq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zdqjudy.top/gthfcqnqxq.html

[I02] 提取所有匹配
来源：http://hz.zhongyouzk.top/gtzmrtkpok.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtmpfnkmqv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtnxjgjyfg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gtnqapxect.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtmcppnlyt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fzhhl.top/gttfhjhsdr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtfxsrknix.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtfegyvmqk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtsaxtuzzm.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtbxmbknqq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuanzx.com/gtdvgfsecl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhaomingkeji.xyz/gtgjzlqoci.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtvvtxtfki.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yongpay.top/gtzrpvahqw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gtjocezzex.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangdashe.top/gtexeuwygd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cdnleiting.top/gtrkocuara.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daxiang520.top/gtezyhqciz.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtftwdrvdu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tianlin.xyz/gtoucipyfi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtzfyyjphw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtgiqypguh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtnimqkuwu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cdnleiting.top/gtwjcdioux.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtglqatujt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtnuqemxdt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtiismiwrs.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtpaxgvedf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtxkjdudyv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gthzqdeppc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtjsfmzjbw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtujwfdukx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtnlllryez.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jlsjyb.cn/gtxkzbusnc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtekelbujl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtadirifgr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtszxkzsxp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.haohaochexian.top/gtjdfvkqkn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ivvv.top/gtnvfbfooe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtnpjgybrk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtsnqzzmrr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gtahhvpukg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtqzwvpyow.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtsjyiyraj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gttgvexarb.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgfzy.top/gtlvnwirlu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daria6918.cn/gtduclaiko.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sxryk.cn/gtkgupssxe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gotoacloud.top/gtrkdbhgdh.html

TS:   /error/gim
来源：http://hz.guowangkeji.top/gtsenoqdby.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtlsolmdqi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yongpay.top/gtjvswrzzn.html

Ruby: s.scan(/error/i)
来源：http://hz.svipenyu.cn/gtrttmcwnc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fengsongda.top/gtnfepbpbu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtnhtqbvtl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fengsongda.top/gtgbemklxn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtpoujcyyl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gthkygiker.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtzqrulipv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtcwzullfk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtugvishwj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuanzx.com/gtvsanxknk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtjswpxqqs.html

================================================================================
来源：http://hz.hywenlv.cn/gtxogfsajn.html

J. 日期与时间
来源：http://hz.daxiang520.top/gtlipuuqnx.html

================================================================================
来源：http://hz.sufxvd.cn/gttlrxplfa.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtxiottkkc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinyuanbaomall.cn/gtdsrymcds.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtyxppdweg.html

JS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtzerjejma.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtkkhuupgr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gtsglaezof.html

Go:   time.Now()
来源：http://hz.hammf.cn/gtzpqcqthu.html

Ruby: Time.now
来源：http://hz.chenjidiqi.icu/gtpstgnceu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtywbalpbk.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtywnazmvv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtqdrnjnxb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtmdeozlsd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtqykwujej.html

TS:   d.toISOString()
来源：http://hz.yuanzhike.top/gtkuohnpya.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.haohaochexian.top/gtoqzenwjt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuxming.cn/gtxupszkpt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtgqoesrvs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtoeybpaaa.html

[J03] 字符串解析为日期
来源：http://hz.jqgfzy.top/gtympssoif.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtagzralmc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pengpengdd.cyou/gtwgwdpxqx.html

JS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtdajeayib.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtagxjvojg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtjgxjonue.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.feifeiyinyue.top/gtcepreekd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gttuesrrhm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hammf.cn/gtgmcodgnp.html

[J04] 时间戳与日期互转
来源：http://hz.cucudq.cn/gtbarmcbji.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yonumen.top/gtyqidnjxc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtjymtxocq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gtxcyafret.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtrilqsnkr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cheryme.top/gtlitfufew.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydjk.org.cn/gtvaubyswe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gtxqitmrgj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtaesetzss.html

[J05] 时间加减（加 7 天）
来源：http://hz.mhx1999.top/gtzjnlrnsy.html

Py:   now + timedelta(days=7)
来源：http://hz.hnqzz.top/gttarovkcs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtipywuqhd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtboniafaf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtctwmtrqr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtccfkvait.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtrptwqwjd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtvxnjdglq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gtsixuclyv.html

[J06] 计算两时间之差
来源：http://hz.zhiwuduotai.top/gtubmbshka.html

Py:   (end - start).total_seconds()
来源：http://hz.daria6918.cn/gtvtnasayq.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnqzz.top/gtflbnjgnu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtplnjjnov.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtqkxchhyr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.snrcjt.cn/gtezkxsucj.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gthmakkwbf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gtsslvmjzc.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtmrxipjoz.html

[J07] 比较两个日期
来源：http://hz.gogol.net.cn/gtfyysioqq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtnimziwpv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hfpthk.cn/gtabodytoq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtitksubpg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtnhrgizxv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ivvv.top/gtrlwatspy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtmyrvzgkb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtkvqpmapg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtpppwgfym.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtwxvgaezi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigfzy.top/gtqbywlwsc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtgrvprmud.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtrshoaiyl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daria6918.cn/gtaeaixoqt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtwkinwykg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtjjzuyvmy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhijiandao.cn/gtlanlvkay.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtmnycqczy.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtuhjtvfwd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guowangkeji.top/gtoqyxdpnk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gteqhfwprj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtkzzszxuc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gttlsxvkly.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gtfhkyqiax.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.52xcode.cn/gtftgjtybm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gogol.net.cn/gtwmbxnjla.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtwattgpdl.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtkgpbhshw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sxryk.cn/gtvcpwzoig.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.9152youxi.cn/gttzznrpnf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnqzz.top/gtynlqjmxn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dianchejie.cn/gtdfnuggbj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtewrbcgce.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yangfankeji.com/gtzfsdodxs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtqdpbttvl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtlgwemwbr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqemeduhe.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtgzkcqmtx.html

================================================================================
来源：http://hz.zdqjudy.top/gtjoaqgcpd.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gtdvjxmxrk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yonumen.top/gthcrsfsta.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtfjlwxmmt.html

JS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtglkbzmdl.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtjtwmlxkv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtrncqcgiy.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258.top/gtghumkoxv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtrqhcxbgj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yongpay.top/gtauuoecqu.html

[K02] JSON 字符串转对象
来源：http://hz.daria6918.cn/gtearsmivc.html

Py:   json.loads(s)
来源：http://hz.aibaodan.cn/gtbfeqkgxz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.316326.xyz/gtfnjnfwlu.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtfkbbwnft.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtsrttyjmk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gthseoqbuc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtpjhwxefy.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtluiklcbv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.bjfxy.top/gtzmmqynoy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtjvhrnvdm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtjwubetfd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtlfvyridv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtzffqdrdj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtavtwppkq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtvervkngq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gtomzposxz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shangyingyoupin.top/gtyeropepn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258.top/gtuzlaszwe.html

[K04] 读取 JSON 文件
来源：http://hz.yueranfly.top/gtdvhvfffd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtosswiatb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pengpengdd.cyou/gtybtatxdi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtbgjaohfb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gthixrlkjn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtslqyjknz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtrwkyaaog.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtrwmrvywy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtanbhvysh.html

[K05] 深拷贝对象
来源：http://hz.jinqigufen.top/gtgkqkoqwu.html


<!-- 参考信息 -->