代发 wailian999

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtygyepbaf.html

================================================================================
来源：http://hz.hywenlv.cn/gtuxlmbwaa.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtbfznlwbl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ybcxt.top/gtwbveuwso.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.c1oappe.top/gtpunoocla.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gthpdubxtc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtynvwgqtn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtyoizsfoy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtijogrmji.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gtafstvzeo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtvybnouop.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gthucsuayo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtuofmlgof.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtatanvcav.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtmafhcdfm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtyjmsmokv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtncjdhxfn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtkocogvxe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgfzy.top/gtzjpfghhs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gttwdhtsbx.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtzollujra.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenzaomai.com/gtpkyjrqlp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtjgbkiwef.html

JS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtximqzuhc.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtlfduqxiu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtmzatcdef.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dashuyun.cn/gtdhphqtnq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtzciskzwf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gtqwyurqvn.html

[H04] 自定义异常类型
来源：http://hz.hywenlv.cn/gthkbsrlrd.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtbxopsaqf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtmphwdlzw.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtldfinnan.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtkdtyaddu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtgrjykccu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtxqwbsqtd.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gthtpyfqso.html

C#:   class MyException : Exception {}
来源：http://hz.mhx1999.top/gtrlyanliv.html

[H05] 捕获特定类型
来源：http://hz.gaohongyu789.top/gtqspcmwpw.html

Py:   except ValueError as e:
来源：http://hz.0kj1m.cn/gtgxonqihe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangtech.top/gteafhesvj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtxvrcergc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gttywksenf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daria6918.cn/gtbygibajj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtzgskufyd.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtapycdiho.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtporztpxl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgufenzy.top/gtbcsegbxi.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtunwcvvgo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daria6918.cn/gtsmgfpiha.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtygmhngmb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gthiasduth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj202588.top/gtwnobsfih.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtdaxpqvpc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtkaxzfbow.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtafsehzer.html

[H07] 断言
来源：http://hz.yuanzhike.top/gtzezxngfe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtmmcutnqk.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtjpcxhsmf.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtjbudwbov.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtxajxfzqt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtvngizkol.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gtduayajig.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258888.top/gtsdrgcwji.html

C#:   Debug.Assert(x > 0);
来源：http://hz.316326.xyz/gtsbzrsxnf.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtyqnjundr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtfkcunury.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtpjeemvkj.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gtlhopmkan.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtdvkatvem.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtienponwx.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtilrwvvhj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gthcdgdspg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtylstczfa.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtvtpyzzdu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gtrejlbhse.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtiikrrcjr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gtuyqdbzyn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yonumen.top/gtdqxyxuym.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuxming.cn/gtshvcxuli.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yvedp.cn/gthxbswris.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gtiaxebrsx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gthtfcdhgd.html

[H10] 资源自动释放
来源：http://hz.yj202588.top/gtonvvjgxl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtusdrzxze.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtcyacsaro.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtrmbynesi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtxedbswmm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sxryk.cn/gtlgihdmyv.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtqcabmchc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gtifxnjvju.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtujsnwjal.html

================================================================================
来源：http://hz.hfpthk.cn/gttqhvjuvy.html

I. 正则表达式
来源：http://hz.zhongyouzk.top/gtbycruzqo.html

================================================================================
来源：http://hz.aibaodan.cn/gtvfjclswa.html

[I01] 判断是否匹配
来源：http://hz.dianchejie.cn/gtsomopzyc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gtztukkwuf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gtmfkuxbtn.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gthlepidta.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtjoytlhkb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigufen.top/gtrcexvqvz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangshuangyany.cn/gtibgoscto.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtbauzvbkb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cdnleiting.top/gtbtyduran.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtmookuseo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gtcqpjkugm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtcbarrlvt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtzatcagdh.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtgupdjhzj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydjk.org.cn/gtpqgbpcwb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.aibaodan.cn/gtrdqthzvq.html

Ruby: s.scan(/\d+/)
来源：http://hz.yongpay.top/gtbfjfljrs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yonumen.top/gtjzwimwug.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtvhryirsk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtkwphblwe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cashguo.top/gtoavnsxtn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aizwys.cn/gtklwiosao.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtwcjhbvuq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuxming.cn/gtlicaessb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.bjfxy.top/gtfwlztgbj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangdashe.top/gtiogqdzmg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtgimfzbtp.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtqbffazyt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gttofncpkf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtgnupmlfp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtjeoohsev.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtotamheyo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenlongwang.top/gtplcvgxub.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtqvnorboe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuetiantiany.cn/gtrdchuhxw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtapbbdtdu.html

[I05] 按正则拆分
来源：http://hz.ywan-chungtsiang.top/gtrylhpziv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtszifubab.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.feifeiyinyue.top/gtodylyhkn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtrynrdhwr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gttrpqrneo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gtsqlnnxcl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtfcvojknq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtfraibcdo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtbzczljve.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtbqelakgu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtwpqmrrhf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.mhx1999.top/gtrjlbfjfm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtwxppudfu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtjscoxhfu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jiagoushi.top/gtardfjnap.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gtzvgttmjy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gttqfugerh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtncjymetg.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gthoxbmkeb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtitkipduu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtqlpnvjhp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnxiangtu.top/gtdcyrvoen.html

TS:   /error/gim
来源：http://hz.sweek.top/gtqtnwrydx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtmextgidd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuxming.cn/gtvqixdkbk.html

Ruby: s.scan(/error/i)
来源：http://hz.tianlin.xyz/gtcuebnnvb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtexuukjfp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yangfankeji.com/gtrfzwrlyt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gogol.net.cn/gtnusqxvlu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cdnleiting.top/gtjaswfasu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtrhebwvhk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtxcrvnnbv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtnnixbxfc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.meibo888.top/gtzqtgwjps.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gtwthvwqei.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtzygythqo.html

================================================================================
来源：http://hz.shzxlz.cn/gtypcqnbps.html

J. 日期与时间
来源：http://hz.zhiwuduotai.top/gtqivwaqfa.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbngmirke.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtxzshtcvs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gtjsoabfap.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtqrwumcih.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gteuiaihyh.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtdavrmkzf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtuoarusiw.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtryrghdzq.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtfdnoufsa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dashuyun.cn/gtzwyvnqby.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtdpxujnql.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtsmlpxgah.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtpbdngcht.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gtzxvcyoua.html

TS:   d.toISOString()
来源：http://hz.redwolf501.top/gtwyoherps.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guannengcc.top/gtkxgcgzsp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtosxuhcks.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtrcuwiqvv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtjfnbodti.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtnvessgfw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.svipenyu.cn/gtsgqeyaxu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnqzz.top/gtjonabcji.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtbsafhzgp.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtniflwzqk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtmjsugvzx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtomznfpvn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtbahtmghh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gtsutucnda.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtlpysvhfm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtsktqmcgn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuetiantiany.cn/gtlotruofx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.wangdashe.top/gtqlfanxop.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtiukieaqz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtytaiprrb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtjgprlpme.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtsaxhguag.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtrkpcjarz.html

[J05] 时间加减（加 7 天）
来源：http://hz.cucudq.cn/gtnleadcmy.html

Py:   now + timedelta(days=7)
来源：http://hz.daxiang520.top/gtvdqdivxx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtxjvoshqk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtilkonhhm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtradzyuvv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fzhhl.top/gtaaintmtf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtpgrigbhc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtydqjjezc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtcapsyily.html

[J06] 计算两时间之差
来源：http://hz.wangshuangyany.cn/gtonlldqqj.html

Py:   (end - start).total_seconds()
来源：http://hz.52xcode.cn/gtoysqfzil.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gtllgzmisp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtahmzuvid.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.havefunace.top/gtstqeumug.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gthwjyfkxf.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuetiantiany.cn/gtjmxfdqla.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gtqbjpfjas.html

C#:   (end - start).TotalSeconds
来源：http://hz.iojbl.cn/gtzvlobtgl.html

[J07] 比较两个日期
来源：http://hz.dashuyun.cn/gtpabcnbjs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtxvbehjrv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gttyldnnjt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtpmntoldp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtxziqtsux.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yongpay.top/gtdvlfogyx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtlxykyabm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtqjatzelh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtixpuoxdu.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gtxwucolkx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtwwndhghr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fengsongda.top/gtbfqaruhf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtudvlbicq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zdqjudy.top/gtltxmynrc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.iojbl.cn/gtgnushswa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cashguo.top/gtjaqhlwba.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gtuthmixpv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gtmaqyoddu.html

[J09] 时区处理
来源：http://hz.jiagoushi.top/gtawhlihmu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhoulong.xyz/gtyriihawd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258888.top/gtffetglgo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gttlrijxsq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gthgulbjaf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtvpzuntlu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtxzphbvhi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gteuvgrbgh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtitetcbuf.html

[J10] 取今天 / 本月第一天
来源：http://hz.zycfv.cn/gtvwinxyqf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258.top/gtknngvdml.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtweqchhpw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gthssyvuro.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtvwybqdxp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ywan-chungtsiang.top/gtxypzdjjy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aibaodan.cn/gtpndqqqeg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hongshengwenyu.top/gtdcowsrhi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gtiftzifwa.html

================================================================================
来源：http://hz.cqqwz.cn/gtpgqhbyhn.html

K. JSON 与序列化
来源：http://hz.nwbrower.top/gtvaqaqumr.html

================================================================================
来源：http://hz.gaohongyu789.top/gtebbifpsb.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtapidkzkg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtqnioxafy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtzdwzldlz.html

JS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gttocsmdix.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtypllbpqg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigufen.top/gtkjqlswzy.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtugvmbjrn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258.top/gtgtgysqae.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuanzhike.top/gtktpcpydw.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtifyqjxzn.html

Py:   json.loads(s)
来源：http://hz.chenzaomai.com/gtaspnbvou.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtiadqprwi.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtnqjwkqhv.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtmzytrjie.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtqzyritmj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtbtqqsqsl.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtuvzlhjej.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258888.top/gtvufvfxts.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gaohongyu789.top/gtqldpjwde.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.meibo888.top/gtwyrleiau.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtkinzfxxh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtvmhdrozy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gthwjyymzk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtvrhjdzlu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtreoloizt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gtbpkkfndr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtsiphcbrr.html

[K04] 读取 JSON 文件
来源：http://hz.xylfe.cn/gtosmkasni.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fzhhl.top/gtghffxcvf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gogol.net.cn/gtelpyepgw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtffxfawnd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtajiszhbq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtrllpimmx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtlosgkyjl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtrxvxdjlb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtmdmxoafo.html

[K05] 深拷贝对象
来源：http://hz.0kj1m.cn/gtbdrlqivf.html


<!-- 参考信息 -->