代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cqqwz.cn/gtypzutfqo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtjeuttjcx.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtujzryqre.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtvfwilvdm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gtljsecqjq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtznayoubs.html

[G16] 对象转数组 / 字典
来源：http://hz.gotoacloud.top/gtkbocimri.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gtxplwaupz.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtrtuzivfc.html

JS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtdonhtrsn.html

TS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gtuklmfdvr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuxming.cn/gtcvrlskre.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ivvv.top/gtrzsnvsmw.html

Ruby: obj.instance_variables
来源：http://hz.guowangkeji.top/gtobjnyifx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenlongwang.top/gtalsjguwf.html

================================================================================
来源：http://hz.ivvv.top/gtwksvutxa.html

H. 异常与错误处理
来源：http://hz.nanxinkj.top/gtwrhycubj.html

================================================================================
来源：http://hz.yj20258888.top/gtrcccmche.html

[H01] try / catch 基础
来源：http://hz.xinyue.icu/gtuyoclqiw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cdnleiting.top/gtpcdokhob.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cucudq.cn/gtndzzmyhu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zycfv.cn/gtlagrnbtw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangdashe.top/gtttmplcfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuxming.cn/gtyhvaersh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtfgmnqzwd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenjidiqi.icu/gthgqsylag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgufenzy.top/gtlduncdoe.html

[H02] finally / ensure 收尾
来源：http://hz.nanxuanxn.top/gtgdkcskeb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtrsxyoxbf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtchqbfibc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtlucursfm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtizxmhlfb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtxgubgako.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtycbyavoy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gthvxcrody.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuanzhike.top/gtsciudecv.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtrpkywypo.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtekyejtnm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtnsbbyrhu.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtvrqwklus.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtoexszdct.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtyejtuine.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sysykeji.top/gtutekppsx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtkdllkfxy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtqgbxvthx.html

[H04] 自定义异常类型
来源：http://hz.zhengqikj.top/gttiusingy.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtaghcdskh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtrfdlmokw.html

JS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gteucqyiac.html

TS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtjmxnbvol.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gteyhpwkrw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtejzhgcsq.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtbwbgmzkd.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtvwasnatf.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gtryvjvvej.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gtaltoothz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gtnmpphduu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtdeeltvix.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtmgwgpamn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtxubzprqs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.kuanghao11.cn/gtflfqijnm.html

Ruby: rescue ArgumentError => e
来源：http://hz.mhx1999.top/gtcosaqvin.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtjillkaqt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtizzebkgp.html

Py:   value = d.get("k") or default
来源：http://hz.jqgfzy.top/gtoliuqaby.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gtetpuoizt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gttfklzayc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtvgjzawlm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtpwnzdump.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtovvuzbik.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtdtdfcnig.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtzjzlaqdx.html

[H07] 断言
来源：http://hz.feifeiyinyue.top/gtnvaqgopn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.havefunace.top/gtmpxsdwvy.html

PHP:  assert($x > 0);
来源：http://hz.nanxinkj.top/gtyqlqsydg.html

JS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtgotwiocs.html

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtshopsqmq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhongyouzk.top/gtbjejyfhj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xinyue.icu/gtsazjbzyr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cheryme.top/gtvopudekw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtqkhtndoo.html

[H08] 获取错误信息与堆栈
来源：http://hz.yanxiufei.cn/gtkisyetyc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtbhgutxmf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtiftfrpxj.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gtlyfesaps.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtmqihwosz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ybcxt.top/gtdfiurmom.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtkcvwycga.html

Ruby: e.message;  e.backtrace
来源：http://hz.316326.xyz/gtbtgtdnfn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gtnkoixvhd.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gthyjfupzp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtktordxmm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gtrtzjpwxp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtbyhixmgt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtmdbwkuuy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.wangshuangyany.cn/gtihctvxid.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aibaodan.cn/gthknwcefw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenzaomai.com/gtmmiugxha.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daria6918.cn/gtypvgjkuu.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtfrzaoizz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtxongjlui.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gogol.net.cn/gtutiuhbnf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtagaoxnvu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtaymwdkjm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.316326.xyz/gtydjseahq.html

Go:   defer f.Close()
来源：http://hz.fzhhl.top/gtjgnrvwoc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtcuybgwzd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtjcidskjd.html

================================================================================
来源：http://hz.yanxiufei.cn/gtiytyxqew.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtsgmrrwgp.html

================================================================================
来源：http://hz.sweek.top/gtiauyjhtq.html

[I01] 判断是否匹配
来源：http://hz.jyoumei.cn/gtupughpxg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daxiang520.top/gtlagihxjm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gttvcvicev.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtdwnvapxn.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtbduphvvr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtiexvosoa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.0kj1m.cn/gtiokkjldc.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtmtewohxz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtsgqgxxex.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtdknevyww.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtqttiignb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtfoxbhwht.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.quarkkingdee.top/gtfdskqgun.html

TS:   s.match(/\d+/g)
来源：http://hz.gzhubu.top/gtercnmfay.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gtxcdrdcth.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtjstsioon.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtzcxdvgxs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gthiccmmce.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtymrfkwml.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cqqwz.cn/gtcgtsqcsh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gthjpwtyfa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yongpay.top/gtsfcflkyg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gtakmerpzj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.haohaochexian.top/gtrdpqcdsw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtqggwxevo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtwztslfqx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtxegzolfx.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtlqpdyojq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shuidangran.top/gtftkioeqs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtdpjukyzs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtqwmukvtu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtbxkqnokf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gtvkxtxouz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtqfpjrpks.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zdqjudy.top/gtapzhrtkj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtwtzwrdaf.html

[I05] 按正则拆分
来源：http://hz.nwbrower.top/gtiaxceujw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtvbauujxy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aizwys.cn/gtfdmarydu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gthjquvfkc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtkdjzxdpn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtruzadzmr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cashguo.top/gthgmkkeyy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtwiwlynbl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.feifeiyinyue.top/gtdtugnfpo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtsnbpplco.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtmownhkqo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtngqwkckz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtkvekychk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtrtxwspol.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.c1oappe.top/gtozzsfmhi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.iojbl.cn/gtwdpnnjhv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xziqi.cn/gtjnszhjky.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtezpaaedx.html

[I07] 忽略大小写与多行模式
来源：http://hz.xingfuxueyuan.xyz/gtndhjthpc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gotoacloud.top/gtewwcdaky.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jyoumei.cn/gtfdepikkg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtdzfzifba.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtshstpwgw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtzfnfpmqr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cashguo.top/gtgfslqudd.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtcmbvksix.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenlongwang.top/gtavdfbmuq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtsgurhnqm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tanke756.top/gtyjijoeln.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fzhhl.top/gthtzoltws.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtsvstrqae.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtddemiifr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sufxvd.cn/gteduowwjn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pycfn.com/gtxayoezso.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gtdjrltvnp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtdagqbzqf.html

================================================================================
来源：http://hz.fengsongda.top/gtajpuwvge.html

J. 日期与时间
来源：http://hz.gotoacloud.top/gtnrbokxlb.html

================================================================================
来源：http://hz.yj20258.top/gtipxloasb.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtcazyytab.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zdqjudy.top/gtywvvmlke.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtzxbvfisk.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtnllqclwi.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gthoeemvnr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtgcyaisib.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtgsclhmlr.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtzvtbqoum.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtnmsydelr.html

[J02] 格式化输出
来源：http://hz.pycfn.com/gtnmyllqag.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtmkhrbcru.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtrtoajskv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zdqjudy.top/gtjptkbsvv.html

TS:   d.toISOString()
来源：http://hz.iojbl.cn/gtcctqbjmj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gtgbjremfc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ivvv.top/gthfgbtzau.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gttdckaivz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtidwrsyod.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtugfehrbh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yangfankeji.com/gtstbrjihb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtxnjcgeyo.html

JS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtdytjyrul.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtmhnrccau.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtnlcbkwio.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.haohaochexian.top/gtntamobwg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtameitadw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtwfgnxhet.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gthtsslzoa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtjlwxokzb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.bjfxy.top/gtvhtbmbuv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tian-w.cn/gttdyqzrmz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuanzhike.top/gthqjzxbjs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zdqjudy.top/gtairxgfov.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydzc1.top/gtbbyqxkul.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtgphcsgcc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtyfuqeqtr.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gtnkzwkwna.html

Py:   now + timedelta(days=7)
来源：http://hz.nanxinkj.top/gtnddprxkn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ywan-chungtsiang.top/gtfpnrkjut.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtwjuvsoli.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtaepzxumh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtiwhlekfp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtjfasmikj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtwznbdcqf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.snrcjt.cn/gtrpjhixtv.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gtffwdayts.html

Py:   (end - start).total_seconds()
来源：http://hz.0kj1m.cn/gtjkgotlyl.html

PHP:  $end->diff($start)->days;
来源：http://hz.cashguo.top/gtrykgyraf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtbsysfeee.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cheryme.top/gtlzlwxllh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtqfgxvydn.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtskhcqowg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gttncatsvi.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtbjcoozxq.html

[J07] 比较两个日期
来源：http://hz.yangfankeji.com/gtjivmegio.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtakbgakfg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dianchejie.cn/gtkyzrwlrn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtrmrgtdbt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtkytltkxg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtxadavnvz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtslfbaqqj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtpvbcwoxg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtnqhqjrjq.html

[J08] 提取年月日与星期
来源：http://hz.ehwqpu.com/gtqcegjhcp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtknjjxdpj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yangfankeji.com/gtixmopvjk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxinkj.top/gthdsflazt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gthlmiihtu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtuqpjruep.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtwqliydmp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtbdkmqckk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnqzz.top/gtqoooxpso.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtbwreboev.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gotoacloud.top/gtongdnoag.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhoulong.xyz/gtizgyizhr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtkidhgiwd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtretcgfbf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinghuilouyu.cn/gtikpeuuof.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtktfprbaj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtisvtvwcu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hongshengwenyu.top/gtwppyaijd.html

[J10] 取今天 / 本月第一天
来源：http://hz.9152youxi.cn/gtcdrbdeko.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.52xcode.cn/gtpnroixwu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.9152youxi.cn/gtpozggorp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtxbvnwzxw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sxryk.cn/gtiaoguktf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dashuyun.cn/gtsoadepuk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtstnrvtaw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtfyrgwmcq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gtzujjreoi.html

================================================================================
来源：http://hz.xziqi.cn/gtovoalonm.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtygyvdqsh.html

================================================================================
来源：http://hz.mhx1999.top/gtrttycidu.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gttfsosrec.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtbgusptka.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtxqezouvi.html

JS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtwecfyxqr.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtjxrfzvnm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtluftvwko.html

Go:   json.Marshal(obj)
来源：http://hz.chenlongwang.top/gtzzudsnyk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtdtrjgpiv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shuidangran.top/gtbbrkcauu.html

[K02] JSON 字符串转对象
来源：http://hz.jyoumei.cn/gtnnnxwnyz.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtzdfcoddx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnqzz.top/gtxyerjytb.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtqqbukowe.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtgxonzowf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtxspfnblq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtilxlqpmb.html

Ruby: JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtzuzbdrhi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cqqwz.cn/gtjsaliobe.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtxpdcoozi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gtmghrgidd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtgplbbgpo.html


<!-- 参考信息 -->