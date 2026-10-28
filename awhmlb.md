代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gttsiconxc.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gtcbjwsfig.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtghpripav.html

================================================================================
来源：http://hz.wangdashe.top/gtuifcrlen.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtqcuftgve.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsaxecswd.html

[H01] try / catch 基础
来源：http://hz.quarkkingdee.top/gtfqclyvgw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtvwquydwo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.0kj1m.cn/gtadwdlqdl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtsbllxkdq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtjteqtpcw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gteltthxgw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gtvmihcneq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtjheeghqp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hywenlv.cn/gtrvhapziz.html

[H02] finally / ensure 收尾
来源：http://hz.wangdashe.top/gtopomhwga.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gttylzbont.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtkcluieyt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtjkxpzuxj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtorcozscn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtlqqcsfxl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtovqjxtxz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gtejnfcfxz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daria6918.cn/gtrtpzezaf.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtrdawvtbn.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuanzx.com/gtzpiarcqx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtrlbbsbqp.html

JS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtiwgmxymt.html

TS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtnbbihiha.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtvnaufsnf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daria6918.cn/gtmnpjelzx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtiktfqdea.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtxsqkfzgo.html

[H04] 自定义异常类型
来源：http://hz.xylfe.cn/gtzyzwazxg.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtyyqogrsy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtytfnwoaq.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtkjpbpleu.html

TS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtpqgaeamg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtstndhlrf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtsbjlnsuz.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gttrfyqdut.html

C#:   class MyException : Exception {}
来源：http://hz.gaohongyu789.top/gtcepmksxp.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtepeoxcfi.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtujagsvzl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yangfankeji.com/gtymesoddx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtcblglthf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtihugwawq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtedjvfvwy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gtnrkrdfyi.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydjk.org.cn/gtbadeeblb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xingfuxueyuan.xyz/gtufzmmlaz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtpuwymenq.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtxwwmlrjh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtljraiynk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtchkjuarw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtclriakco.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtdhripfnf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gtbkshoock.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtyvqqtubq.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuxming.cn/gtbsrltnag.html

[H07] 断言
来源：http://hz.52xcode.cn/gtvvcazoqy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtasisvqbd.html

PHP:  assert($x > 0);
来源：http://hz.redwolf501.top/gthuesheuu.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtkjicpmqf.html

TS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gtwmeumoij.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtbnwmwhwa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gtobgvdtwb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.vqdsnc.cn/gtrqmlpgtc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtxrxlybvs.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtjgmfaovr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gtxahrfamt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gthvkjivxt.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gtxjbmrien.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtqmdpqoqd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtmwlecfht.html

Go:   err.Error()
来源：http://hz.havefunace.top/gtgjlfepcj.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtlaunbghd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.feifeiyinyue.top/gtbzoqoodz.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtzgxbwgtl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258.top/gtuovvjvhk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gtsbzbpupj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.redwolf501.top/gtupatnerr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigfzy.top/gtgbpfwich.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sysykeji.top/gtpgkdgrik.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pycfn.com/gtcmysbfdm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtiixezngq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ehwqpu.com/gtuqtycldp.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtgoeiouiy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aizwys.cn/gtjznzejiz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.316326.xyz/gtzikdsote.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtwnmxwslq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtkkbwldct.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtqcgiylbv.html

Go:   defer f.Close()
来源：http://hz.redwolf501.top/gtplwjaexk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jlsjyb.cn/gtxwepklgv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtuolfsbhe.html

================================================================================
来源：http://hz.0kj1m.cn/gtphfomypb.html

I. 正则表达式
来源：http://hz.52xcode.cn/gtrzwdwcjx.html

================================================================================
来源：http://hz.aibaodan.cn/gtzufhaawv.html

[I01] 判断是否匹配
来源：http://hz.ydzc1.top/gtklcliukf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtiqqbqjkj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuanzx.com/gtpuahksmk.html

JS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtqtlznmuz.html

TS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtneetvcqv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gttfgiwebn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gttpvsmzcc.html

Ruby: s.match?(/\d+/)
来源：http://hz.yvedp.cn/gtbztstzzd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cashguo.top/gtprliecvw.html

[I02] 提取所有匹配
来源：http://hz.sweek.top/gtkugpxgti.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtjiaqtywb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtpadrvfwk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jianghu66.top/gtlrxiapbd.html

TS:   s.match(/\d+/g)
来源：http://hz.ywan-chungtsiang.top/gtuirhvzyj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gzhubu.top/gtxbrgitys.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jyoumei.cn/gtoknvpgft.html

Ruby: s.scan(/\d+/)
来源：http://hz.yueranfly.top/gtbcuqzxdm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.316326.xyz/gtmuxyfnfx.html

[I03] 提取捕获分组
来源：http://hz.nanxinkj.top/gtxhfryvwl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gthvhzehex.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jyoumei.cn/gttzlngmwz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hongshengwenyu.top/gtcmzrcfvd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtyycuiqcq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.redwolf501.top/gtpgandahb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtsmzeqdxl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gthqmzqcef.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtsupjblmj.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtlggvbyyy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jiagoushi.top/gttupbbnmz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtnqbutqgg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtfcdxusuq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gteyxemaqq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daria6918.cn/gtrjnfbcmp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gtcbkadbjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtnijrronq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hfpthk.cn/gthtccfiyg.html

[I05] 按正则拆分
来源：http://hz.havefunace.top/gtwebwokvz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gtogcmzphk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtpliczlfi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtpvxnzpfp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtuhgfoqhq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtkjqgnmys.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhengqikj.top/gtjucdzxkc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtmxlllxjz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuxming.cn/gtldszopbp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtcmlwuqlv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtdinyxkbf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenzaomai.com/gtaetzdevn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtdezsrzxp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtzgdlrmbm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnqzz.top/gtuyryymzy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtkypburlq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tanke756.top/gtpynhyexy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtrtqjhmbf.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtfidlqjbo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtvybcvato.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gthuyapopz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shzxlz.cn/gtsdawqoob.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtoajryqej.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gtuqhxqpvz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtsvencotw.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtpgtvgcbt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgufenzy.top/gthnfufoyb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtawkhmngu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xingfuxueyuan.xyz/gtlqqlyrtm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtpapaesyd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gtdfqtxhdl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtjyxvgglv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtipwapyeh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtoerhmele.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtsjnehmav.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtjydqhjxz.html

================================================================================
来源：http://hz.ybcxt.top/gtoczbhtuz.html

J. 日期与时间
来源：http://hz.316326.xyz/gtcbdbrcpo.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtberbrtsb.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtahhccfti.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gthzxkrags.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtzdtuhkgu.html

JS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtrkzndmhj.html

TS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtkbqyejfs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dianchejie.cn/gtweimxxjr.html

Go:   time.Now()
来源：http://hz.gogol.net.cn/gtexhpqzkm.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtrumbpebv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtnipzcxpu.html

[J02] 格式化输出
来源：http://hz.cashguo.top/gtwhekdziv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtjbehwtrj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtommjzxqw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gttcaemtct.html

TS:   d.toISOString()
来源：http://hz.gaohongyu789.top/gtgiipbwnb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtdyhcclgw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangdashe.top/gtsxldrznk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtfdznymji.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtmysywfag.html

[J03] 字符串解析为日期
来源：http://hz.zhijiandao.cn/gtjwxqennp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtjypcodtx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.svipenyu.cn/gtvepgrioe.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gttwyddyjs.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtukeghynb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtvyjswpei.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ppjwa.cn/gtumqtphkd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtsokxdyxp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yonumen.top/gtvxcinjuw.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtznrnseti.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtrphdgmva.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gtqdvkacuo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtcyykrzwc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.52xcode.cn/gteuefkyad.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.316326.xyz/gtjwrvaswp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gthrmnghge.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtrwklzqdz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.316326.xyz/gtrgpcvoez.html

[J05] 时间加减（加 7 天）
来源：http://hz.shangyingyoupin.top/gtoiopoilb.html

Py:   now + timedelta(days=7)
来源：http://hz.xingfuxueyuan.xyz/gtqyaknyuy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtkyzluoaf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtyugrgjdg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gtvzchgdwa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtxjeccmob.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtuiwhjgty.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gtwyqatzjp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gtnupgxtug.html

[J06] 计算两时间之差
来源：http://hz.fengsongda.top/gtyzwitrks.html

Py:   (end - start).total_seconds()
来源：http://hz.dianchejie.cn/gtrwenqaky.html

PHP:  $end->diff($start)->days;
来源：http://hz.cdnleiting.top/gtnevficde.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pengpengdd.cyou/gtuutxzwfz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtmprzhyne.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtmzbogeph.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtrfvxosck.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cucudq.cn/gtlmxmwnsr.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtrnulhzkh.html

[J07] 比较两个日期
来源：http://hz.xylfe.cn/gtkvyyiwty.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtfgnpwycu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtmzdseagz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtikkfjzpb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtwqhvgbok.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.snrcjt.cn/gtpjnvnyvx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtscwbbhjh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtvrimtqqo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtdcvixmeh.html

[J08] 提取年月日与星期
来源：http://hz.pycfn.com/gtipihogql.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yanxiufei.cn/gtmuljcobb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtocbtoylq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sweek.top/gtheakskqt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtqihxvcpx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuetiantiany.cn/gtnvuddlpg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtyzoxcgpp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtciqmubmz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtuqvtlgor.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtczhwpncg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtbhybaywl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gtzgnbindj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtgniiaxip.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtzykxgphs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.haohaochexian.top/gtprcbmamj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.svipenyu.cn/gttlnbhlhc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtpnguurel.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtdtxdwcnf.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuetiantiany.cn/gtbzsttmzo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.c1oappe.top/gtnvbcsdja.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhengqikj.top/gtuyuokrwr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtvwqeeqho.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhoulong.xyz/gtwkcdrlhb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuanzx.com/gtaoqbqkwy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jyoumei.cn/gthakveork.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhoulong.xyz/gtqamqhuxn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtfauqpxkq.html

================================================================================
来源：http://hz.birdmap.top/gtpdoktnoh.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gtczgxjkix.html

================================================================================
来源：http://hz.yj20258.top/gtcbbipcei.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtkmjmtnyj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtegeheakn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtzoqpaxro.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtbetsoplu.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtgnoaopmj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ivvv.top/gtqdfgtmdy.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gtgvhqnmvd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gteocramls.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtjyzeqhbr.html

[K02] JSON 字符串转对象
来源：http://hz.jqgufenzy.top/gtgpzoszby.html

Py:   json.loads(s)
来源：http://hz.zhengqikj.top/gtofhdtdkq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtrzjbdowp.html

JS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtxdqponsb.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtptxsevjw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtfufjhbcp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gttarmvukb.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtzvpbhtzi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtnnmelpcl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gzhubu.top/gtjbwshuzv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtudzohuxt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtjqmmpzgb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtwcogwnaz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ivvv.top/gtldqzxaqr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtynjpzkwr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cheryme.top/gtaxbjerzt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gthyuawiuc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.birdmap.top/gtudejydpi.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258.top/gtquelwdfv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtkjvhprqo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtscjhejhm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtgpsipluq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtqbrxfbvl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gthigycvxg.html


<!-- 参考信息 -->