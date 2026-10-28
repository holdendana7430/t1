代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtaweecvyl.html

[G15] 枚举
来源：http://hz.yonumen.top/gtkouydlkl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtahrbxhvq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtfjxqtgtl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangdashe.top/gtgwxxakhy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtsgadoebg.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtejaviqnr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtajlvptaw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hongshengwenyu.top/gtlwvxgezm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtjehvboef.html

[G16] 对象转数组 / 字典
来源：http://hz.zhiwuduotai.top/gttqelxgpr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtkruewfof.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtvsvgbpvd.html

JS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtaaffjmvn.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtroqujjfy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gtgbsqyggm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtzpwccbol.html

Ruby: obj.instance_variables
来源：http://hz.ybcxt.top/gtpjyuuiyj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.guannengcc.top/gtmlfqbmub.html

================================================================================
来源：http://hz.sweek.top/gtheexyofb.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtorsirzme.html

================================================================================
来源：http://hz.ydzc1.top/gtxfbtupap.html

[H01] try / catch 基础
来源：http://hz.nanxinkj.top/gtzzmqpogy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhiwuduotai.top/gtyglsxbvc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenlongwang.top/gtjhswadpj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gtjvisnczk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtbjmijowc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yvedp.cn/gtpfiidgej.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jlsjyb.cn/gtyjyugdkm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pycfn.com/gtcrlqkkvw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtrnhaqjaw.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtkxdfjsmz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gtxyupwduu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtbgweeuop.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtospavewz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtggwwsuta.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtefjcfytp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhiwuduotai.top/gtanuufwpj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cdnleiting.top/gtmiskszxk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtwhybqais.html

[H03] 主动抛出异常
来源：http://hz.0kj1m.cn/gtusgqbdio.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtmkrptufp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtawyhsxbw.html

JS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gthnpjnxen.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtqswjycut.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtvhqwfqti.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtijmeucqm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.haohaochexian.top/gtpcygrwio.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtvollmzoi.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtlcjehvfw.html

Py:   class MyError(Exception): pass
来源：http://hz.hnqzz.top/gtdgxrbmgs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gtpnqrcnij.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtivmuwpxy.html

TS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtbkejdixn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xinyue.icu/gtqirvjdii.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.316326.xyz/gttqqzqded.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtieuxjgkc.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gttbcayqec.html

[H05] 捕获特定类型
来源：http://hz.jinqigufen.top/gtfzcqmwvu.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtvsfelsei.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtedbxapsd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtefkcbelh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtrfmkkwry.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gtklhxtoqu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtcwqcmfdt.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangshuangyany.cn/gtovwcckdb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenlongwang.top/gtxenvuzth.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtaegsteya.html

Py:   value = d.get("k") or default
来源：http://hz.gzhubu.top/gtxosnlvsu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtgrynstgn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtlbnjjjwr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtazyigftv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtcffgimmk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gtpmtgbijn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigufen.top/gtnmjcidvl.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtcuglapqb.html

[H07] 断言
来源：http://hz.ivvv.top/gtcnsfxkkq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtvbyrlqtg.html

PHP:  assert($x > 0);
来源：http://hz.jinqigufen.top/gtwzyswdnb.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtpicqelhj.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gttnfwsagh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gogol.net.cn/gtwxzjfqxr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.52xcode.cn/gtnepiexuq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.316326.xyz/gtxloccuvs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gthevzzfhp.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhengqikj.top/gtaudsxgkh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuanzhike.top/gtenkrjwkv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtlmwolufv.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtpsmcplhx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guowangkeji.top/gtnojxbmcp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuetiantiany.cn/gtqjlfvgeu.html

Go:   err.Error()
来源：http://hz.hfpthk.cn/gtcifdfgyh.html

Ruby: e.message;  e.backtrace
来源：http://hz.gotoacloud.top/gtoeylndqo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zycfv.cn/gtbeizfgwv.html

[H09] 带错误码的异常
来源：http://hz.gotoacloud.top/gtpojlwxug.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtniuzxenu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gtddscqrop.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtflciuegl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.snrcjt.cn/gtrbgvffhm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gtjoylqptb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yangfankeji.com/gtzyrqnkoc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnxiangtu.top/gtzxbvnctr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtnxrkgucl.html

[H10] 资源自动释放
来源：http://hz.zhoulong.xyz/gtlgylmgci.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.quarkkingdee.top/gthacylfbx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtkpomlmyc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtcrudlxpb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtzlrvuiqw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cdnleiting.top/gtawhubjxu.html

Go:   defer f.Close()
来源：http://hz.chenzaomai.com/gtqnerbdgb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yueranfly.top/gtmmafhwmf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtzwddzmgp.html

================================================================================
来源：http://hz.yvedp.cn/gtpiwzoevm.html

I. 正则表达式
来源：http://hz.316326.xyz/gtfhocvgcz.html

================================================================================
来源：http://hz.chenlongwang.top/gtihoxwvvy.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtbrtbwrhg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cashguo.top/gtspfuiknl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenjidiqi.icu/gtcketzeiz.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtxgbuyhod.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtzuxeedyc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.haohaochexian.top/gtedizhfhf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gotoacloud.top/gtcgnasdku.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhixingplan.top/gtrghuspoj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aizwys.cn/gtbmjrfyiu.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtgtxfyqcf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gtyzpjhdlv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtsdxakuvu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnqzz.top/gtazoyqfxx.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtukosvgcu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtobcpbnoc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtuohvlsqs.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gtfsszodyl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj202588.top/gtiunvgkjf.html

[I03] 提取捕获分组
来源：http://hz.cashguo.top/gtsydwednh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fzhhl.top/gtfaagglur.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtjkfpynfa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtyiqjzcok.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cqqwz.cn/gttpwgdsbj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ppjwa.cn/gtbuewycgx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shuidangran.top/gtkkirxohl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.iojbl.cn/gtdkbtiqfb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shuidangran.top/gtwsnyysxz.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gtfxcbiyqw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuetiantiany.cn/gtwyacleqh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtdxffrcbn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gttklowgvr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtoqzrbvuy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtaayzpqie.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.haohaochexian.top/gtqbxslaqo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigfzy.top/gtogkcanvj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtrixoydvq.html

[I05] 按正则拆分
来源：http://hz.chenzaomai.com/gtgdiwmeol.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtudrsjmku.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtbywxrvlc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtyngsbsps.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtjelooyck.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnqzz.top/gtjdogxhsd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tanke756.top/gtftreqoks.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtvbihdtcn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.havefunace.top/gtlvjyschq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nwbrower.top/gtkdetphsx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtwtexcgsp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtndvcbsvb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtbtzrggkn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtthykcofl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtbbyfkmzn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gtlxutlocf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtrnkpexsq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gthqfadqgk.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtxfatxsvh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cqqwz.cn/gtqikqrons.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.mhx1999.top/gtdmrzgubx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tian-w.cn/gtcnwtlsic.html

TS:   /error/gim
来源：http://hz.aibaodan.cn/gtkeoknnzi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fzhhl.top/gtsccektzj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtedwvprfu.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtplggohvb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shuidangran.top/gtpsbizyik.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtfeppzphq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aizwys.cn/gtnelwuyfl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.haohaochexian.top/gtanlefmik.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtmjupdmzb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtvxyqffij.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtidzhniuc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtyzuxgdex.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.andypj.xyz/gtjcskwwmf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gtusmgumbs.html

================================================================================
来源：http://hz.jlsjyb.cn/gtuvtehytr.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtauhxzbio.html

================================================================================
来源：http://hz.mhx1999.top/gtyshevwyo.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gtkycexrug.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinyuanbaomall.cn/gtkljzjbfd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtnfezomwm.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtscmyurkn.html

TS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtagjxinhi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtvmqzzupu.html

Go:   time.Now()
来源：http://hz.hywenlv.cn/gtqxiwehdr.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtdadanewv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.haohaochexian.top/gtobdacfrp.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtakdsfxbj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtrlywaaja.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gthphgeazf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtwopwpqoa.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtsfmcwtmj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258888.top/gtenhdewec.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtssolfdyk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtcrwvxhav.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnxiangtu.top/gtvhletguh.html

[J03] 字符串解析为日期
来源：http://hz.316326.xyz/gtmozjoaih.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hfpthk.cn/gturdmdrcs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtkabbzxcf.html

JS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtbhrincdb.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtqtmhitfv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sweek.top/gtmouttksu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sweek.top/gtelyrxrhh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtfaoqgkxr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shzxlz.cn/gtvrrhpvqg.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtlkulauce.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daxiang520.top/gtjcjoapmt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhaomingkeji.xyz/gtccnsnmwl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtkvijakxu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hywenlv.cn/gtdicaorpu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtjteoydse.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.iojbl.cn/gtrxsxjzrm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtdugewqfh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xingfuxueyuan.xyz/gtcyejfwnv.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtzejqkyba.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtumrnajap.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigfzy.top/gtogbjpbst.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtjtshguhn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtiqqxgepo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.vqdsnc.cn/gtpcmivsrl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258888.top/gtkjowpkqw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aizwys.cn/gtgprwaxsy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj202588.top/gtoordiorq.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtgkrxlwyf.html

Py:   (end - start).total_seconds()
来源：http://hz.snrcjt.cn/gtesttrwct.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtzhicowdi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gthvesczvz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydzc1.top/gtxyditdin.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtvcdwanll.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuxming.cn/gtsxydogvx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gthuutrctn.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtlkgbccto.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtzbckgxvg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtgvtxkwlm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtctwvrhwe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gtpktuyeas.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtjuuwxcne.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gthnihofyw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtebcuqcti.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtdwfjpizw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtbzfbchjs.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtachkleji.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtfywaurnx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhaomingkeji.xyz/gtjsagjkak.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtpgcxfezi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gtkytlewvf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtkjkviqub.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtxxckxoaz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pengpengdd.cyou/gthovphtud.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gtrlodkykg.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtrtqhsdmn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtonxoxvwq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtwmpfgxma.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtszpqsddw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtihhjohsq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tanke756.top/gtunpgngic.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtkiiuimry.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.9152youxi.cn/gtyektjpkr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yueranfly.top/gtmrlseews.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuetiantiany.cn/gtwzkochzh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigufen.top/gteliveudp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtmrlgqyky.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtegdynvbb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgufenzy.top/gtosvmcvvo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtnwkmpegy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtvnfofbiv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gthmeylevw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtwbosdzqa.html

================================================================================
来源：http://hz.chenzaomai.com/gtqxwygfsu.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtihkgmhfd.html

================================================================================
来源：http://hz.zhixingplan.top/gtrdsydyvn.html

[K01] 对象转 JSON 字符串
来源：http://hz.tian-w.cn/gtypgykyql.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtfrpgnwjg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtnqzziilq.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtiygstqpp.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtzgwgmnte.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gttnjblhyj.html

Go:   json.Marshal(obj)
来源：http://hz.xingfuxueyuan.xyz/gtzpswygrw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xylfe.cn/gtrtaloprv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yongpay.top/gtkiloenwg.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gtxncuxyyb.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtwoywceja.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zdqjudy.top/gtdsokwjkq.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtkiqowxqq.html

TS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtqmmnwlnc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yvedp.cn/gtxkwstori.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtwfutoaju.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtnolayvbi.html


<!-- 参考信息 -->