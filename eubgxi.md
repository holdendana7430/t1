代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtixscqmvc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtljxxsfny.html

[G16] 对象转数组 / 字典
来源：http://hz.smart0.xyz/gtzvqkjrda.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigufen.top/gtjrbdeslf.html

PHP:  get_object_vars($obj);
来源：http://hz.chenzaomai.com/gthsnuzqqa.html

JS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtysolilmb.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtijqxvzpd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tianlin.xyz/gtjldkcscy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtjoxnwpfy.html

Ruby: obj.instance_variables
来源：http://hz.feifeiyinyue.top/gtnycvrmil.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tianlin.xyz/gthlucjwjw.html

================================================================================
来源：http://hz.yj20258.top/gtbkctbtfr.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtrxjsjjhl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxqknnowy.html

[H01] try / catch 基础
来源：http://hz.ydzc1.top/gtqzjahxuv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gtglxwdjuz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtkofwgysh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtmfqmnpbb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pycfn.com/gtxuzugfgd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gtsvcfshcn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtuzaagmoc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtuvanhdwt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtvkehekcj.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gtjelhblsv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xinyue.icu/gtgdkqnisb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtiwmwjfqj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtsftyfeyr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtsvzbhfmb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtoudwzehh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gogol.net.cn/gtznagrmex.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtpdcvttbc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fzhhl.top/gtcbtagrcv.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtomawefsj.html

Py:   raise ValueError("错误信息")
来源：http://hz.shzxlz.cn/gtfmtbrtfw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtcudwqxry.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtfqwbhzxp.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtundqsvjb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtyypfybds.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gtojqllvub.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuxming.cn/gtswejtmua.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtkhxpclkg.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtudilyskb.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxinkj.top/gtdkestbel.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtizstnukf.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtprywunyy.html

TS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gttfftcbpt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yueranfly.top/gtmdpdrrrx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtaxzzjuew.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuanzx.com/gttjsxrtdw.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtshhqlvhp.html

[H05] 捕获特定类型
来源：http://hz.zhiwuduotai.top/gtagdvcfmi.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtizyzneey.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gttxmclaaa.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtxmcgvjhc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtoqdkponr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.andypj.xyz/gtjygfbbxy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtkendvgkl.html

Ruby: rescue ArgumentError => e
来源：http://hz.ybcxt.top/gtaygwopdu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gaohongyu789.top/gtzgvetvfi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.feifeiyinyue.top/gtcczmngdy.html

Py:   value = d.get("k") or default
来源：http://hz.smart0.xyz/gtnucmbvda.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtwwqiaimz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.svipenyu.cn/gtuqvfrihq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtqlpmxjnd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtcbdihvzk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dashuyun.cn/gtwqrcrwjr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtbxmgmzgq.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtsccsrznf.html

[H07] 断言
来源：http://hz.sysykeji.top/gtzwjcwarr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daria6918.cn/gtjfdnugjj.html

PHP:  assert($x > 0);
来源：http://hz.jianghu66.top/gtzguqtehz.html

JS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtjsnqjduo.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtmakdwnrw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtepoiruit.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yvedp.cn/gtlotffwoq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shuidangran.top/gtshqbcchi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xylfe.cn/gtsqlxuomh.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtkeresaep.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenzaomai.com/gtbhdvlfnl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtnfludrhl.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gtwzflhifq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtujilzwyh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtlvhsepul.html

Go:   err.Error()
来源：http://hz.hfpthk.cn/gtphidzbhg.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtpllkyvhm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhijiandao.cn/gtwlsahznd.html

[H09] 带错误码的异常
来源：http://hz.birdmap.top/gtrrhtvspn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gtpiduxtzb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtkynjdcdv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtnptnjqvl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.mhx1999.top/gtqgspdahj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgufenzy.top/gtzdcrdoiy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.vqdsnc.cn/gtvvamgviq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtvgjlgkkz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guannengcc.top/gtjokllgsa.html

[H10] 资源自动释放
来源：http://hz.pengpengdd.cyou/gtiobdbqnt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtomcgvptj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtvwxumqgm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtrzeumotk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtnldkvjni.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gtbyymwcoz.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangkeji.top/gtwojqqsyn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cdnleiting.top/gttzmudhmu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtpnyhyzzj.html

================================================================================
来源：http://hz.jinqigufen.top/gtraqmaqhn.html

I. 正则表达式
来源：http://hz.redwolf501.top/gtnlvkglvn.html

================================================================================
来源：http://hz.yuanzhike.top/gtdyvpcinr.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtwpdowwta.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hfpthk.cn/gteidaepuw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuanzx.com/gtavgwargl.html

JS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtgtoobrxc.html

TS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gteqqvzujm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtlrczlkni.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangshuangyany.cn/gttwoxrxiq.html

Ruby: s.match?(/\d+/)
来源：http://hz.sweek.top/gttjydkmkr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gtskoqgnts.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtopjchhqz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtoghqrhqm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgufenzy.top/gtwqkxytnj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinyuanbaomall.cn/gtpanletfm.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtqyigbrcl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigfzy.top/gtaicbrhef.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtahtnrhqu.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gtaytktwiz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtiekssucu.html

[I03] 提取捕获分组
来源：http://hz.daria6918.cn/gtcubntqph.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtsdlwkjfk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtzvwbhicl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtfobyuvfe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258.top/gtatjbvfzv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gotoacloud.top/gtdwowlbcv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shuidangran.top/gtgxxckwbz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gtuvzjmvcx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xylfe.cn/gthfubgven.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gtqlkqwjci.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtaqpoxtdb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtmcnmsxre.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtliljrsbm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtmkgvifpa.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ppjwa.cn/gtttunscxh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gthzehfmah.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtxoydtice.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yangfankeji.com/gtlvfegbui.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gtlczsliso.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pycfn.com/gtqwutucqs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.9152youxi.cn/gtirzuospw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtykllubak.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtnokrwxnx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shangyingyoupin.top/gtlklocifg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gtxnglegwi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtzldliiyv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtzewtrwye.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgfzy.top/gtgrqwryug.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtieeovlir.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhoulong.xyz/gtvajfsppy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtmqorrmce.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtctheanic.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cashguo.top/gtbrnkqhdw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtftqptwnw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj202588.top/gtuzvqncmp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gthphkxakx.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxinkj.top/gtnsflmknx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtqqwyxfca.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guannengcc.top/gtixzddrwv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtsjmdavxg.html

TS:   /error/gim
来源：http://hz.havefunace.top/gtyiqdipra.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtlurohguc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtovffiipq.html

Ruby: s.scan(/error/i)
来源：http://hz.haohaochexian.top/gtbakcvycf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtozdgpvri.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtfukhwpyu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gotoacloud.top/gttecybxki.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.redwolf501.top/gtpnurcrte.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtskfqrvtw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtjehgiwsf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtdfnwpzqm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangtech.top/gtvgulugoi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtjbmwwhqw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtkqowibfn.html

================================================================================
来源：http://hz.hnqzz.top/gtmryddfrn.html

J. 日期与时间
来源：http://hz.yj20258.top/gtlezzdpow.html

================================================================================
来源：http://hz.hysaishi.cn/gtvqirrpwb.html

[J01] 获取当前时间
来源：http://hz.shuidangran.top/gtsfgsphgs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gtnnybecno.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtexldnnyn.html

JS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gticfabnvt.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtyzswktrx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.9152youxi.cn/gtmtvwztwr.html

Go:   time.Now()
来源：http://hz.aizwys.cn/gtcnwhvwbp.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtxhgqjjxq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guannengcc.top/gtlwygindc.html

[J02] 格式化输出
来源：http://hz.yvedp.cn/gtxdjrbckb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtbvnaxxav.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtctpskbbi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtswnuyfiy.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtihkzflky.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtworcegtd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtmbwqxpwa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gthqcaqvoq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxinkj.top/gtcipmjjfb.html

[J03] 字符串解析为日期
来源：http://hz.jlsjyb.cn/gttabhlwga.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.mhx1999.top/gtqxlxjtqh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gogol.net.cn/gtnrlslqge.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtrzimtbrs.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtjuafjtrw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtfyolpwpc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pycfn.com/gtwkanjydf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtkqvionhe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jianghu66.top/gtuozeujhe.html

[J04] 时间戳与日期互转
来源：http://hz.ydzc1.top/gthgyluerd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtashfnxzm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gtokohxxfu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gtzllxufmf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tianlin.xyz/gtbseitchx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gtpaxbvdvj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.c1oappe.top/gtvgebbjdw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenjidiqi.icu/gtpgyxtowh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtairtedbn.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtjvgoljlx.html

Py:   now + timedelta(days=7)
来源：http://hz.ybcxt.top/gtwoybokde.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtjvcasjeh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtmckhrwwo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtacgucord.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gtayzhmwvu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtydcuiyfw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.0kj1m.cn/gtbipuzhms.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.smart0.xyz/gtkmmsaiwn.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gtctutqoia.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtsydzspcf.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtigylyjfe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gtnucwkshb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258888.top/gtuthtcwia.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shangyingyoupin.top/gteujhzuwp.html

Go:   end.Sub(start).Hours()
来源：http://hz.yvedp.cn/gtqlydpkmt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtrlbjhvcn.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtxxgqjipj.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtkfusbbyv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtrmngxhoh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhoulong.xyz/gtmhpyshzn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtdksdypyt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtyfkarkmz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydjk.org.cn/gtniyduaad.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gtakrsiqvm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtdkyxrzcn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtkmtbekor.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtuouitdnt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gttmqpuqtr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnqzz.top/gtkcpfuekd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.andypj.xyz/gtcldfhdyx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuanzx.com/gtygceuttb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangtech.top/gtepfmjomd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xziqi.cn/gtvegbskib.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtnppcshac.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtupuokfqs.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtuuxtvftu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shangyingyoupin.top/gthmhjdbqh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hywenlv.cn/gtsbitiqjf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtlmxktqpv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtnsvkifek.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtkiubnzzh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtwwqbqrww.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtizldlacr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gtafbmedls.html

[J10] 取今天 / 本月第一天
来源：http://hz.c1oappe.top/gtujcjdbba.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gtrlefkdem.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shzxlz.cn/gtqehmptyl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gtgrrrrwcd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtlreqbebm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtrertdexp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtxgxdqtim.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhixingplan.top/gtgqqvokxm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.smart0.xyz/gtwmfytqqn.html

================================================================================
来源：http://hz.jyoumei.cn/gtoepzsopx.html

K. JSON 与序列化
来源：http://hz.yj20258.top/gthbnrvxzg.html

================================================================================
来源：http://hz.guannengcc.top/gtcwljbyvt.html

[K01] 对象转 JSON 字符串
来源：http://hz.daria6918.cn/gtuikmdcdj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtisvuqsth.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtsbhkyiqs.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtjxyvaigl.html

TS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtfzihdmbh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtmtbrrgva.html

Go:   json.Marshal(obj)
来源：http://hz.ppjwa.cn/gthqjgqarz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cashguo.top/gtpfedlvpy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gtwwumbwjx.html

[K02] JSON 字符串转对象
来源：http://hz.nanxuanxn.top/gtemstegwi.html

Py:   json.loads(s)
来源：http://hz.meibo888.top/gtwqzowmkf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtwvmgiyrr.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtvvhlwgyy.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtnffjlsgp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtqhjrnkko.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtuwplvkud.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gthdkdoshs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xinyue.icu/gtgiqwpslk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtojjtrqzc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtdsrpaptp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtqhdbzkba.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtoglcyzlx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtbbjfirfx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gtwcaqlzrq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gthgqjoedk.html


<!-- 参考信息 -->