代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.zhengqikj.top/gthsthehmw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtrqypvgkn.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtjmjbtdln.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.haohaochexian.top/gtyanoeipa.html

PHP:  get_object_vars($obj);
来源：http://hz.ydzc1.top/gtrufldsep.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtrmtqygrb.html

TS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtgjkpoapj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuxming.cn/gtktkvkqmb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuxming.cn/gtvgumfvfs.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtvwrgrkul.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtscuxgnpj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqogkitaq.html

H. 异常与错误处理
来源：http://hz.ehwqpu.com/gtqlasfogg.html

================================================================================
来源：http://hz.zdqjudy.top/gtyvxblyvl.html

[H01] try / catch 基础
来源：http://hz.xuetiantiany.cn/gtlphcczow.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yvedp.cn/gtcxuznuwo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtqjgzctqz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtmtovjths.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gtcdigrnyd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtggvgjmfy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtupjkcxka.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gtncrwuhjn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtsqcvzybe.html

[H02] finally / ensure 收尾
来源：http://hz.guannengcc.top/gtuloxxpmo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gtvkxxfapk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtkoxszzgo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtbcglqurn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtjixkswdb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtfexxirzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuetiantiany.cn/gtrenjzdqy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shangyingyoupin.top/gttfvxpjlh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtvflltzjs.html

[H03] 主动抛出异常
来源：http://hz.yj202588.top/gtsglfhltk.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtsbyrdnjm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtvmfsaciw.html

JS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtofvefwiw.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtbijmfxws.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtfgmorjqp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnxiangtu.top/gtauwvuogo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tanke756.top/gtlyimhnyh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yonumen.top/gttazedmcw.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtdkivodsk.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtlrvcxqtk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtqtzifgxv.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtzoadpsah.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gthyufpwoi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.redwolf501.top/gtwrbqnxqm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtcuxcmuqj.html

Ruby: class MyError < StandardError; end
来源：http://hz.vqdsnc.cn/gtugehzndm.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtdicltccx.html

[H05] 捕获特定类型
来源：http://hz.chenlongwang.top/gtbpmwnwhq.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtilxkwwjx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtijdfanyd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtmpblgcoc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtcfqgrrwy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtjtmjidpp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtarbkdwsm.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtylqmfquw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ppjwa.cn/gtauyyxygi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtjekerffn.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gtlrijpgrk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.pycfn.com/gticptvsgh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gthwjyvicr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtwnicdfaa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtbogbwbkm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtmyxvatmc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guannengcc.top/gtxhfahpps.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gtvfolhmtv.html

[H07] 断言
来源：http://hz.bjfxy.top/gtwaknbknx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cucudq.cn/gtwpwiasgg.html

PHP:  assert($x > 0);
来源：http://hz.bjfxy.top/gtcgnmpjcc.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtckccfjhy.html

TS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtselfvadb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aibaodan.cn/gtqirqiymb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtjqtjkyse.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtjhudeepu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtihnpsrbj.html

[H08] 获取错误信息与堆栈
来源：http://hz.daria6918.cn/gtowouebqo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sweek.top/gtausghyhq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtmgzqgays.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtcjnddeis.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtwxohwcaq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtaryakidf.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtnafgryvp.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhixingplan.top/gtmjdmyweq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.redwolf501.top/gtswvmalrb.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtqxiqtqny.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gthzjsmhkr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hongshengwenyu.top/gtcinveyyo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guowangkeji.top/gthdycssod.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtjfastpmh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yvedp.cn/gtuhnbjhqc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gtmmhfttbc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtpqhnxmnd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jiagoushi.top/gtlgeownbe.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtctxmrlyi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtaurovyap.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtptipvbxu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtxhnzjqlt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtxdkvivfj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.bjfxy.top/gtnudgtzet.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gteicttsbb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtnridmhqu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.haohaochexian.top/gtizzthgzm.html

================================================================================
来源：http://hz.zycfv.cn/gtqtygdtth.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtkyumuvfh.html

================================================================================
来源：http://hz.ydzc1.top/gtijfazjeo.html

[I01] 判断是否匹配
来源：http://hz.jlsjyb.cn/gthqtgkmnt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hysaishi.cn/gttaxylzor.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtyoqxhufr.html

JS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtphypiahf.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtsgpcdcqr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtpijfcmks.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zycfv.cn/gtnhjfxrsk.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtfqhgwudn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtlrrrnbxd.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtubchknuh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aizwys.cn/gtrgamuviv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtjxdlddxx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtlsflfsdo.html

TS:   s.match(/\d+/g)
来源：http://hz.cashguo.top/gtcnlbkvwe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinghuilouyu.cn/gtcssehdmg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtbafixsfv.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtbjimnixu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zdqjudy.top/gtsolbmhjt.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gtmewaintt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydjk.org.cn/gtfympjztn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258888.top/gtkjeeadfh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtmbazoais.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gttfcthbva.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtrqyukbol.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.birdmap.top/gtavzvyxbq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.bjfxy.top/gtefbrquur.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtpykyjaab.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gtrgynncbp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtelikfxcx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gticmbaagt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtcttqfusc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtyzvazzwl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtriybkuvt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guannengcc.top/gtnfbsaefq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.andypj.xyz/gtvbyfwgdp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yangfankeji.com/gtqufxyhhh.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtagjglfvi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtfqaeqpsr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtnhjmuzri.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtmbuwouyb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtukjvhezn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sysykeji.top/gtbxkdipwd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ppjwa.cn/gtqmdoxgep.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtloaecgnt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtvndpynmu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gtygspxxkm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtbeldsipi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aizwys.cn/gtmmvlgszf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtshhpqqmi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtdwobvnly.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gtgeaemzio.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtdrzybbff.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtmlffkhxy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gttjkevqzv.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtrcuvcbyt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtksjwtqra.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtnhprslwa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtytolcovi.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtttwyodav.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtspxumvfe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cashguo.top/gtilfxarzp.html

Ruby: s.scan(/error/i)
来源：http://hz.xingfuxueyuan.xyz/gtlzopdjza.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtagcdccld.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.haohaochexian.top/gtjcnufwlw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydjk.org.cn/gtkdlpdlbg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtvhjlsoyp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtoozmqqko.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtydafoxdb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtvrzqodyh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.bjfxy.top/gtsbpvzzun.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtulshyboh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtoakkjcvq.html

================================================================================
来源：http://hz.tianlin.xyz/gthkfnsywv.html

J. 日期与时间
来源：http://hz.316326.xyz/gtycyfgata.html

================================================================================
来源：http://hz.hammf.cn/gtldrjjsze.html

[J01] 获取当前时间
来源：http://hz.kuanghao11.cn/gtcuswoqba.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydzc1.top/gtsnvyeodr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtbirimoqd.html

JS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtzmjvgcsn.html

TS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtkukhnfhu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.meibo888.top/gturehhrjt.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtasepajhp.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtjmqokzar.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtglnpxhwi.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtjdowmihg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtzwhekxzv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtrxkmjaae.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gtmpvaoket.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtglbeljcj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gtdprwalkt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenzaomai.com/gtykrqvgyj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gttnehrdon.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtwpgptogs.html

[J03] 字符串解析为日期
来源：http://hz.jinqigfzy.top/gtepjgmyul.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gtaolkykzm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gttrsrlhqo.html

JS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtowvzkwbj.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtdwjxcrxi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtiyafuihi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cdnleiting.top/gtyqoideya.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtnkmmwuno.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dianchejie.cn/gtiirktzxd.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gtpbhymbiv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtnjrgsjjy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtoshhbcgn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258.top/gtyaetysov.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtlvmbqcwr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daxiang520.top/gtsnglmpei.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gtelqyzjhj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtrkudkuqo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtewtawzcq.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gtsuzmoatf.html

Py:   now + timedelta(days=7)
来源：http://hz.dashuyun.cn/gtfbspcdsk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnqzz.top/gtvhawzhrd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtnagxfpvy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtnoyvthjx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtraklhixu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtnklggbdo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtvvhnezrw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gthwhzguis.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtnhjirhgn.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtcrkhrwbw.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtldyludjv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xinyue.icu/gtfezwelcz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gtitvuvavh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtpxenyutd.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtuzhbviyw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtboebbcxr.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtedpnmelz.html

[J07] 比较两个日期
来源：http://hz.chenzaomai.com/gtrcspnqpe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtyqhzusuf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtyegekulx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtajcaftui.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtfehxbtls.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hongshengwenyu.top/gttlbeayof.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtiulwlarr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtbsdhqleo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtyneygnkn.html

[J08] 提取年月日与星期
来源：http://hz.ydjk.org.cn/gtilwyuicn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtcfnsqhtd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zdqjudy.top/gtmynpgxbt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gthfjkotti.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gthteyjxmz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydzc1.top/gturnawfmc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gttjptlkmk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtlbuddbxg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtyohzqyhp.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtujqxzkat.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtgkjafkjj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gteuvfrrzl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtcslfiljf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtvctrfler.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shzxlz.cn/gtbuzvrklh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgufenzy.top/gtqtdfgnwl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gtisasghga.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yonumen.top/gtjnvfpxgx.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gtcekygixg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gtxfgfngao.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gtfhiybeip.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtarzmucma.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtxmdpqngr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtpwvehtpe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtchqvqcjq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtsrbaflkt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtnthbysqy.html

================================================================================
来源：http://hz.fengsongda.top/gtovzklsxj.html

K. JSON 与序列化
来源：http://hz.sysykeji.top/gtaioxhsdp.html

================================================================================
来源：http://hz.quarkkingdee.top/gturiznwkn.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtnkhtsvnm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtmfuebjrj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtljvvjoys.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtzmibogwk.html

TS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtmiwqmhkr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ppjwa.cn/gtyudganlu.html

Go:   json.Marshal(obj)
来源：http://hz.jqgfzy.top/gtfhtuujqx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gthxtizdvd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtnsujqyvp.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gteggstdfz.html

Py:   json.loads(s)
来源：http://hz.ydzc1.top/gtqkhdvrpa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtfenqmsxb.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtutqnceql.html

TS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtuhnbpjul.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gaohongyu789.top/gtpjzsmtax.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtduyhmqly.html

Ruby: JSON.parse(s)
来源：http://hz.9152youxi.cn/gtbkifqoim.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtnvrcmbst.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.0kj1m.cn/gtpmkeunyu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtdzpsxjia.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtxkqauxtx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtpjmhjbvy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtuypdttga.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangkeji.top/gtnyfclbvx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cdnleiting.top/gtvuftmkvx.html


<!-- 参考信息 -->