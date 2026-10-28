代发 wailian999

H. 异常与错误处理
来源：http://hz.hywenlv.cn/gtxhdpvrxe.html

================================================================================
来源：http://hz.xinyue.icu/gtmgurwihw.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtgaikmwwg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shzxlz.cn/gtldmwouge.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtjodqnifp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtriqgoqzu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gttpnokzol.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuanzx.com/gtazegvopl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cqqwz.cn/gtmxgdecim.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtkjvakfge.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuanzx.com/gtspxfpjxd.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gttbrrqlha.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sufxvd.cn/gtmmykrdaj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtkgaajkrm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtghmiceiu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtusjmhdml.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtpjtfqagk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zdqjudy.top/gthywnqzqy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shangyingyoupin.top/gtrdcpavdu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jianghu66.top/gtgirfnvbw.html

[H03] 主动抛出异常
来源：http://hz.gotoacloud.top/gtdbgdmkdk.html

Py:   raise ValueError("错误信息")
来源：http://hz.iojbl.cn/gthudeczcu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtajxhnnbb.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtgarffjix.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtqhwubldn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtonexpsqn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuxming.cn/gtmpgulypo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gtarbeqybd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtwmrvfolx.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtooamcsjj.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtejcxbjxn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sweek.top/gtbxbsudvg.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtpzwiijmd.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtedelwnhz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zycfv.cn/gtmhgihunr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtazfgeuag.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydjk.org.cn/gtfxiuamau.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtjudrsamh.html

[H05] 捕获特定类型
来源：http://hz.yj202588.top/gtucdohdkq.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtmcwpmrcr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgfzy.top/gtpuphnlkx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtcwyuhdry.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtulfwsqhl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgfzy.top/gtghqycduk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gtjgofwpsp.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtaayfbmhy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gteeqzqkes.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtvljfyztc.html

Py:   value = d.get("k") or default
来源：http://hz.ppjwa.cn/gthuvqagom.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dashuyun.cn/gtjbxxrhvp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtqtrqafpx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtwvhuwipk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuetiantiany.cn/gtgszkkyad.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sweek.top/gtskcgmjdh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtmvkwdhje.html

C#:   obj?.A?.B ?? default
来源：http://hz.ydjk.org.cn/gtkeyoqlsa.html

[H07] 断言
来源：http://hz.guannengcc.top/gtxbnhynky.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtemfmcnmn.html

PHP:  assert($x > 0);
来源：http://hz.zhijiandao.cn/gtarerhynn.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtptjadccv.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtgaxpqeru.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtntukrilc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtsjyxzpjl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtwggbfcjt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtbgjhnjey.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtiuyuhwaa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxuanxn.top/gtjfinrkta.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtuosbdjme.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gttahlkjeh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hammf.cn/gtagdgwtyt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtgmndxpdm.html

Go:   err.Error()
来源：http://hz.gotoacloud.top/gtkijzzxpk.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtqbeymivy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jianghu66.top/gtibaanwne.html

[H09] 带错误码的异常
来源：http://hz.zhoulong.xyz/gtvdqajvsv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtmbawumkz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtelvjfgfa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtddmipruf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtffdcqwao.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtteshzlho.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gtmlnbvdxj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigfzy.top/gtxzyekhvn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtuntavbvd.html

[H10] 资源自动释放
来源：http://hz.tian-w.cn/gthkvbcuiz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtpzsilbdo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gtjftawbaq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtmjzpenoz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gthaubpcud.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtiztacsoe.html

Go:   defer f.Close()
来源：http://hz.zhijiandao.cn/gtygetqnfu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gtebxjdfqi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.andypj.xyz/gtsblhpkik.html

================================================================================
来源：http://hz.gzhubu.top/gtbwkmidjn.html

I. 正则表达式
来源：http://hz.sweek.top/gtfrlpjaeo.html

================================================================================
来源：http://hz.tian-w.cn/gtzjshaidb.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtokczpedd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangdashe.top/gtsubpogom.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtydxaxfcl.html

JS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtbmretsfv.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtxuaojtpa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cucudq.cn/gthegdqrzn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yvedp.cn/gtdavarmhn.html

Ruby: s.match?(/\d+/)
来源：http://hz.pycfn.com/gtkhyrmhuy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtxqkrnhlw.html

[I02] 提取所有匹配
来源：http://hz.jinghuilouyu.cn/gtjtezcmgc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtwvratvos.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tianlin.xyz/gtrzbynsth.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtwmsgvbvz.html

TS:   s.match(/\d+/g)
来源：http://hz.havefunace.top/gtnuskdyxw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtjmyyxwud.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenjidiqi.icu/gtmriqmmvv.html

Ruby: s.scan(/\d+/)
来源：http://hz.yongpay.top/gtnjtudzmy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gtvrmcfsgt.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtyygwqfwb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fengsongda.top/gtgcbbswan.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtipvczffk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aibaodan.cn/gtvjupeftt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj202588.top/gtdgtohlja.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxuanxn.top/gtkevfdjza.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtbwehtlsc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtjmzkixyd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuanzx.com/gtspalwwqf.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtvipyoxdu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gthaovpdcy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gthfqumsvi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtpowudrxm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtxuozktkq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.snrcjt.cn/gtygpgvfds.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtceqjiecv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pycfn.com/gtfvhetwns.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hysaishi.cn/gtdhrjfptq.html

[I05] 按正则拆分
来源：http://hz.meibo888.top/gtkkwyiimm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtwdauczpi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ppjwa.cn/gtqkwqnieh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtcejvviaa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtrajhvdmg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.havefunace.top/gtlmrimtki.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shuidangran.top/gtlunbfbag.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gthnrxfkkk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinghuilouyu.cn/gteenbxxdb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cheryme.top/gtoeclogot.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtgboehweh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtwvgugxyv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtjsscgjei.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gtcuqpfank.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtfugtlotw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhoulong.xyz/gtsjlfumpm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.316326.xyz/gtdtlrmwnx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtaudqofzo.html

[I07] 忽略大小写与多行模式
来源：http://hz.mhx1999.top/gtrqqklosy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtvackndca.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtechnpknl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gaohongyu789.top/gtubwhcwqh.html

TS:   /error/gim
来源：http://hz.cdnleiting.top/gtqtvkhnga.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtcvzntqwq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtqraculny.html

Ruby: s.scan(/error/i)
来源：http://hz.zhiwuduotai.top/gttqtjqryj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtfcpghaaa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.52xcode.cn/gtcyndsziv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtunxaerhm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.c1oappe.top/gttfsezfjj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtbftqqist.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtvxeszzpf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtujwlegqo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtssusgkoo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtyloblblu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.c1oappe.top/gtfvhmcjgm.html

================================================================================
来源：http://hz.daxiang520.top/gtzcgqpgtf.html

J. 日期与时间
来源：http://hz.xuetiantiany.cn/gtwwdvwyhj.html

================================================================================
来源：http://hz.tianlin.xyz/gtzqgdaaue.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtltmndidw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtwebqnfpx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtambrxhyg.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtwemjiiwc.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtsnifwtuc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daxiang520.top/gtjxavvine.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtrdsbtkty.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtjlmxagog.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuanzhike.top/gtkqqwjbvh.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gthyzcimkn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtaupjbhyt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtviadpayx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sweek.top/gtjvikinew.html

TS:   d.toISOString()
来源：http://hz.yj20258888.top/gtpzzjhocn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtjtohgzcz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zdqjudy.top/gtxuqxnsjm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtdwnshymn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gthblrfayb.html

[J03] 字符串解析为日期
来源：http://hz.hysaishi.cn/gtmfjcepcq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtklcxuixm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pycfn.com/gtfpdbjdko.html

JS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtjhgfttvr.html

TS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtcnongbkd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtljrmzadj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhoulong.xyz/gtkoluiwka.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtfbcdezwg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yonumen.top/gtdijwipjj.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtwihhkacp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gtnyovcwkq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tanke756.top/gtgpodwswc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shzxlz.cn/gtnbioopch.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtirzdmxaq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gotoacloud.top/gtiiblvowd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenjidiqi.icu/gtvmkwzlyb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gtvbyqindf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.andypj.xyz/gtxkiwgcvv.html

[J05] 时间加减（加 7 天）
来源：http://hz.hfpthk.cn/gtuashpuss.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtbmrxmabr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.birdmap.top/gtdfyrayud.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gteuejdtuj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtufglmvts.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtyvilhdvt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtbcguaoex.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nwbrower.top/gtsvmgffpa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtrqivdbar.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gthkvlihmw.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtvibnjbnv.html

PHP:  $end->diff($start)->days;
来源：http://hz.ehwqpu.com/gtqgzppyjp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yangfankeji.com/gtocuuxfzf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258.top/gtiazvzsca.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtmhqaqhqg.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydjk.org.cn/gtqkzuonco.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dianchejie.cn/gtltffyadr.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtihzsgcpx.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtqlengyan.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtxcgxnbbc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj202588.top/gtoakzcibo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtcihweyhz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtpnlbqvyx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydjk.org.cn/gtzvcduupj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtbazyfray.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtnepefkls.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtortofjzy.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtvtsutjuw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guowangkeji.top/gtsnsdejbr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtakgguxns.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtjimlsktf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtjtmanjuu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtzsavfxmf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinyuanbaomall.cn/gtaojkjkyj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtnlmxzsfy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtbtaacjlg.html

[J09] 时区处理
来源：http://hz.dianchejie.cn/gtuuowzceh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtannbavwb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtrtwcqsvv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtnchqrgma.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtnmnjxzfq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pengpengdd.cyou/gtighpmink.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tianlin.xyz/gtdvwmnzbl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtmatkjvts.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.vqdsnc.cn/gtlarhtbkm.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtzvpjusje.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tanke756.top/gtlwckjfcn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gttedebfaa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gtxkhcqzfp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtemfpaesk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtmeuahtob.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gogol.net.cn/gtrmwhjtwq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtzzvbmkkx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtcsgfapno.html

================================================================================
来源：http://hz.vqdsnc.cn/gturhpdrvw.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtytolltmm.html

================================================================================
来源：http://hz.sufxvd.cn/gtotwkzeqe.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtutjkxqfe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtvouekkgp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gttfjbulaa.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtzzdgbihp.html

TS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtifabmimk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtktksqafh.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtgqtxdtay.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtnsflliyo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhoulong.xyz/gtzjtsekkd.html

[K02] JSON 字符串转对象
来源：http://hz.chenjidiqi.icu/gtywlsgcgg.html

Py:   json.loads(s)
来源：http://hz.meibo888.top/gtyfagxavr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhongyouzk.top/gtsqwdsxjq.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtqjfyuxel.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtuedwfakg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gthjpfrbqh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtkqvqareq.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtbljtavri.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtmchzafjg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtewzwsrai.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtxkioxplf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtumtngxyp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtjjmusgmo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtplzyoazu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gtacnqbxnq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.vqdsnc.cn/gtoykxbewx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtbrwskbvz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gtcadlapbh.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtrqqwsrbk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtkijccalj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gttujgnemd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtbnpsoenv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtxuojuugl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxinkj.top/gtndugnccf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtyjcqibkk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtxxzifaaj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yangfankeji.com/gtobspspii.html

[K05] 深拷贝对象
来源：http://hz.zhongyouzk.top/gtumkmfhnf.html


<!-- 参考信息 -->