代发 wailian999

Java: u instanceof User
来源：http://hz.pengpengdd.cyou/gtwbwofrtb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtihdebtvy.html

Ruby: u.is_a?(User)
来源：http://hz.fengsongda.top/gtkkysttcb.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtkzvlkxbh.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gttagdzxbv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258888.top/gtpbzfjrui.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtwikrbsme.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtmobyawzh.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxuanxn.top/gtnfztozyf.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gttpsbjbno.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuetiantiany.cn/gthypmxgme.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtopnifpad.html

C#:   record User(string Name, int Age);
来源：http://hz.zdqjudy.top/gtzygjsjtl.html

[G15] 枚举
来源：http://hz.nanxuanxn.top/gtlkuqmvaq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtkmfrpduf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guannengcc.top/gtktkpilgi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tianlin.xyz/gtajldvges.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gticfskkas.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtfkjxhnhz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtdcadcnpa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.andypj.xyz/gtyyhamjya.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtulljxnzj.html

[G16] 对象转数组 / 字典
来源：http://hz.bjfxy.top/gtynmzzkwh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jyoumei.cn/gtojmtrbxn.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtwuqdlzid.html

JS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtjgdxoxlb.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtffadeovd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtdtfxivvr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangshuangyany.cn/gtxrnnrfht.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gtknxdwzxv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtuftfwofy.html

================================================================================
来源：http://hz.cucudq.cn/gteeejitly.html

H. 异常与错误处理
来源：http://hz.wangdashe.top/gtdhmazwgx.html

================================================================================
来源：http://hz.ybcxt.top/gtfgxiaphr.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gteyhwqvmz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtovtnakvg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gtgxokxvur.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtfuztnhzo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gtklzsmvwy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gtsqgfvjnl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yongpay.top/gtuyzbopfk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtuahlgntr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daxiang520.top/gtzylqdxgu.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gtrsjwdqlv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sufxvd.cn/gtqfenxcvb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtlfqgbzzw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gttdfvocym.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtjeuefzxe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtmwebchso.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtiwvrejfq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guowangkeji.top/gtwjxxspsr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtlbcnslxe.html

[H03] 主动抛出异常
来源：http://hz.chenzaomai.com/gtvthtzasf.html

Py:   raise ValueError("错误信息")
来源：http://hz.sysykeji.top/gtcqkirift.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtrbchrrus.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gththndzwi.html

TS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtcxxgrjnf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtkiqvwctl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gtuasdgfpi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hywenlv.cn/gtmhzopzeo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtdgaugfhy.html

[H04] 自定义异常类型
来源：http://hz.havefunace.top/gtfppxgruu.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigufen.top/gtoaoaxaep.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtkivlsmws.html

JS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtbrbwlepm.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtlssocnfd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtzyzukhpq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gzhubu.top/gtvwveejqn.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtkjmoximm.html

C#:   class MyException : Exception {}
来源：http://hz.daxiang520.top/gtlyytcxoz.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtbyjwzdac.html

Py:   except ValueError as e:
来源：http://hz.smart0.xyz/gtcyunvonm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ivvv.top/gttovbpiqy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtjkymyidg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtkbrlybsi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yonumen.top/gtnxhoxndk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gttevwvhne.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtalbvmykm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtdjqomegq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jiagoushi.top/gtglvubrvo.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtmqhqgfav.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gtpnexznlc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtiqqyqzoc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtkomqyujz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuanzx.com/gtkvowkidd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fengsongda.top/gtyxrkbjgm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.birdmap.top/gtcmaeatbo.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtfgoelcwy.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtcmuuolis.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtkptcpayb.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtbbgldexz.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtjtftonae.html

TS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtyfllrhnt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtxprxevad.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtfaazsrkd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenjidiqi.icu/gtafmjswsd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtgjwobxpc.html

[H08] 获取错误信息与堆栈
来源：http://hz.hysaishi.cn/gttikvryxo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtrjhwzqps.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ybcxt.top/gtxrebwzyi.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtviayftxx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtkzmdabxo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtzrpqzdrm.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtdwusoxkc.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtpezfgfap.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnqzz.top/gtuawbmevm.html

[H09] 带错误码的异常
来源：http://hz.ydzc1.top/gtcukbheru.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxuanxn.top/gtlcvtfijo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shzxlz.cn/gtbppzjpqq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xziqi.cn/gtjthoiyyc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yangfankeji.com/gtckiinudk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sxryk.cn/gtcdolgwtp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtqzmiyxpt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tian-w.cn/gtilqgdyhm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtuxwiwyjn.html

[H10] 资源自动释放
来源：http://hz.zhaomingkeji.xyz/gtpkmarprt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtpujcwrzq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtndfbyyxy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yangfankeji.com/gtppfjkccd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtdpklquft.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.snrcjt.cn/gtgwldeids.html

Go:   defer f.Close()
来源：http://hz.xziqi.cn/gtgcyxpggd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtsuekbkzr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtgugqntrg.html

================================================================================
来源：http://hz.ppjwa.cn/gtjcqgzybr.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtoizdukqp.html

================================================================================
来源：http://hz.xziqi.cn/gtqocusbpy.html

[I01] 判断是否匹配
来源：http://hz.haohaochexian.top/gtwkkljttz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yongpay.top/gthpocscch.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zdqjudy.top/gtmdtavpok.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gttgdxopoy.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtdcldzxov.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtvgbokojx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtmowxfdmh.html

Ruby: s.match?(/\d+/)
来源：http://hz.bjfxy.top/gtlxvpxytg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gtnjtmvype.html

[I02] 提取所有匹配
来源：http://hz.yongpay.top/gtobfyotsj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtnqzrbhbd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guannengcc.top/gtddmpsjca.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shangyingyoupin.top/gtutfxqzwk.html

TS:   s.match(/\d+/g)
来源：http://hz.redwolf501.top/gttxcnduai.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.9152youxi.cn/gtfbewzceb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xinyue.icu/gtdbaoiqyr.html

Ruby: s.scan(/\d+/)
来源：http://hz.hongshengwenyu.top/gtgnllincw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gttqzwhlfg.html

[I03] 提取捕获分组
来源：http://hz.ppjwa.cn/gtudspseka.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtfjjssfwg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydzc1.top/gtpygplmfm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhaomingkeji.xyz/gtvempfaro.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.mhx1999.top/gtqbqmkrgd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtrsfhiwph.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigufen.top/gtfykfsydq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtighwpqau.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gtgmehtwdr.html

[I04] 正则替换
来源：http://hz.nanxuanxn.top/gtqiuuqzfn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtczmipcbr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtlhpbtigc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtffjzhvsg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtgcqxeqbw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxinkj.top/gtegtxtlvc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jlsjyb.cn/gtmezebljj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydzc1.top/gtsfelwpxf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gtjikwtayx.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gtnwkgqvcs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dashuyun.cn/gtdasshqvy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pycfn.com/gtsygogjql.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtefbpsebz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtgoyhcwbw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.9152youxi.cn/gtqdvjpuxj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtqwalelow.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtctkojxjp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gthdkbtoyj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gtraaxgtvf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtajrlbxfr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gtyiihmtoj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gthbhaaldl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtttwlpgkx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.bjfxy.top/gtykftsugm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtohwodvmh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xinyue.icu/gtocfgxjdg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtqdifonra.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtoondnbal.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daria6918.cn/gtbhjeccpl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtpslutivu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtvrpnibvw.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtbnydezji.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj20258888.top/gtpbdohioj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nwbrower.top/gtvngqsjpe.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtixakkkwe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnxiangtu.top/gtexjfiosk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hongshengwenyu.top/gtyfwigbkg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ehwqpu.com/gtbysixrdt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhengqikj.top/gttpphqpmn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtlgwtgpgo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtqmwcegms.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gtguzwopbp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daxiang520.top/gtwfnkscte.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtgrmsggfo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtiqwsmpdb.html

================================================================================
来源：http://hz.dashuyun.cn/gtnclwugev.html

J. 日期与时间
来源：http://hz.52xcode.cn/gtwzxvppjf.html

================================================================================
来源：http://hz.iojbl.cn/gthpcpuumq.html

[J01] 获取当前时间
来源：http://hz.yj20258888.top/gtbuwgodsi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daria6918.cn/gtauqdmjpx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtdfhujyjz.html

JS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtadzsnnep.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtcemjjmxc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gthkvopgyc.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtokfrzarw.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtaazdvpix.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gtdqeoeseo.html

[J02] 格式化输出
来源：http://hz.nanxuanxn.top/gtptixctyl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtkijwsmgi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtdlhdrcpr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtbvocwxdh.html

TS:   d.toISOString()
来源：http://hz.316326.xyz/gtaqhhjush.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtwqqejjbq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtkuuxvbne.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtxbnmbbnh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtrmxpxhfm.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtrbnqtzgj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtsreuzqwe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yongpay.top/gttdkhbmeg.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtiwiavlmw.html

TS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtzltczcyp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtialtvwjb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zdqjudy.top/gtblrhaoqx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtrhgrumxf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aibaodan.cn/gtlbstiabw.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtenazsgvw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ybcxt.top/gtuurbikuq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgfzy.top/gtkmovbjfh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtxzjhmblx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtmxbnnjbo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hfpthk.cn/gtppultjwq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gogol.net.cn/gtgoceueqq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258.top/gtbtedknfx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtitnnioph.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtaxocqbpe.html

Py:   now + timedelta(days=7)
来源：http://hz.ydjk.org.cn/gtbogkczsu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtnxjxbcyr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtizzbzjmn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtfncxaaja.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.0kj1m.cn/gtmleuzpls.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangdashe.top/gtjlaaqbuv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258888.top/gtnpylkfrm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtfsqsahtw.html

[J06] 计算两时间之差
来源：http://hz.zhoulong.xyz/gtsjvkbdpj.html

Py:   (end - start).total_seconds()
来源：http://hz.vqdsnc.cn/gtlbilwfzr.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtlynbphdz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtuqnqykre.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tian-w.cn/gtvjmqrfvr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtlpotapyg.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtooxiylin.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daxiang520.top/gtjalekkgu.html

C#:   (end - start).TotalSeconds
来源：http://hz.smart0.xyz/gtnzsvovth.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtvvclsidp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtclrhmzup.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hongshengwenyu.top/gtglpjsoff.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtxzhvaegq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtjwtwwvrk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gttghfrlmd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gtyltcpayx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtuixndlas.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtgrkuvshg.html

[J08] 提取年月日与星期
来源：http://hz.dashuyun.cn/gtamcogjub.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtunqwhvkq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gtgitcegjl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhiwuduotai.top/gtblmumhdl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtjmzmloek.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtlyiuopwp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtwhbwzgaj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nwbrower.top/gtxvzhywoc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.snrcjt.cn/gtkagpnbxl.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtilotbhmw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yueranfly.top/gtumkkubjl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gtagivillq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtblsjkndz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtotvesxcb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.snrcjt.cn/gtdnawmqpm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtpaztykvs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtqxwbqyic.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtveibrbnb.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtmimqlzwt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ywan-chungtsiang.top/gthxcfigiu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtxzpfjfbu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pengpengdd.cyou/gttoetjgsq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aizwys.cn/gtmczziwts.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtlpsqjmfw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.meibo888.top/gtsukzzwuv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtyryhpdxj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtvntpkmhe.html

================================================================================
来源：http://hz.ybcxt.top/gtyppnroqt.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtvetcqoeg.html

================================================================================
来源：http://hz.gaohongyu789.top/gthabbovzt.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhiwuduotai.top/gtrepojbko.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtxchobspq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtgwatskic.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtvkguppsy.html

TS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtzwvplacv.html


<!-- 参考信息 -->