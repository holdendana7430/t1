代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtfeipgwzw.html

Ruby: obj.instance_variables
来源：http://hz.andypj.xyz/gtenntyflh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtwkbwdckk.html

================================================================================
来源：http://hz.jyoumei.cn/gthnsntbuy.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtntmsosxo.html

================================================================================
来源：http://hz.yj202588.top/gtadjywrsx.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtqoisehjc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jianghu66.top/gtgsaehpgx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guannengcc.top/gtuewkcoqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtxlrlfxuq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gtijackhts.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtjiutpxea.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtwpsdqknz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtrsyxunvn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tanke756.top/gtodnmvqnb.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtsiycvrfe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxuanxn.top/gtrsalmtiu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtxcdchhyy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gttqweyntc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtyqgpymha.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtnhurwhjk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgfzy.top/gtbjsbvzgo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtvprhbwjf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gtduvzgyqb.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtnxbfezfx.html

Py:   raise ValueError("错误信息")
来源：http://hz.yvedp.cn/gtdhmiwlgw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtjvexyemz.html

JS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtxlppehum.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtbuaxjdrq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtxvwvlnth.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtamyrgqjm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtiebqyxtu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtlzncofrr.html

[H04] 自定义异常类型
来源：http://hz.meibo888.top/gtsncqgivr.html

Py:   class MyError(Exception): pass
来源：http://hz.fzhhl.top/gtvrvozpig.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yonumen.top/gtunlitqbj.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtxwosahcq.html

TS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtcwoydshs.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtmiqrkipf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtowulmvgf.html

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtdqolbprk.html

C#:   class MyException : Exception {}
来源：http://hz.tianlin.xyz/gtxhieropr.html

[H05] 捕获特定类型
来源：http://hz.zhiwuduotai.top/gtqctpxsen.html

Py:   except ValueError as e:
来源：http://hz.zycfv.cn/gtlgxnwljb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtdfdrsazl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtxhjpdezr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtegwerzin.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.havefunace.top/gtkwctunio.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pengpengdd.cyou/gtjnbrwaby.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtkmcelcxz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ppjwa.cn/gtsfwxkplz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtrjijprwc.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtkjpvspat.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtmdfvqagg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtpmxxaopq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtiitajnuo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jlsjyb.cn/gtcgjjdwyu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dashuyun.cn/gtqaczxnlv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.0kj1m.cn/gtkkwfdqvv.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuxming.cn/gtgroivnkg.html

[H07] 断言
来源：http://hz.meibo888.top/gtowtzjihk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtwglvnsxd.html

PHP:  assert($x > 0);
来源：http://hz.chenlongwang.top/gtcewahlns.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtdhlqzdqg.html

TS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtwazkgszx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtbjoliiqn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtdnpormvq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtixfjbpfp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtkewvzuig.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtjlzaeeam.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shuidangran.top/gtnxiyziex.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gttltsbxxe.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gtreripwrh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtnrnsunhn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhoulong.xyz/gtkcitysav.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtodttkaia.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtgedsgksp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenlongwang.top/gtghfophcl.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtwwaftqew.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guannengcc.top/gtvqapgyfo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gtktueafic.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xinyue.icu/gtcrwcyaid.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuanzhike.top/gtwgzhpyiu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sysykeji.top/gtvopitmno.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.c1oappe.top/gtyrjttazz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gtobnzfepj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.svipenyu.cn/gtkmyraogi.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtpizwutur.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yanxiufei.cn/gthklunfdf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtibjtkkgx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gtzlmmyzzf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtladuhylt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtjhsvdueo.html

Go:   defer f.Close()
来源：http://hz.mhx1999.top/gtoqvukwlx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.havefunace.top/gtmvozkwau.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.mhx1999.top/gtvypsojyu.html

================================================================================
来源：http://hz.ybcxt.top/gtwwzfhwyf.html

I. 正则表达式
来源：http://hz.xuetiantiany.cn/gtgrytxxiw.html

================================================================================
来源：http://hz.dianchejie.cn/gtdhymlere.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtfvihesnt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtupiqazyx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtbperbpzm.html

JS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtflrwbego.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtcsixatoi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gthrhnvrbr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtpuzyozrl.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gtramwcczl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtqafkuutm.html

[I02] 提取所有匹配
来源：http://hz.316326.xyz/gtqhknnsph.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtmkdhztos.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtzsgoemvt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.52xcode.cn/gtmarvgpfq.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtfpdrrvqz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fzhhl.top/gtzglnhzua.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtnlcpcvrf.html

Ruby: s.scan(/\d+/)
来源：http://hz.gaohongyu789.top/gtxlvlxmvo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gteacltall.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtndejadgx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sweek.top/gtfvyjavcx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ywan-chungtsiang.top/gtgoagqggw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtcyfvvhwl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hongshengwenyu.top/gtoregunxt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtnyzwfxcd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtsctptdtl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gotoacloud.top/gtyejyvrbi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xylfe.cn/gtapkgyiuu.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtkgctawzp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nwbrower.top/gtkhfwogqy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtljxfnwut.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtvgfkzoqs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtimjkspkb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.kuanghao11.cn/gtyptrtpqv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtlcyzqxho.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.svipenyu.cn/gtkdtfgouj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuxming.cn/gtwrrprwqq.html

[I05] 按正则拆分
来源：http://hz.nanxinkj.top/gtimkvgqvl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cheryme.top/gtrhumpsby.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxuanxn.top/gtszjtwbkm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gttcjnqrlq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtqajfrzvh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.mhx1999.top/gtnwcsvwoc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtdsgauhod.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtudaktqpl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydzc1.top/gtiqqwwnjl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.iojbl.cn/gtycdjhjms.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtoxnwxayu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtjwnjjgml.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtpbzffdek.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtyaxkpyxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtpfawzxst.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gteuwnpzvf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj202588.top/gtawojtdiw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtuqjtvpgk.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhaomingkeji.xyz/gtsycruicu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhiwuduotai.top/gtxfeipxor.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sysykeji.top/gtthxqefzu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gotoacloud.top/gtobzfdndq.html

TS:   /error/gim
来源：http://hz.jqgfzy.top/gtvooznjuc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yanxiufei.cn/gtbckixdkv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuetiantiany.cn/gtcqjwopna.html

Ruby: s.scan(/error/i)
来源：http://hz.hnxiangtu.top/gtixfsbcoo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gtcowifnck.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gthgageksl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gthzhtyttn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aibaodan.cn/gthdioljri.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtupbhfxxl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtlcavhytw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtdwsrvmqc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ywan-chungtsiang.top/gtqyxzkhoo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.andypj.xyz/gteasgpjnp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yuxming.cn/gtkogayhmk.html

================================================================================
来源：http://hz.svipenyu.cn/gttdwacwwl.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gtzvndgdgp.html

================================================================================
来源：http://hz.yj20258888.top/gtewdeqjef.html

[J01] 获取当前时间
来源：http://hz.jinqigufen.top/gtdfckqmiy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtdwcexoco.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtmzttpodn.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtqntllyyk.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtbhnbawpp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtoftkewef.html

Go:   time.Now()
来源：http://hz.nanxinkj.top/gtjgyyycsj.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtzxzlqqgj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj202588.top/gtlipvegrj.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtsdfjfevp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtqbnmspfq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtcuioiiox.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtmnxcbhqw.html

TS:   d.toISOString()
来源：http://hz.nwbrower.top/gtlethhqfl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxinkj.top/gteurwugrt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fzhhl.top/gtmmjlahue.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gturuhvald.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtedkbiwoj.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtkwywzmcb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtizlddabh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gaohongyu789.top/gtdcxzgmwq.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtdkxrutay.html

TS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtpzggseyt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtfjxftkxe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtkwzoisyj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtqcfqvvgn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtskqfjzxw.html

[J04] 时间戳与日期互转
来源：http://hz.tianlin.xyz/gtrcrvsbtx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gtthehdywh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtrtosqflv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtexkibfvj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuanzhike.top/gtdjjqqfby.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ehwqpu.com/gtljhzsqwd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtzvsalvnl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.quarkkingdee.top/gtorsewxms.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydzc1.top/gteexiuzvo.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhijiandao.cn/gtmslmnmia.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtnopphplu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtmvosvjvo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtmnbbhdcf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtylwpikzp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gtvwyzzkvq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258888.top/gtkoeadomm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tianlin.xyz/gtuzsneqak.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.birdmap.top/gtwgsxxfqm.html

[J06] 计算两时间之差
来源：http://hz.yueranfly.top/gtmcckjnfx.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtzuzutouy.html

PHP:  $end->diff($start)->days;
来源：http://hz.svipenyu.cn/gthgxkwyaz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gthxtrcpvq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ybcxt.top/gtjdxwhofk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hongshengwenyu.top/gtdrqfpyed.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxinkj.top/gtxvievonl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtjeegcawt.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtmzhlosym.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtqcywvzsa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtzcmsybyn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtrumlupfg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtxzmatvtj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtowhdcvfo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtctngcoff.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtkqfvgkip.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtemgcihdu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtvckccbvj.html

[J08] 提取年月日与星期
来源：http://hz.dashuyun.cn/gtzegrwbol.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtpcciwbnl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ybcxt.top/gtvocpsegh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhijiandao.cn/gtkonmzfik.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hysaishi.cn/gtsurigfij.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gotoacloud.top/gtvjaiiikw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gtcslmbptp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigufen.top/gtoxckyyya.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtthhpfikc.html

[J09] 时区处理
来源：http://hz.snrcjt.cn/gtyxhsxanx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gtfugzsmca.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shzxlz.cn/gthuxiavly.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtnjmqsipg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtqkqwiuxv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cashguo.top/gtvkcanosj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtwvyoxfzw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gogol.net.cn/gtdbnlvrzm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtfysvcqkq.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gtnwaprvuu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtwhkbkrha.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigfzy.top/gtdmxkirqr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hfpthk.cn/gtkqtrygix.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtskghaoxv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cqqwz.cn/gtnliuzgqp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gaohongyu789.top/gttxfvalsv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gtgbtpyoug.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtwvhitoya.html

================================================================================
来源：http://hz.gaohongyu789.top/gtcyiofpsh.html

K. JSON 与序列化
来源：http://hz.cheryme.top/gtfukafjog.html

================================================================================
来源：http://hz.bjfxy.top/gtfhnntbjj.html

[K01] 对象转 JSON 字符串
来源：http://hz.cashguo.top/gtfydsbdka.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtiwasgynu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtrkxboprv.html

JS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtadlnutjr.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtjbittwwc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtbkjlydah.html

Go:   json.Marshal(obj)
来源：http://hz.cashguo.top/gtnqaxuyni.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gtwpvqutrm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xziqi.cn/gtbausxdgu.html

[K02] JSON 字符串转对象
来源：http://hz.hywenlv.cn/gtgxmgiztq.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gttzurbjam.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtsssfejeu.html

JS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtuawqlrau.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtckfbzknr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daxiang520.top/gtqrizruor.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtzpcgmniq.html

Ruby: JSON.parse(s)
来源：http://hz.andypj.xyz/gtqcxcxvzz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gteeehyyfm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtkvyqagtp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtxlolqzns.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gticzafpnx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtxruxbzwe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtkglyhnki.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yangfankeji.com/gthegyumno.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtyqukxkpz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gttppapxyr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtqvmqtafb.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gtzvgngwkd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtwsviamuv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yvedp.cn/gtlcirrwwm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtngyvwdhk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtupokpyqk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtnfuwxske.html


<!-- 参考信息 -->