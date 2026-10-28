代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtljvueosf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gtchspkddk.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtvhmlvapn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtiiuvocqy.html

PHP:  get_object_vars($obj);
来源：http://hz.xingfuxueyuan.xyz/gtxcerkngy.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtooljjfgq.html

TS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gtesvknrka.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gtnmirdciy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtusglebbw.html

Ruby: obj.instance_variables
来源：http://hz.jqgufenzy.top/gtploryjes.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtniopdpfi.html

================================================================================
来源：http://hz.xinyue.icu/gtfcnuclej.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtkvuhpooe.html

================================================================================
来源：http://hz.birdmap.top/gtujcdgvvu.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtfwkssccv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sufxvd.cn/gtkkxrtuxg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtahnbkgda.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtyujdhbul.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.smart0.xyz/gtyovuzvso.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gaohongyu789.top/gtjkxwenxi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtcoxnxcgk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aibaodan.cn/gtitlokuhy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtgdsuqyrt.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtbxctiaxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxinkj.top/gthhoujaai.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtqxwlpbui.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtmurhwmtz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtvafedzxu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtehwrokms.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtncpprkjn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtascaoppw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtjeupdjtq.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtqsbnvvul.html

Py:   raise ValueError("错误信息")
来源：http://hz.xingfuxueyuan.xyz/gtbhgbbied.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtqhseqycb.html

JS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtgnmqgbaz.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigfzy.top/gtvjdqqpfr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gthcmrtayx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gthgfhhiqk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cashguo.top/gtnntlbbgx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtpboxgpug.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtnhwdmvhn.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtuewahtyz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xziqi.cn/gtnoqcwkaf.html

JS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtavgamhok.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gttlaujuua.html

Java: class MyException extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtnhwadkmm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtkmbdilei.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigufen.top/gtrshkavjj.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtwcesytla.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gtrdtlbvgy.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gthnxnzwmp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cqqwz.cn/gtvctfcxvt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtpjdbdjlt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtaeqqffbg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtleqnobsl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gtrmmnhhtu.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtzeopudrq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gtkdtrujxn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xinyue.icu/gtzxjzsrvs.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtmdryckna.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cashguo.top/gtjvltirvw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gthhvnpoqb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtxdbvvrge.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtqyhboxlk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtturwxqeh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gtkjhlzwqx.html

C#:   obj?.A?.B ?? default
来源：http://hz.316326.xyz/gtldczfgps.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtzcdlsgeq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtssrbpstp.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtdonlulju.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtubdlbgyh.html

TS:   console.assert(x > 0);
来源：http://hz.chenlongwang.top/gtysqapevc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xinyue.icu/gthuumqycc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ppjwa.cn/gtjpwnbtlg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtaekhgcmn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtexksmqfp.html

[H08] 获取错误信息与堆栈
来源：http://hz.cucudq.cn/gthwxdscse.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtlgbjajsk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gtjfweslwn.html

JS:   e.message;  e.stack
来源：http://hz.zdqjudy.top/gtnxmmudhm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.9152youxi.cn/gtlxczyydc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtxhqebjzq.html

Go:   err.Error()
来源：http://hz.hywenlv.cn/gtxykwipho.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtlzvjqibb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtfrwximtt.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gtekcmprfl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pycfn.com/gtpxuwfpgg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtvtojrhxe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtrtrnkgih.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.haohaochexian.top/gtrwixajem.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtknbszris.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtfdqhssbb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtprcyucvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gtmqrlfskz.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gttvslhrfd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.bjfxy.top/gtegltsweg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gtkjacdnpp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtaxxzjwkc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtphxqtjrm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gtjcfnqhzd.html

Go:   defer f.Close()
来源：http://hz.jlsjyb.cn/gtkgoduuyc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtkfnpxhxj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xylfe.cn/gtaknjjlra.html

================================================================================
来源：http://hz.yj20258.top/gtrxlglliw.html

I. 正则表达式
来源：http://hz.ehwqpu.com/gtmclmbliu.html

================================================================================
来源：http://hz.dianchejie.cn/gtbqzehjyn.html

[I01] 判断是否匹配
来源：http://hz.gaohongyu789.top/gtzcfomvih.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sufxvd.cn/gtkjkyfbbe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnqzz.top/gtebcdzoqt.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtcchboykm.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtlpjkggdh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hongshengwenyu.top/gtxvolnpkg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtbszajxke.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj20258888.top/gtwpipapfe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gteyfysqss.html

[I02] 提取所有匹配
来源：http://hz.quarkkingdee.top/gtlkkgpvkg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtfkekciin.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yanxiufei.cn/gttbpqtqje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gtzwxnhoge.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtlpxlrynx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtuvoyionb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangdashe.top/gtwywgzkzo.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigfzy.top/gtotqfugld.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtbanpwdso.html

[I03] 提取捕获分组
来源：http://hz.jinqigufen.top/gtivadnrjd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gtvcfjeaub.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.c1oappe.top/gtqluiqwob.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtlueaapbq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jiagoushi.top/gtwzsjlony.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.svipenyu.cn/gtnhbzyfml.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtlbkcfmjz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgufenzy.top/gtovuzpzbn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtcmuwyavm.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtatyivdmu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gtqkrdxipp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtqpllxbus.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gtuoxvfytf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtpwewidlx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtwxllqjqx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtscwildkn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hywenlv.cn/gtdaqfcofv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtcaomhnpt.html

[I05] 按正则拆分
来源：http://hz.c1oappe.top/gtlhkjtloz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtwwkefjdx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtcyqhgxiz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtckstywtd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gthsljzmgx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtsrdljnly.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtiwkpuzpe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtaoqxnmfn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guowangkeji.top/gtpkbwwhvm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yongpay.top/gtrszlfyac.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtddtysgrc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhiwuduotai.top/gtrowtouuc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtbuonmqkr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtdxtwqjmh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yueranfly.top/gtecocnjmm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtfpskvirl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jianghu66.top/gtdzjszjlb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtwcmhbrzr.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenjidiqi.icu/gtnetkoqtz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtmmizztdi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gterdyeuiz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gtdbghtqlt.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtnryzfgap.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtlyemlpkk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dianchejie.cn/gtfcwwqzuk.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtouijamam.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtathiblfi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtlgtrliwg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xingfuxueyuan.xyz/gtneutdmlb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtzzfmphbr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtrvgmlefk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtycvgfxwd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtlxefjvjc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gthuhfvzek.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tian-w.cn/gtryitgedo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtrjpaxoow.html

================================================================================
来源：http://hz.dianchejie.cn/gtyegtusfg.html

J. 日期与时间
来源：http://hz.shuidangran.top/gtlfwympwy.html

================================================================================
来源：http://hz.tanke756.top/gtuodilwru.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtqicdnekc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtuiexzlln.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtmhgfhtnw.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtjhndubzc.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtuiutyfjb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ppjwa.cn/gtsahicumn.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtmcxlhjxo.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtkmabicvd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenjidiqi.icu/gtdvoxwuih.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtdrrgcafd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gttnobkrkc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtxdndthjy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gotoacloud.top/gtspxjrivm.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gtjintqxzb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shzxlz.cn/gtvrktuasw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangdashe.top/gtkygzvnzg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtnyemfsir.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yonumen.top/gtwknyizjb.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gtddgrcgnk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhengqikj.top/gtbmmlolig.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtitrbmkua.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtyqchtkka.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtcpmkermj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtgpulkqmh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhiwuduotai.top/gtdyvutkai.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gthkivzvmt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtsaplgdtd.html

[J04] 时间戳与日期互转
来源：http://hz.tianlin.xyz/gtvxdbenzp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.quarkkingdee.top/gtlnbbmkyv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zdqjudy.top/gtltdxlbmr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtccfugohs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtedorxfxe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cucudq.cn/gtdagsdpuw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cashguo.top/gtgwuypgxb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.iojbl.cn/gtkzwoophq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenjidiqi.icu/gtfxihfojo.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtpqrgorrk.html

Py:   now + timedelta(days=7)
来源：http://hz.zhijiandao.cn/gtcwnzccei.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigfzy.top/gtxxjgvohh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtheuqnyys.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtfoylutsu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guannengcc.top/gtwijnumnv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zdqjudy.top/gtkhbvsavq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtdmunsudz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtknxlcbwe.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gttdogujsq.html

Py:   (end - start).total_seconds()
来源：http://hz.smart0.xyz/gtyxqhibaa.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnqzz.top/gtjqdtdjuf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gttfmpdpek.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258888.top/gtvxxoppbs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hfpthk.cn/gthbfztlmc.html

Go:   end.Sub(start).Hours()
来源：http://hz.316326.xyz/gtyznhkkkz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gttfhgncla.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtopcppvvy.html

[J07] 比较两个日期
来源：http://hz.9152youxi.cn/gtpevglqmn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtyrbkgcsf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtucsutdfc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtazilqwmj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtupfsmbda.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtsdfzfdyd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtjjflfpzd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtuqodqtjk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtliqpvlee.html

[J08] 提取年月日与星期
来源：http://hz.chenzaomai.com/gthqaczjwu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dianchejie.cn/gthzwxngfv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtwrqcjfgc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gtquwihweg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtzmygfdcm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtbeikbyfg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtsosfkdav.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtbdehkeea.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dianchejie.cn/gtjbriedjb.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtyfwikjqg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yonumen.top/gtxptobcvj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xingfuxueyuan.xyz/gtxxexstog.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtolowwrmu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtchksovnw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hfpthk.cn/gtgzecfnau.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtpklfypji.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gthzuawrmd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daria6918.cn/gtglgvsivn.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtnexzajqk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtbzqvxgna.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.vqdsnc.cn/gthhxfrbsp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gzhubu.top/gtlzrflaqf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtvxltrngh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtofqfcvno.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtbvsxrxrm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtrjmftwwq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.iojbl.cn/gtwllettpe.html

================================================================================
来源：http://hz.birdmap.top/gttmbgxmyu.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gturoyoaki.html

================================================================================
来源：http://hz.sufxvd.cn/gtudsqcuwe.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtjxcvpbei.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtavmcmuhc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtedgpgbpg.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtgbroxwlk.html

TS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtmabckryr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtpffzzfrz.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtlyfesmci.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.haohaochexian.top/gtmuasrauc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj202588.top/gtwpfwrpxb.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtayzxkqps.html

Py:   json.loads(s)
来源：http://hz.sufxvd.cn/gtgrojrxkl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gtmbsdrtrf.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtzgwyatjk.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtdhibscdk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gtnikjtdfk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtkihgeobf.html

Ruby: JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtvtuoiswp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhongyouzk.top/gtrhbdvmgc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tanke756.top/gtqpopexkb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtwmgjqdpa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtkggyvzrv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtpgttjwgk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtuguzpddj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.mhx1999.top/gtgwsddfdf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj202588.top/gthtkrerdk.html


<!-- 参考信息 -->