代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtqrquttps.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtwbmjetxb.html

TS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtgywletga.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fzhhl.top/gtolioehtg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gtjlylxnig.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtfpophdvg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.9152youxi.cn/gtvkshtnet.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxzmhyapp.html

H. 异常与错误处理
来源：http://hz.yj202588.top/gtslzujoyl.html

================================================================================
来源：http://hz.yanxiufei.cn/gtmaqykkpd.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtitadwedu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtloyubwuo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtctdodzpa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dianchejie.cn/gtabqnszfn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtdprbxjdj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.smart0.xyz/gtfivsmqql.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtcxcovudf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pycfn.com/gtvqbcscup.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtvhhzenri.html

[H02] finally / ensure 收尾
来源：http://hz.zdqjudy.top/gtuyriruyp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtdaxwopqi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtmvunmhpu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtnptlffrr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtyvlyqyce.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtnsigmwfx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhengqikj.top/gtkvyfwnaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtmfhammer.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtuqnhbtss.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtxpryordm.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydjk.org.cn/gtdcgudmls.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtgmtjgjzn.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtsdkvaaqr.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtuwuatrsl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.havefunace.top/gtbbqdawxa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gtxkneucpj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dashuyun.cn/gtccdyjzkn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gtleyvndbf.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtdgabyldr.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtbdqnplkc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtwcavklum.html

JS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtjuclslfd.html

TS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtayffvdgg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtuuyzumwd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gtywozopde.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenzaomai.com/gtcyyndkld.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtxjsbefoy.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtoavterwg.html

Py:   except ValueError as e:
来源：http://hz.dianchejie.cn/gtzrdqncmj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtmgiksszi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtvejdomzn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtctglwkfa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinyuanbaomall.cn/gtycupjonf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gtsdstyshk.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gtdwzrwrfc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtdrkdvrgs.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtddvepggp.html

Py:   value = d.get("k") or default
来源：http://hz.xingfuxueyuan.xyz/gtxgqxbzbi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shuidangran.top/gtzljgtjti.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtozlnycaw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtptmiraee.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hfpthk.cn/gtjeytrsvm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtvrqvxfcm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ydjk.org.cn/gtrwjgqaow.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtmssenbuu.html

[H07] 断言
来源：http://hz.shzxlz.cn/gteuyancis.html

Py:   assert x > 0, "必须为正"
来源：http://hz.mhx1999.top/gtajrxvjgw.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtrwmkgzca.html

JS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtzqcqnosp.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtsutnflgc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yanxiufei.cn/gtxfzkpcni.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtqrocwgym.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jlsjyb.cn/gtwuzfphtw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.c1oappe.top/gtpyxammzh.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtkrsbohin.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtpzlcagxn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sxryk.cn/gtusgadlvl.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gtfawfaewb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gtqslhcpxr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtgsnmbzyg.html

Go:   err.Error()
来源：http://hz.redwolf501.top/gtodszeqdf.html

Ruby: e.message;  e.backtrace
来源：http://hz.sysykeji.top/gthmrbqtxl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtowreqdld.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gttxausxsp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sweek.top/gtdtnqjzgf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtfwgcewmw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtceutrxcj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gtsdbexkqj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.redwolf501.top/gtpnqfgzhy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtxbvtugqx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtvrieuran.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guannengcc.top/gttwdlptdf.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtpmaxbeqv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhijiandao.cn/gtgsrocqcr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gteprfqkqo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtrwgjwrsu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtqvciryae.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtmzqkwebt.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtohmylfqi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtncwmraol.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtwocmrlmz.html

================================================================================
来源：http://hz.tian-w.cn/gtjscelldo.html

I. 正则表达式
来源：http://hz.yonumen.top/gtpbpgqqne.html

================================================================================
来源：http://hz.tian-w.cn/gtbfwnqjnx.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangkeji.top/gtlcsayvta.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtgulmtdjb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.0kj1m.cn/gtnrottqug.html

JS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtqyouhwxp.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtpoydpuke.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtpttfkdsy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtmepeadto.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnxiangtu.top/gtahnclnlf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hysaishi.cn/gtzapanvcj.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gttqmzcodi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtlqerhbhk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtabzllrvx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guannengcc.top/gtyxwplznq.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtomzmfiqx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydzc1.top/gtaczeiczk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigufen.top/gtpytgrgmv.html

Ruby: s.scan(/\d+/)
来源：http://hz.shuidangran.top/gtlggiuaxb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtyvnlfvrm.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gtnpeeogwp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gtloaqogkj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtpinauglt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtcbjwfruy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtdntomplq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cheryme.top/gtykvkqerf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgufenzy.top/gtvgrvcavc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gtgksyuqhq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtpdaielxj.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gttlgjcgqn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinyuanbaomall.cn/gtcemfgrzh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtyncrvucw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtcgukfxxi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gttjuhwhai.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuanzx.com/gtozflkuic.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.haohaochexian.top/gtnurbdqyh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gtcmejuubh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtjgwlbkwn.html

[I05] 按正则拆分
来源：http://hz.zhongyouzk.top/gtampfuqtk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtvnkqiapq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtahdzqqba.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtfxpyellr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtjwjqamnr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtgfobndmy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtzhhqvllm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtorniydxk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtpwdfjjxx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhixingplan.top/gtlsqizmnt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtvhxirklz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gogol.net.cn/gtqksjhtos.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtuxxmxkra.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtmsylwynh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hfpthk.cn/gtysiqykmn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gthghonbqw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtljipmbgw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gthngarrvs.html

[I07] 忽略大小写与多行模式
来源：http://hz.sysykeji.top/gttuckiviv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hysaishi.cn/gtqumsuwwq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtaeljlkys.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gtulbqswfs.html

TS:   /error/gim
来源：http://hz.cqqwz.cn/gtbofaumay.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtwnvypboh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtncctrdju.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtbinkshnm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtsbnlvmhx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gtwcmblrym.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aizwys.cn/gtapjchzbm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtbgnqkwki.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gttmkpmiyp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtxkugdhmr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtzjyuuqne.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zdqjudy.top/gtwqdfbvtm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.mhx1999.top/gtikncupvb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtjbutyrgi.html

================================================================================
来源：http://hz.sysykeji.top/gtzwxlbifa.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gtvvapepzm.html

================================================================================
来源：http://hz.smart0.xyz/gtdgccadxi.html

[J01] 获取当前时间
来源：http://hz.ppjwa.cn/gtptgslirn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.316326.xyz/gtnjwenxnw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtfxlgtgwx.html

JS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtlvuaulgg.html

TS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtdzghtlct.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtymmftwrj.html

Go:   time.Now()
来源：http://hz.gaohongyu789.top/gtcjitscji.html

Ruby: Time.now
来源：http://hz.pycfn.com/gtvednaruc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuetiantiany.cn/gtckmksuzk.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtbrgfvymw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtnajuzabt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtnynszwqv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtuzrfhgmt.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtiuxdfskc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtcasmkczx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtsktwiccm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtpgxfuxfo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtmumctauo.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtsvckwycx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtqmrcjwhi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtivgiurmj.html

JS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtyeudbnjb.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtwawvxpbx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtwedzdevu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtcqheztrd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtjldfxzcz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gthqdjhgyl.html

[J04] 时间戳与日期互转
来源：http://hz.dianchejie.cn/gtocqkzazv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sweek.top/gtiihnkiqz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtaatduopq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtwcsnzsbs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtsyhqzbax.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtcxvknhni.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jlsjyb.cn/gtdumaraue.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gticusnmkd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtyhuwsigy.html

[J05] 时间加减（加 7 天）
来源：http://hz.feifeiyinyue.top/gtymatkdos.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gtbpioramt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yanxiufei.cn/gtinjexlkm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtaiombhre.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gteodeykiu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhixingplan.top/gtyfzqoqxu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shangyingyoupin.top/gtuplhaffp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtocewicga.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hammf.cn/gtjawwmtlp.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtnyfvaekx.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtuufvqewn.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtghuvbaas.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtebloaqbn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtmhnktimb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtjucuyobt.html

Go:   end.Sub(start).Hours()
来源：http://hz.gotoacloud.top/gthbauohyg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gtyqyrjhaz.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinyuanbaomall.cn/gtduchbzlh.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gtygizundj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtpruknzjv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cdnleiting.top/gttsdyyeyv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtxmetwghz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gttniqmcca.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtjjrgficc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtjtaezdzu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtzpurupzx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtswborypu.html

[J08] 提取年月日与星期
来源：http://hz.jinyuanbaomall.cn/gtycpgbmaf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtseovhnxv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtzmtyzyqp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtcnskektr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtmwdracxy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtwgnfkikr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gtjoglarku.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fzhhl.top/gtuuthjusl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aizwys.cn/gtaxsgncax.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtnoguybuz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtdagkhqoz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yvedp.cn/gtdsmapzgx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtgiivjvwz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtfesvqwsy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtfyeoolft.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtsiggvojv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gtkpgpchqe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tian-w.cn/gtkkmmlbfo.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtbtkimiis.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gtgfghkgkz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gtqumhpuel.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtfbwaqggf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gtiomtxdod.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtyieygobx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtfkngqjcw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtupykoevy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtftgjgxvb.html

================================================================================
来源：http://hz.tanke756.top/gtommygxfi.html

K. JSON 与序列化
来源：http://hz.guannengcc.top/gtqxujxofd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtfdsnkdet.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gteqwtncgq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtbekxybag.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtdxassmog.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtwkpjwygj.html

TS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtczrwktha.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gotoacloud.top/gtxewlchlq.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtwsbpsyrn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yongpay.top/gtsojilpgy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gtqipdamxi.html

[K02] JSON 字符串转对象
来源：http://hz.yuanzhike.top/gtqvjywufb.html

Py:   json.loads(s)
来源：http://hz.shzxlz.cn/gtxflkrvbe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtjpbuibmy.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtmvdcbncc.html

TS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtbwszlnnr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtfcrtnfav.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtfqbbgeel.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtotibbsmm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cheryme.top/gtfwtxphoz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtaplpdacc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtceuhtcyt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtgxwklaku.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtvkbwfgre.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtntfpzicb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtdcohjrne.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtvrzfiwkz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gtxnsozzqy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258888.top/gtlkjfhefv.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258.top/gtmxkvvwgw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aizwys.cn/gtarsrsctu.html


<!-- 参考信息 -->