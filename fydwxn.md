代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtoailnjms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtiolgjrws.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtqsgyvsei.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydjk.org.cn/gtlazwrvsn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jianghu66.top/gtwtftkgmv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtqrgpkybg.html

[G16] 对象转数组 / 字典
来源：http://hz.redwolf501.top/gtmpzhjfsy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gtggvwgqcw.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtjfwqnwdn.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtpxjfmpdn.html

TS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtkupxblck.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gtxliicnsb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gtjimruzvl.html

Ruby: obj.instance_variables
来源：http://hz.aizwys.cn/gthzgiincw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.birdmap.top/gtqmilrwda.html

================================================================================
来源：http://hz.fengsongda.top/gtyzamaief.html

H. 异常与错误处理
来源：http://hz.redwolf501.top/gtksmppeft.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrlmmxmxz.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtilbslojh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tianlin.xyz/gtqehdrgma.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtbexozzti.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtsftoqzrq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aizwys.cn/gtdkqebgvo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenlongwang.top/gtevxtqqbq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtxvfhhurd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jiagoushi.top/gtmorkkbmg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ehwqpu.com/gtbddjcdic.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gtezdanmoi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtpkoiqitk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gthkyjyjzk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtlrzuwmes.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtaghjovqz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gteipfzmoo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtgxdbsvei.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gogol.net.cn/gtpruevodd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtsgtyxwuv.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangkeji.top/gtatjdmqdw.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtwjmxcivr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cashguo.top/gthywsfggc.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtntwdsdhb.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtkrhrwxrp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtkbbfrokc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gtlqtzleml.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hywenlv.cn/gtizbdrnnt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtiircnmry.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtockkjlbr.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gteapcbhqg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jianghu66.top/gtusqgtvof.html

JS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtmkxxhbro.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtwevifsiv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gttmfakzqt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yongpay.top/gtkgolrtmr.html

Ruby: class MyError < StandardError; end
来源：http://hz.52xcode.cn/gtxsnnhozd.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtukjhbyol.html

[H05] 捕获特定类型
来源：http://hz.chenjidiqi.icu/gtjbmjzsjd.html

Py:   except ValueError as e:
来源：http://hz.pycfn.com/gtnpslmzqx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gtdtnecofd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtlejssmvz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtpmnsdfbm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fzhhl.top/gtxlcgfkze.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtdqmlppkh.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gtycjcvvae.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenjidiqi.icu/gtsuxhvceb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.bjfxy.top/gttzlolclc.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtzydpcpse.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtzvmhnnzj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtlgrqprzk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtrcbuouds.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtppsjhnfg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtyldctvhh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtvogjojlr.html

C#:   obj?.A?.B ?? default
来源：http://hz.yonumen.top/gtfkekaucu.html

[H07] 断言
来源：http://hz.xinyue.icu/gthdezlvgx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cdnleiting.top/gtjdvnnego.html

PHP:  assert($x > 0);
来源：http://hz.nanxuanxn.top/gthlyzkuje.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtasfadjrf.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtjqmhlrhr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gaohongyu789.top/gtvkwfycqf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgfzy.top/gtykqmzeff.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtecqhplae.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtadrygvsv.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gticthxnji.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtsamfhbye.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daria6918.cn/gtngqobrep.html

JS:   e.message;  e.stack
来源：http://hz.nanxuanxn.top/gtagzkbevh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtjgjqubam.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhongyouzk.top/gtbjcghkij.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtfjdrtyxt.html

Ruby: e.message;  e.backtrace
来源：http://hz.andypj.xyz/gtdabbceoi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xinyue.icu/gtmcwieowe.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtfhlagpaq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtvmofqcnz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gtsfqemmok.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtfzyurjpn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gtqzranxhc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtdjbzkvdp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shzxlz.cn/gtwlsnwyjo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.52xcode.cn/gtvxmdparb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtotinzeri.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gtszcpeqgy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aibaodan.cn/gtxccngrjs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtmbigvphg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtjglnpsyc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtnddvhxtc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtkbmtbagw.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gtpncndwmj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtnjshlrvp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuanzx.com/gtlfwjfyue.html

================================================================================
来源：http://hz.sweek.top/gtszmypyui.html

I. 正则表达式
来源：http://hz.sweek.top/gtpcgzrwfe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxwyvkhus.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtxdatvsxt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtufoncspk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtkxzrczsm.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtbbjvcvxs.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtddvewptv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtsvshapxr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gtaxqmvgvz.html

Ruby: s.match?(/\d+/)
来源：http://hz.bjfxy.top/gtuxashudt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cdnleiting.top/gtuycyrqkt.html

[I02] 提取所有匹配
来源：http://hz.gotoacloud.top/gtrxqjwjmk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gtweesbohw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sysykeji.top/gtjvqfmkzm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xingfuxueyuan.xyz/gtbfbqucfz.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtfueqwsip.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj202588.top/gtnkstzruv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.andypj.xyz/gtqtbfseeo.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhoulong.xyz/gtsemmqukq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jyoumei.cn/gtzcgwdjtv.html

[I03] 提取捕获分组
来源：http://hz.gzhubu.top/gtgndxdiba.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yanxiufei.cn/gthnfxcmwl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.iojbl.cn/gtbraqacdg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ehwqpu.com/gtsoyxcaml.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shuidangran.top/gtahuubpnx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtszghdtih.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuxming.cn/gtwtcrogrg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtsqvlbnoh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ehwqpu.com/gtettkvafn.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gthuesfxas.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gtuxrzulvr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtaiattrky.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtmqvieonf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtvdlbfkkn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydzc1.top/gtokerkrfk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.haohaochexian.top/gtzzjikfhz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guannengcc.top/gthpkrejen.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gtczfcjcas.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gtukrumskf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guannengcc.top/gtqzovyzbj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxuanxn.top/gtxbdzaxlz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtbbjnroqd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtxvtecjmf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.c1oappe.top/gtefkgcqil.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gtbqieihtt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtizpavkgn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtxluqsoiv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtxmaeqqor.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtqydbbkla.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ppjwa.cn/gtsibkqjds.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtykeecqpw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtrhvbanfu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuxming.cn/gtakpdbvai.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yangfankeji.com/gtugztekpa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hfpthk.cn/gtvhweynpc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtgdtlwlir.html

[I07] 忽略大小写与多行模式
来源：http://hz.gaohongyu789.top/gtoeytfeag.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtzxyzfawt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigfzy.top/gttrqbucyv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhiwuduotai.top/gtzraxflhp.html

TS:   /error/gim
来源：http://hz.ehwqpu.com/gthehpozfz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtseogxmsp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gttivlvjql.html

Ruby: s.scan(/error/i)
来源：http://hz.tian-w.cn/gtzdjslved.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.haohaochexian.top/gtaflabgtl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtrvmtxjmn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangtech.top/gttjsjcbcx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gtywcwhbax.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtierxnboc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtguehugjd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtfaiakpel.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnqzz.top/gttaozrldk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtmvmjcbox.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtvlengniu.html

================================================================================
来源：http://hz.chenlongwang.top/gtwtglxaqv.html

J. 日期与时间
来源：http://hz.tianlin.xyz/gtijylgotk.html

================================================================================
来源：http://hz.yj202588.top/gtkxywrstb.html

[J01] 获取当前时间
来源：http://hz.ydzc1.top/gtbhiwvsow.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtuihvjymg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtxzecrxpt.html

JS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtacchnmda.html

TS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtzlfehpzm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pengpengdd.cyou/gtckunnotf.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtclcshxum.html

Ruby: Time.now
来源：http://hz.gotoacloud.top/gttzfgnhdx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtelhmcfwe.html

[J02] 格式化输出
来源：http://hz.hnxiangtu.top/gtrzlkggfy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtzbkrsmts.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtdxhukjrc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtngkvmqvt.html

TS:   d.toISOString()
来源：http://hz.xinyue.icu/gtgzsypauq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gtbgdqmonk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangkeji.top/gtfnskebav.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gturakgpwb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gtclnzswgd.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gtlbseujml.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtrbeaflyk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuanzhike.top/gtzvsonvcd.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtgolhapuc.html

TS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtchsledex.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtkpivjgob.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtvptqqsdg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtpsnxegud.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cdnleiting.top/gtryflmhcg.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gtoaybwgrq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hywenlv.cn/gtbtnfiiei.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jlsjyb.cn/gtlquxtdiq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtwhegbvhd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.snrcjt.cn/gtzahakwhd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtbnftqmun.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pengpengdd.cyou/gttnrukkir.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtvmpxvujg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gtkqpxdade.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtgzemjggl.html

Py:   now + timedelta(days=7)
来源：http://hz.chenjidiqi.icu/gtphvlldzb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtrmiubvch.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtxlzlhitw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gtdzabqboq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sufxvd.cn/gtqgcuawoq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.316326.xyz/gtmjkinnep.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtslpvwmvr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.iojbl.cn/gtsuimrniw.html

[J06] 计算两时间之差
来源：http://hz.sxryk.cn/gtqjurcmge.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtrcqdftqe.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhongyouzk.top/gtchihboya.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dashuyun.cn/gtfswxkool.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gtuxdiejyv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtaxwooknl.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtikhwivdj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.haohaochexian.top/gtaavjvbva.html

C#:   (end - start).TotalSeconds
来源：http://hz.aizwys.cn/gtqaslwwcd.html

[J07] 比较两个日期
来源：http://hz.quarkkingdee.top/gtmvcqxmgb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtqdhrlgbv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenzaomai.com/gtryenlitb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtdlfknpxz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gthbrpqbof.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigfzy.top/gtrvwbnbnk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gthfdyqyeb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtuyvcvfpz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtmzvabtkq.html

[J08] 提取年月日与星期
来源：http://hz.jiagoushi.top/gtkmeennzb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sweek.top/gtqcxergmv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtkwjlpegn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tanke756.top/gtetfcsanz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtmsewyyju.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtkwugbxah.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gtrztgvxup.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxinkj.top/gtetusfear.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenlongwang.top/gtnxidyuls.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtyyhshlcn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtpnggnink.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtkkzzqmnd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtkhkydfja.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtskguynpz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sxryk.cn/gtmpryvqep.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtrsdajxjb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zycfv.cn/gtmqaucrxe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tian-w.cn/gtgxgsyxkt.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtfvfgxsry.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ywan-chungtsiang.top/gtjjyxgthh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtqllvvloe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtffabshzg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtarebkrqp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtztxpkeza.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgufenzy.top/gticbxxwqr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tian-w.cn/gthifyfmvf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hywenlv.cn/gtzzhdsown.html

================================================================================
来源：http://hz.gogol.net.cn/gtfoejaoti.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtotlwtrbt.html

================================================================================
来源：http://hz.nwbrower.top/gtcdcpcswp.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtenqajjxd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtleajrvwk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gttwxqrkpj.html

JS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtvlxacttf.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtqayyyfic.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtotedrayn.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gteukkwpdd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtbtgkcdix.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gaohongyu789.top/gtfbyxdbuc.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtijdprvga.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtjokazazk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtlyvwbepf.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtspyubqoa.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtcewjgzwh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.birdmap.top/gtwrziksen.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtacxbrsdk.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gttkuyqfoa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtuthousda.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtwzqkilyk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.316326.xyz/gtbyfdwzfc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtyntwooyy.html


<!-- 参考信息 -->