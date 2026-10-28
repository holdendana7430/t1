代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtfweurjkb.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gthrwhvvim.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tanke756.top/gtfxpdoacz.html

================================================================================
来源：http://hz.c1oappe.top/gtpkbjaojc.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gteyewcayi.html

================================================================================
来源：http://hz.yj202588.top/gtqwvpvgaa.html

[H01] try / catch 基础
来源：http://hz.gzhubu.top/gtncsuweat.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenlongwang.top/gtlikqqvso.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtsihiztua.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtmgffwsqn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtnrskpexb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fzhhl.top/gtxtrtnyta.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yangfankeji.com/gtvdhsqikv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daria6918.cn/gtgacxjmom.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtmuprijqr.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtqtpwaxjr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtbgxqzfxd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtsljcystd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gttnajlipl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gttmtwdqdc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtuvtwrdyx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cqqwz.cn/gtjyhurblj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtlvfyntkp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtxkraqlby.html

[H03] 主动抛出异常
来源：http://hz.jinqigfzy.top/gtcacbwakt.html

Py:   raise ValueError("错误信息")
来源：http://hz.sysykeji.top/gtxamqvjyk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtburxfcmv.html

JS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtcxjgvcvw.html

TS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtunvhengw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtjnjqomdl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtadumrlqa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtxeanaiie.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtrrfxryhl.html

[H04] 自定义异常类型
来源：http://hz.yj20258888.top/gtixxmdfjk.html

Py:   class MyError(Exception): pass
来源：http://hz.aizwys.cn/gtszddyvwc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtnjdfoxue.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtlubbbfxw.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtgkyezsla.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtlpdzrqtq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhijiandao.cn/gtfuesebyb.html

Ruby: class MyError < StandardError; end
来源：http://hz.hysaishi.cn/gtrrwvbglh.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtxtrfkkcn.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtqxhfigxh.html

Py:   except ValueError as e:
来源：http://hz.nanxuanxn.top/gticvrxwse.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtivkyxalk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtsdvfxpwp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gthzvamalm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.haohaochexian.top/gthlmwmumb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gtotpsruip.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtclqheims.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gtpvcyxfbz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtzjqyiaxm.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtvcrcjwxb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhixingplan.top/gtbburjyrl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtmxpmtkqw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtlodhopkv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxuanxn.top/gtfzluftws.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtpwaayjyg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtoqbijrjd.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtlfyqdych.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtdgadmuvz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuanzx.com/gtemaaqoel.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtohqyanny.html

JS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtapdghscs.html

TS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtzovmtjdk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtwsljlond.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtjmenamaa.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gteifouroy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gtkbcljtoc.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtbludnwxi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtcydnjlne.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangshuangyany.cn/gtugxooepc.html

JS:   e.message;  e.stack
来源：http://hz.quarkkingdee.top/gtwtweqcxg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnxiangtu.top/gttzuebgts.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtsmufvdun.html

Go:   err.Error()
来源：http://hz.316326.xyz/gtoudwksyi.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtfjfxtgjb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenlongwang.top/gtaxlvsube.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtgncvvyxk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gthmqlibuh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtmcqeymtp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhijiandao.cn/gtoseomgao.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtgsmdgyjf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangkeji.top/gtnwuvuaut.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigufen.top/gtwneejdvr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shuidangran.top/gthhzdoxyv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daxiang520.top/gteimgcfpy.html

[H10] 资源自动释放
来源：http://hz.hnxiangtu.top/gtejmculfi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hfpthk.cn/gtolcnefnd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtyzlglfbs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtmbrjfctr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtvclpywgl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtjmwqetbp.html

Go:   defer f.Close()
来源：http://hz.yanxiufei.cn/gtfreeujbq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gthgxehimk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gzhubu.top/gtwyurbwmn.html

================================================================================
来源：http://hz.9152youxi.cn/gtfpbyocou.html

I. 正则表达式
来源：http://hz.wangshuangyany.cn/gtkwwifgwv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gttfffwnva.html

[I01] 判断是否匹配
来源：http://hz.daria6918.cn/gtpdwrcxhh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtdifouqzy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangtech.top/gtqmprqcma.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gttftkurim.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtpyukhrlf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtlqpvozgi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtkiexilsv.html

Ruby: s.match?(/\d+/)
来源：http://hz.gaohongyu789.top/gtvtmjfovq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hammf.cn/gtgozwqlay.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtxkgzjxlq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nwbrower.top/gtaemxjmtk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtcvkzxmvq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtmzpybrlq.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gtqoaipowh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtgteuvtkz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gotoacloud.top/gteacrlmve.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtbodyjyyu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtxowznvwc.html

[I03] 提取捕获分组
来源：http://hz.yuxming.cn/gtvrovpgxo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtixahqhxl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gthnwfgfem.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtkfcdlzoq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hywenlv.cn/gtvcizeaya.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gthuzsfcvk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gtvjtufsuw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtyrccilop.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtuvvwleux.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtskioulxc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haohaochexian.top/gtgkfujxuq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtmqrweljg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtneyntton.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtpkidszez.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gttylyxjor.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zycfv.cn/gtyxlkgjst.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cdnleiting.top/gticdwjzow.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fzhhl.top/gtoaepaxsf.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtaemxyxii.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gthiwevrjf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jyoumei.cn/gttfhyfdsf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtgoqjvgvd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtkopbuxex.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtwubqpjdp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.mhx1999.top/gtwelnvwcu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtutrbjmnt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gtmjqrxsln.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydzc1.top/gtmwszilca.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtgpnixhax.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtjudkcouc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtbosgqrqo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtyxczvjef.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gteldwnitg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangtech.top/gtihgunxdn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtqkxghsqq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gttvixkmjq.html

[I07] 忽略大小写与多行模式
来源：http://hz.jianghu66.top/gtbbxkqiuf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gaohongyu789.top/gtxmdzefou.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtzujjoaqh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sweek.top/gttyuzdrmn.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtjxmswycn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jyoumei.cn/gtlpqiaxoa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtkcqoiggi.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtlcgywdmo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guannengcc.top/gtkrqmjqlb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nwbrower.top/gtibydgwyx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.smart0.xyz/gtktkfizwa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtkrohmfwi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtdzylxpzq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtyeqkbsmc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuanzx.com/gtyvqckydo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtvavwncxe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sysykeji.top/gtndkapfiv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtywebnydu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwuukxgya.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtapdiokxb.html

================================================================================
来源：http://hz.yongpay.top/gtrnhccvut.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtwuiubfbs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cashguo.top/gtyxpyoasn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtmipfnget.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtrvwhtijg.html

TS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtgpoggmyt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sysykeji.top/gthawodbmm.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtszfsjwhq.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtygrfllop.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgfzy.top/gthdmtrfky.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gtfashrlbl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtqcyctszg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtemhiqsnv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fengsongda.top/gtrjitelms.html

TS:   d.toISOString()
来源：http://hz.yangfankeji.com/gtwvculyey.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtoubvudfy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtbitbnydp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtkedkwieh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hongshengwenyu.top/gtdddwqdkb.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtvltxkcjw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cdnleiting.top/gtpluvtctd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gogol.net.cn/gttzhcvmtl.html

JS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtyhnrkbmp.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtxovoxozm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sweek.top/gtjeazoody.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtuybqckvg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtyvspgqnh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtqymlrcbw.html

[J04] 时间戳与日期互转
来源：http://hz.hnxiangtu.top/gthdbsgkfr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtdiivzyhc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gtlccrfyvc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtlzvxjbtk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pycfn.com/gtckematzc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhongyouzk.top/gtewaommbg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gtjcknpgbn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gterkvnury.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtkdwtbjsc.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtwboeksdw.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtjkflkmxk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gzhubu.top/gtsppffqla.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtpnnxbmxk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtenzyongu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtinimafcp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydzc1.top/gtvxbuthox.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtddjdmlek.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.feifeiyinyue.top/gtlgavwwtc.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtprqonosf.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtlziiewbe.html

PHP:  $end->diff($start)->days;
来源：http://hz.smart0.xyz/gtjvxplofu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtdfrqwsli.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yongpay.top/gtuxtistzl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hongshengwenyu.top/gtfmyhgykw.html

Go:   end.Sub(start).Hours()
来源：http://hz.fzhhl.top/gtbfiagxsr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangshuangyany.cn/gtoyitfaih.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtfsojxlox.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gthumwcsuf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtmjaiykge.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtdnvpjfie.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtrjoavmhp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtfsrlwaoo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cucudq.cn/gtbqboybcm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gttcvocjkj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtvrauhjej.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtvejlwhcf.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtdrahjtce.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tanke756.top/gtcunprbsg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtlwyenrah.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258888.top/gtbzuukxqi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.c1oappe.top/gtwzwfcimp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtdfgycgrp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangkeji.top/gtbyipojtp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxuanxn.top/gtxtcokfls.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtvzyioqfk.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtbldqigii.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtmyeknoqt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtirmkuckn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtngcxfjdx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtxwlwjjjw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gtkumoogee.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shzxlz.cn/gtxvwmjnpr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtfijxxtnc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.pycfn.com/gtaxhqimhp.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gtmbklsotk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.c1oappe.top/gtcpxghskw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtjdpmjqtj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuanzx.com/gtnstcvjrd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtwtllyuvr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258888.top/gtuzvpzloe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sufxvd.cn/gtzgpfuvaw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258.top/gtglrfeyir.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhengqikj.top/gtulrzahoj.html

================================================================================
来源：http://hz.zycfv.cn/gtqkcgkspg.html

K. JSON 与序列化
来源：http://hz.sxryk.cn/gttljdgwyr.html

================================================================================
来源：http://hz.dashuyun.cn/gtqmxocqmz.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtmjmgvjnj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtbidtjnsx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtdwfjihxc.html

JS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtvwcrnkfo.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtydxaojny.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gtltofswvp.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtbltijyqa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydzc1.top/gtjkfspruh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtbxcrcjho.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258888.top/gtmratutty.html

Py:   json.loads(s)
来源：http://hz.sxryk.cn/gtsuhhmoer.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gogol.net.cn/gtevsfktqw.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtgavbhves.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtklmqywto.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtiapeqqcp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtacgeuggf.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtsauceyir.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gthebxmfgf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtipbameon.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtctllcfks.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gthsdqhelq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtjbgnaluf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtjwnuflaq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtdbfoebqy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pycfn.com/gtspkqpzcg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtmaowdpmg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhijiandao.cn/gtbigpuzre.html

[K04] 读取 JSON 文件
来源：http://hz.yj202588.top/gtjjkhenhk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxuanxn.top/gtzfijxnyj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtgmvaleap.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtzjtxbaeu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gttfyllrbw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtaophapvm.html


<!-- 参考信息 -->