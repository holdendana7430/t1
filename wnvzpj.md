代发 wailian999

H. 异常与错误处理
来源：http://hz.pycfn.com/gtzyipendh.html

================================================================================
来源：http://hz.hfpthk.cn/gtzguyfsrj.html

[H01] try / catch 基础
来源：http://hz.vqdsnc.cn/gtdnpvncxn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cheryme.top/gtjqpeucnk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jianghu66.top/gtbkceyjgu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtulaqktyp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hywenlv.cn/gtvyipzrop.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtkjeldutd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhijiandao.cn/gteiugtpys.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtgcbatmwk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.vqdsnc.cn/gtxiqjhoof.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtxmoolyub.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.feifeiyinyue.top/gtfkschswd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gttmbrntap.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtvesdzpmu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtrvtyfzpm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gteghivajk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yanxiufei.cn/gtucstjbsa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gthcejxhix.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shzxlz.cn/gtlpcxnhuc.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gtdptwdzlu.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtyxghvfeo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtsycivhlu.html

JS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtjjrbstmj.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtdvzgkkpu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtbqdyfbcz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtdpsmiihg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtebqzfeaj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtzzfkbjny.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtxlyathdi.html

Py:   class MyError(Exception): pass
来源：http://hz.yvedp.cn/gttqazaljb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aizwys.cn/gtqvxbjxnp.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtbhceapmk.html

TS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtwybntyfb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.andypj.xyz/gthrfphoet.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtwgwyxjzu.html

Ruby: class MyError < StandardError; end
来源：http://hz.hysaishi.cn/gtkmemrpyc.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtouqivxry.html

[H05] 捕获特定类型
来源：http://hz.pycfn.com/gtvigdyrwq.html

Py:   except ValueError as e:
来源：http://hz.cashguo.top/gtxhzwlqov.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daxiang520.top/gtwtvgoykv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtfhvkncxe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtynsyurtd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cheryme.top/gtplnvlkkb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinyuanbaomall.cn/gtakkowvis.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gturffiogo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtntfereiz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.feifeiyinyue.top/gtgkkobbqm.html

Py:   value = d.get("k") or default
来源：http://hz.316326.xyz/gtbevzdhdk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtvjgdhxlt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gttawgmipb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtrrajqagm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shzxlz.cn/gtsuxtauqa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yangfankeji.com/gtcfqgnjcj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtgbzxldno.html

C#:   obj?.A?.B ?? default
来源：http://hz.fengsongda.top/gtrdvsppan.html

[H07] 断言
来源：http://hz.yj202588.top/gtqadjlomb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuanzhike.top/gttkddpphh.html

PHP:  assert($x > 0);
来源：http://hz.yj202588.top/gtuncrgkgd.html

JS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtpvfldjmq.html

TS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtgwntqadh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhengqikj.top/gtpnnzhrhw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.iojbl.cn/gtthpisysf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuxming.cn/gtwablojrz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtkrgdsvxu.html

[H08] 获取错误信息与堆栈
来源：http://hz.pengpengdd.cyou/gtrwcfkszf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtrzobhhpr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtdzdipdjy.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gtvetwmmig.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zdqjudy.top/gthzigiozd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtuopznoal.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtyhmuqlwz.html

Ruby: e.message;  e.backtrace
来源：http://hz.pengpengdd.cyou/gtxmnfcruv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigfzy.top/gtiduykfzb.html

[H09] 带错误码的异常
来源：http://hz.gzhubu.top/gtmcgniymx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gtdajylded.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtvohofdef.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtqrfgoqeh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.quarkkingdee.top/gtaybvbukr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tian-w.cn/gtalebwexv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sysykeji.top/gtovglqafx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtoemtpzkp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtkyucicnt.html

[H10] 资源自动释放
来源：http://hz.zhengqikj.top/gtljskhgcj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aibaodan.cn/gtxaaqgmrq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtlmsqzbvy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtlcmcmnfn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtyqwdwhyz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nwbrower.top/gtmqghifpk.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtxtbqojvq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shuidangran.top/gtmdyyiehp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtcdsttyju.html

================================================================================
来源：http://hz.meibo888.top/gtrreptbzk.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtlrwcqfef.html

================================================================================
来源：http://hz.c1oappe.top/gtynbqmcni.html

[I01] 判断是否匹配
来源：http://hz.hammf.cn/gtmuzewayj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ehwqpu.com/gtnkhavvkl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtelnxiskw.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtxytjwuqr.html

TS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtkgcsmwtr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtttayyhrj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tianlin.xyz/gtcvdpaoyp.html

Ruby: s.match?(/\d+/)
来源：http://hz.52xcode.cn/gtpzjawcdk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtbfssihsq.html

[I02] 提取所有匹配
来源：http://hz.zhijiandao.cn/gtwuttzlzp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtwsmoubjq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtxdjffpde.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtxhuxmtrh.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtmewjvmfb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gtianeebqo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.haohaochexian.top/gtlezlfkab.html

Ruby: s.scan(/\d+/)
来源：http://hz.gaohongyu789.top/gthygbnncf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtyxikpdka.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtgfkzuuws.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtluzntkpt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangtech.top/gtdbiciyev.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.havefunace.top/gtlqfuqzxi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gttrogvlfy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtgwozmttg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtnxoawgnp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.feifeiyinyue.top/gtzatkcqof.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtffwplkws.html

[I04] 正则替换
来源：http://hz.ydzc1.top/gtzmjmoahf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gtojqwoaao.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtoqmxhzsv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtlpoepewt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gtbjixxkwk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gtfferurkb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yangfankeji.com/gtebmeeldn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zdqjudy.top/gtkdppiphd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtkqhbttyk.html

[I05] 按正则拆分
来源：http://hz.andypj.xyz/gtlggkhpqt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gaohongyu789.top/gtttubrvja.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtwrotrfjn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtsvlazdrf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gteygamrvn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydjk.org.cn/gtxpwelpvn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fengsongda.top/gtevventzw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtlnqyuqou.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fengsongda.top/gtxsecbpgm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtddsjygqq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtrhogoxff.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtrukyxkeu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtvamuedrf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtuohzmqvf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtmdtvjokd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zycfv.cn/gtdlwclqoy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj202588.top/gtphbiwzjy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtfmieusrh.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtpgwhlqsn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.bjfxy.top/gtpuahqqfg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtagqxvujv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tian-w.cn/gtaziwmldu.html

TS:   /error/gim
来源：http://hz.9152youxi.cn/gtscudfxmd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gtfqoqndkc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guannengcc.top/gtldveggzb.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtioixpmkf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yongpay.top/gthykstlge.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtldwlfhmz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtmcubbqqo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtvcljektr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gthviddbij.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtzkpsxrte.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtzsmszvfo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtfibmzfdr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhongyouzk.top/gtngzcikun.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtamwpppad.html

================================================================================
来源：http://hz.nanxinkj.top/gtzuxqshdc.html

J. 日期与时间
来源：http://hz.mhx1999.top/gtczzkonpr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwwadyunl.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtcrfzvmob.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gtmftooawr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtxhgunsmq.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtrnuuirpr.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtdhyozvxg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtefipjodt.html

Go:   time.Now()
来源：http://hz.jinghuilouyu.cn/gtoxddqzwk.html

Ruby: Time.now
来源：http://hz.cheryme.top/gtounymmst.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenlongwang.top/gticxffxfq.html

[J02] 格式化输出
来源：http://hz.nanxuanxn.top/gtnrmkkdli.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtlqwvezdd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtjmfdxwyc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtreguvutp.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtcdvtzjtk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtlagjzlnl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cashguo.top/gtkfyurbcy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtuzrvfgwt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gtrjqldohk.html

[J03] 字符串解析为日期
来源：http://hz.dianchejie.cn/gtbpfryspj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pengpengdd.cyou/gtwrxypxag.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtlidiavbo.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtmrjdmejl.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtervahaap.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtoxbkinnt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sweek.top/gtksdyvifh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj20258888.top/gtxkkznhon.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtsobxcwqq.html

[J04] 时间戳与日期互转
来源：http://hz.hywenlv.cn/gtiwaaodqf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gtwzaxtooo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cdnleiting.top/gtpaymvjzx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtdktsavjm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtibqemjwb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.quarkkingdee.top/gtvjzonkek.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuxming.cn/gtsefyftuh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtvpmvadhj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gtsuolxvgq.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtnzfkkmmr.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtizturmfu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtiucynqzn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtivmnmrwc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtokhejmxk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gtdidslhzl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fengsongda.top/gtztjggokd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yanxiufei.cn/gtsvrxdybn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gttviumigl.html

[J06] 计算两时间之差
来源：http://hz.tanke756.top/gtniueucat.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtdogrndsz.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtouuocoft.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nwbrower.top/gtxqcqgnqg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtohiqvrth.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gotoacloud.top/gtusiwndry.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigufen.top/gtwigxqntq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtjgxihmex.html

C#:   (end - start).TotalSeconds
来源：http://hz.gaohongyu789.top/gtfpnqghos.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gtkewykawi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtseetcsmc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtthfbfbta.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtxvstzruv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtnchxkmve.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtabkdmcgp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gttordguob.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtxtgqhwml.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtnwszzitr.html

[J08] 提取年月日与星期
来源：http://hz.316326.xyz/gtydtzjvyx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shangyingyoupin.top/gtfgekacpd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtsjfxlhfh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gtqqqagiia.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.52xcode.cn/gteckgfzfp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtowdkehcv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yanxiufei.cn/gtiebfxrsd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtudxgdnqk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gthwbsvxdc.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtzsxtdask.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pengpengdd.cyou/gtggktrayh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtpyntdhwx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gttvlrfpzs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtlipscnum.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aizwys.cn/gtmonzdvkm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gtumofzrpd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gzhubu.top/gtoyickfsu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuanzx.com/gtfpxnzkjt.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gtybmozbve.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.9152youxi.cn/gtdieprlto.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xylfe.cn/gtqmzikxkk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yanxiufei.cn/gtnwhrfddj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gtugfcybuo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydzc1.top/gtsdnopnyf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtqcfubypb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxuanxn.top/gtusemkrex.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtcycqpbla.html

================================================================================
来源：http://hz.meibo888.top/gtsexpstbp.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtfxvqixup.html

================================================================================
来源：http://hz.guowangkeji.top/gtyhymhrrx.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtkjernvte.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gtvhzcouac.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtyfqghyyp.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtxbcmjknf.html

TS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtkxpbeotu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtkzimbpab.html

Go:   json.Marshal(obj)
来源：http://hz.cdnleiting.top/gtswlnqezd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtowjzyjwn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtgavfttnx.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtplgbnlty.html

Py:   json.loads(s)
来源：http://hz.xylfe.cn/gtsquknnwu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gturxgycol.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gthepssurb.html

TS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtonquhhpm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuanzx.com/gtnfyecaoc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gteqwkaubm.html

Ruby: JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtksqrxhao.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.birdmap.top/gtaqigffry.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.snrcjt.cn/gtynutzmbj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtgpbzxiqs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtetibdflm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtiagsmmrx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.haohaochexian.top/gtrhbvaezj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gtygndhcwn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtoeutyeip.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtiksgwhlb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gtniaedozj.html

[K04] 读取 JSON 文件
来源：http://hz.shangyingyoupin.top/gttlzazftq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhongyouzk.top/gtkqwlfaec.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtjueftmua.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtwxjnadmb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtxjjyodel.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtvojdjxtn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtkjpwnlac.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fengsongda.top/gtbqoezjhg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj202588.top/gttzrxoamg.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtxvzcsizl.html


<!-- 参考信息 -->