代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtjapxzdkz.html

JS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtmraudvlz.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtaiudnhin.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jlsjyb.cn/gtfeazzsvz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.pycfn.com/gtaejfyius.html

Ruby: obj.instance_variables
来源：http://hz.tanke756.top/gtvpybjkjk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ybcxt.top/gtojcrbbym.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnqtbsliq.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtjylbbwwm.html

================================================================================
来源：http://hz.andypj.xyz/gtvehcchxf.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtmzylyroe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hammf.cn/gtitaqcmsj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtxygitfjx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtuazzstbj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtixudbbgj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtqaumhlos.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhiwuduotai.top/gthxpsofgl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.havefunace.top/gtgazrbxme.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.haohaochexian.top/gtlvrprilg.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtdsuqgxwd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtnseqbltj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtiydgzvis.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtrqokqghq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtlbyjocrr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtldlyibtn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtnxkcjdsb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.9152youxi.cn/gtzwwgexua.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtvvfhajwo.html

[H03] 主动抛出异常
来源：http://hz.jinqigufen.top/gtprpytvmp.html

Py:   raise ValueError("错误信息")
来源：http://hz.tianlin.xyz/gtqwlacugh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtijtoqbdn.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gttleeqkrd.html

TS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtlwekajsb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xziqi.cn/gttbwaukri.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jianghu66.top/gtaxiiumdc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dashuyun.cn/gtfhhssogc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtfitlmwky.html

[H04] 自定义异常类型
来源：http://hz.ydzc1.top/gtlamdkaby.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtkcmnadey.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtuwgxkbcx.html

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtrygkcufy.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtlpsnsjoz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtzwfewnul.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.vqdsnc.cn/gtpsqenuyh.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gttcevocjo.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtvdonxpwv.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtkpejdfqt.html

Py:   except ValueError as e:
来源：http://hz.gzhubu.top/gtfwfjhckz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtazbzkian.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtrenekoun.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtlvgbadxf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtddxhimtp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ywan-chungtsiang.top/gtzxohdvce.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigfzy.top/gthaoadpxj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtmmxmgeuk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.c1oappe.top/gtmgdxebti.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtilcofzgt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gtqttraqzn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtpwoxiuob.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtybuvkppy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtvkjqbknu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtsanpkvoo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ybcxt.top/gtykguzbbu.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtwyyfvpiu.html

[H07] 断言
来源：http://hz.shuidangran.top/gtubxembvo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtoyjvjwng.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtrkrroznq.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtfdulsqdm.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gteixixqlh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtdakraepm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shangyingyoupin.top/gtnpgieimh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhongyouzk.top/gtmxgmhlhe.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtkpbgfhex.html

[H08] 获取错误信息与堆栈
来源：http://hz.gotoacloud.top/gtufdmupvx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtugiwxqug.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hywenlv.cn/gttikjbfix.html

JS:   e.message;  e.stack
来源：http://hz.fengsongda.top/gtmohmnbcw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtzsmpmmpo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gtvzrqqawl.html

Go:   err.Error()
来源：http://hz.pengpengdd.cyou/gtcfotzaoc.html

Ruby: e.message;  e.backtrace
来源：http://hz.yanxiufei.cn/gtulninkgq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtuaytdsry.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtyqokwhid.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtfkpiwmqf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj202588.top/gtubrosbxg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gtpmzjboqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gttcmyvvtc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.svipenyu.cn/gtaumqbujq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgufenzy.top/gtcavdczgm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangdashe.top/gtjeiozyrr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yvedp.cn/gtchgrgmju.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtvzgclnag.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nwbrower.top/gtvwkrzysd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtammnrsuc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtcyrzaocr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtgrwwbtws.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtnporpdin.html

Go:   defer f.Close()
来源：http://hz.smart0.xyz/gthdnrcxwy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258.top/gtxualuzue.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtznevvknk.html

================================================================================
来源：http://hz.daria6918.cn/gtwmawzjpv.html

I. 正则表达式
来源：http://hz.wangshuangyany.cn/gtlxotnsak.html

================================================================================
来源：http://hz.jinqigufen.top/gtyrlqtomt.html

[I01] 判断是否匹配
来源：http://hz.jlsjyb.cn/gtyqhdorjy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuxming.cn/gtustszuuu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtyaxvmobs.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtvxijdhot.html

TS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtnsguyqgn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtmfxbyjce.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtfdnrxjhb.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtaqwixibo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtvgjwjxkc.html

[I02] 提取所有匹配
来源：http://hz.zhixingplan.top/gtwbmagxkk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.0kj1m.cn/gtnbwbfyjt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtriqpsloc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtctarqrfu.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gttbxoaeyn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtfcgxieuz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.snrcjt.cn/gtppraipxw.html

Ruby: s.scan(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gtgnzynnwc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtwtkefzip.html

[I03] 提取捕获分组
来源：http://hz.gaohongyu789.top/gtnfplomxk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cdnleiting.top/gtdhmytdom.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gtgcfpixvn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.redwolf501.top/gtegaolpqv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtazfhaptq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtwskithvz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ppjwa.cn/gtdltjiehx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.quarkkingdee.top/gtiacrqtfm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtwqbmttja.html

[I04] 正则替换
来源：http://hz.52xcode.cn/gtwexdtjsi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ybcxt.top/gtvqyubrmf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtogcwqojy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtknaudnvi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtmcxrieaq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtgzszrocr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fengsongda.top/gtydvjwbhy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yongpay.top/gtgdufzonk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258888.top/gtparxpwsz.html

[I05] 按正则拆分
来源：http://hz.ywan-chungtsiang.top/gtykeyaovi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtwjbwymme.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gttzqmcyui.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtmqgfnpxq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtcphcsxep.html

Java: s.split("\\s*,\\s*")
来源：http://hz.kuanghao11.cn/gtbazsgonx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgufenzy.top/gtvzryrupc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtnluybuzu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtdiuywsir.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hywenlv.cn/gthyoslhbl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtgpuquiqs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.9152youxi.cn/gtkefbhmtw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtuwvbsrle.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtavnkijsd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gteebqzgkh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ywan-chungtsiang.top/gtnstwrhoy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtkgouijhy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtnjthjomx.html

[I07] 忽略大小写与多行模式
来源：http://hz.hfpthk.cn/gtaebklffu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.feifeiyinyue.top/gtyyseyxnb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtatmuijma.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangdashe.top/gtepcwipes.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtooarusbs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ybcxt.top/gtwrtcjmss.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cheryme.top/gtudfrgglr.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtpequwrip.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gtydlhzvjp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtzqrncxrz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtjalhkdpd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtxskbkmpo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtycvskdob.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtqdahnght.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtdyffcbcs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhijiandao.cn/gtexkorkbb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtggshygak.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gthdrfjjfp.html

================================================================================
来源：http://hz.iojbl.cn/gtdueqvuxw.html

J. 日期与时间
来源：http://hz.meibo888.top/gtlowvvafm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrvfytsjg.html

[J01] 获取当前时间
来源：http://hz.aizwys.cn/gtiabvzhzu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtfoyvwrvo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtlvstbzwq.html

JS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtwtjuxdef.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtqkfvfadu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtwgfmzews.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtuetgejpf.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtwyfcgspp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yangfankeji.com/gtvpltooos.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtrnwilaih.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtmsttrlhj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtlgvpngqw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gtryfvpbtq.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtorbacqfi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhengqikj.top/gtvjtyeebl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.quarkkingdee.top/gtexfnxlno.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtlqeuqtdi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hywenlv.cn/gtoqsnxmfi.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtgylrtqgv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtndplembo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gtqcrckueo.html

JS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtppondowx.html

TS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtklermojp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtmirbumqu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yvedp.cn/gthsvnboqi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gttxdmgarz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gtfrewzxub.html

[J04] 时间戳与日期互转
来源：http://hz.gotoacloud.top/gtjwfnpvph.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.havefunace.top/gtqgscdspq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtqyaotjlg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gteyxafhru.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ivvv.top/gtqhpjpdkk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangshuangyany.cn/gtfvxrzkke.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtdxemlbpa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtfoqjzfwg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtngkqrnme.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gtuvitrzid.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gtrczwkeqe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gteyedobmw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtrvyqlqvz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtgwmsmown.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtycgvytel.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gtytixrzzh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtiigqxstv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuxming.cn/gtxgxtqnqf.html

[J06] 计算两时间之差
来源：http://hz.haohaochexian.top/gtfznxuonn.html

Py:   (end - start).total_seconds()
来源：http://hz.bjfxy.top/gtjgnmbnlw.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtitcohnxd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnxiangtu.top/gthxcbygaf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtrxxmuuho.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gtrcjlqssh.html

Go:   end.Sub(start).Hours()
来源：http://hz.fzhhl.top/gtiiolablm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtbcygsxxm.html

C#:   (end - start).TotalSeconds
来源：http://hz.iojbl.cn/gtxvuepvat.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtolhsexsg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtiarmmnpo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gtcleahxvq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtxpnbwnek.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtouldxmfa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtvbdgcpnp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtlpvfqwke.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtrzexccei.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtsqlvmolt.html

[J08] 提取年月日与星期
来源：http://hz.yj202588.top/gtlyzcrevw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gterglfvhw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtfqpiwjfv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gthiabcqah.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtggrnbtaj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtkusbmdzi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtoxtdjofr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cheryme.top/gtiipiaxkx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fengsongda.top/gtbbijqlqd.html

[J09] 时区处理
来源：http://hz.ydjk.org.cn/gtcwlvjkgm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtiiwdfgof.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtlblkoudq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtsqapmrcz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtprvyplwi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtkvizcyso.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtatozfzyb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtzijrhsak.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtcnwziddl.html

[J10] 取今天 / 本月第一天
来源：http://hz.tianlin.xyz/gtjqyqqufl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtkgnlzgje.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhiwuduotai.top/gtvqsmzlar.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cqqwz.cn/gtevfivoag.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtctrodmyc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shuidangran.top/gtojugfyrr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gtdwnksuwx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtqlnykhpn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtyworlfux.html

================================================================================
来源：http://hz.cashguo.top/gthnhgazhm.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtthywfsaw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxgykcukz.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtdmrxkwgn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtligijvrx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtdfonfnvy.html

JS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtzhdshjao.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtuaasytwb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtzcedmghu.html

Go:   json.Marshal(obj)
来源：http://hz.c1oappe.top/gtrfrfiqkk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtgutlnmfe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtnfxxxkfk.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtgftugchz.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtpolgzxmv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtvuxcmhfm.html

JS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtrxpjzrgx.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtfhurggzz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gtyqlabfbt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtbagzvttu.html

Ruby: JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtspsholmn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtywsgkplh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cucudq.cn/gtlorejkvf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gthmuyroby.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtnobqobzk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtqlexlcvj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cucudq.cn/gtoidimmcn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ywan-chungtsiang.top/gtbmhdvnwa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xylfe.cn/gtmnoseaxs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cashguo.top/gttuaymmrn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gteungpgbk.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtnjigumlq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtesjorjtl.html


<!-- 参考信息 -->