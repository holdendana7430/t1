代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.ppjwa.cn/gtbihitbfd.html

JS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtnvnwekcq.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtbxspelyz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtvwmwnaaq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gtmanzderq.html

Ruby: obj.instance_variables
来源：http://hz.316326.xyz/gtjiwrwcsr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtzzgexchl.html

================================================================================
来源：http://hz.snrcjt.cn/gtvfjvyexx.html

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtrshfetlj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdwykcazl.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gtiwpgdukc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuxming.cn/gtwncgkbjy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtuifbmstw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtcjkdxasj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gteqdnzwna.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.svipenyu.cn/gtxapbffhn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtywlryntp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtlyajqeyy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtndzelulx.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtbpkkjcyw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xinyue.icu/gtlwvcxeen.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtfgpprgpu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtptajokdt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtqfkkewgt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtrqbiqdvc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtfepfcfwf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.snrcjt.cn/gtrhwyimrv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydzc1.top/gtaaejhaeb.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtzmjkqdzy.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtmdvpqpvh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtjcmgjxsj.html

JS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtjdgtxoze.html

TS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtbdqkidws.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtpyzcoinr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.redwolf501.top/gtvzfzecfx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shangyingyoupin.top/gtoxmqycnm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtpwxvimhl.html

[H04] 自定义异常类型
来源：http://hz.ydzc1.top/gtnskizkwt.html

Py:   class MyError(Exception): pass
来源：http://hz.snrcjt.cn/gtprznfcdy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtxiaiwjeb.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gteekxbomf.html

TS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtxypzyrfh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jianghu66.top/gthfqshjsf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gtqudegslb.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtxowcqkvo.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtzciurtls.html

[H05] 捕获特定类型
来源：http://hz.ydzc1.top/gtvovdkegj.html

Py:   except ValueError as e:
来源：http://hz.nwbrower.top/gtqkuzfuju.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtyjwimuwq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtpiurrvzl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtyhekpdgw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtephzlliy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtjglmmfls.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gtozmhbpyr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shzxlz.cn/gteizepovg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuetiantiany.cn/gtiadoomji.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtszjdrddx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zycfv.cn/gtoaajekiw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtteojgizz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtpasqajfw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtpacxdbjp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenlongwang.top/gtlprislko.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtmuszjubv.html

C#:   obj?.A?.B ?? default
来源：http://hz.birdmap.top/gtzpdagnhu.html

[H07] 断言
来源：http://hz.iojbl.cn/gtssdlnnhz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.snrcjt.cn/gtajgihygg.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gtvhywhwtv.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtqnmkvqfv.html

TS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtyhvyayfs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gthedzxpsc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dianchejie.cn/gthqzsrchk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tianlin.xyz/gtinqvqqae.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtvxvedaos.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtfalobyce.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zdqjudy.top/gtkwdhpkwl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtzeenjzzi.html

JS:   e.message;  e.stack
来源：http://hz.iojbl.cn/gtagjgnnbs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guowangkeji.top/gtbigowsud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtqgpxyxsh.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtgkcpvjhm.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gtyzwwwoqe.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtokguczbo.html

[H09] 带错误码的异常
来源：http://hz.chenjidiqi.icu/gtrcjdwuko.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtkuzmwyvd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtrzukcktg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ywan-chungtsiang.top/gtncqzhaqh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtrhklkxrb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxinkj.top/gtenkaxren.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fzhhl.top/gtbymvnfur.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj20258888.top/gtlkzyfiiq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtgvpwtpkg.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtildrvivz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnqzz.top/gtxiivjgiz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtkootdrxl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtmicbfdrn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtferfguau.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gtocsyuubd.html

Go:   defer f.Close()
来源：http://hz.snrcjt.cn/gtvahgfhir.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gttlrpehto.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtechaseum.html

================================================================================
来源：http://hz.zdqjudy.top/gtpnycplqd.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtypcagzyg.html

================================================================================
来源：http://hz.zhoulong.xyz/gthnsepzpm.html

[I01] 判断是否匹配
来源：http://hz.gaohongyu789.top/gtamilrcji.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtdghajhxo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guowangkeji.top/gtqeovjyqx.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtaxkyxqcd.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtilexszyg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtjdhutpjf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtlokfvqzp.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtdwvbeadb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gttbhthjrg.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtruderpxl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gteebujemd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangtech.top/gtoveyezha.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtdkowajdd.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtstznonro.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtvryglijg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.c1oappe.top/gtlaqcelfn.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtntlisvty.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtcnphmnsu.html

[I03] 提取捕获分组
来源：http://hz.ppjwa.cn/gttwdrhjks.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tanke756.top/gtpjpbcxep.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtvqtgvcpp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.smart0.xyz/gtcjeumcru.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gtokgmjoae.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtfpboxjbt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gttqnadawt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fengsongda.top/gtrxkzrnre.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gteoxbiffl.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtltdpuhoz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gtpbsbageb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtqfxzfvbp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtuiahweio.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtpmypsnuz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sxryk.cn/gtprociovc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yongpay.top/gtqkshlioe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtrfcrhvyv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtyxjoqpeh.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtyictefjy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aibaodan.cn/gtkxoicixz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gtmtwmiutr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtfqxtrrlv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtffhldpco.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhixingplan.top/gtddkjxojk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guannengcc.top/gttoxiyjyp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtaddivjum.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtwedommqy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtcucuygem.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtrhfvzgrx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtvrjkwhex.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gteagyeikt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtdqthnwll.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cdnleiting.top/gtrjjzioxn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtiqpmkpuo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtxbeozhgr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtirymjufw.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gtcbkwkprt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gtearymceq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258888.top/gtuegygcep.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtczgfhncs.html

TS:   /error/gim
来源：http://hz.yongpay.top/gtwnvvhasp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xinyue.icu/gtxwcczuar.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhongyouzk.top/gtkesuyobm.html

Ruby: s.scan(/error/i)
来源：http://hz.jyoumei.cn/gtijbnwtzl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtthnlrzkl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtfflaqiil.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gthhyoqsfs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jianghu66.top/gtbodoovfy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtjekmbxar.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtnqydptup.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gthkdyhhgp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtdwmdoyeu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gtetocvckg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtcbekqutp.html

================================================================================
来源：http://hz.fengsongda.top/gtqtqjkeyx.html

J. 日期与时间
来源：http://hz.yvedp.cn/gthegypibl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtchfynngu.html

[J01] 获取当前时间
来源：http://hz.jqgfzy.top/gtzdrtmede.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtrlcaxjxr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtcgjzfmui.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gtvjkiylei.html

TS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtecqavxha.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtoreigsha.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtsyizbzjd.html

Ruby: Time.now
来源：http://hz.sysykeji.top/gtnjilncgl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yonumen.top/gttswfmcmw.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gtndtcoiec.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gteoytxjnr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gteqyhdnnd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtbbsougli.html

TS:   d.toISOString()
来源：http://hz.nanxinkj.top/gtmngrsuok.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtpuqqiilf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtrwnqiqiy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtcnbqemew.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtnkvsqbua.html

[J03] 字符串解析为日期
来源：http://hz.yongpay.top/gtcwpznprw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtqncqtgkx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.feifeiyinyue.top/gtpelyedtl.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtakbwfxhj.html

TS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtcrnkywdg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtnpgrvxcv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jyoumei.cn/gtkhkguvhi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtqgzitrnt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xinyue.icu/gtvlbjalvi.html

[J04] 时间戳与日期互转
来源：http://hz.cheryme.top/gtimjtygjx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxuanxn.top/gttnzvevcz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gtfvijwvxs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.redwolf501.top/gtmhhuyuir.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.bjfxy.top/gtythamwal.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gttjrzndtz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtpbymsqsl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtuzfptcpe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gtvxrnebvn.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtjnxckfiw.html

Py:   now + timedelta(days=7)
来源：http://hz.pycfn.com/gttiqhdzkb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtygtguisr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtucddprhm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtsfssrmyt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sxryk.cn/gtfbxyqhql.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtjmyzgyks.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sysykeji.top/gtfiorxnzx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtejacynki.html

[J06] 计算两时间之差
来源：http://hz.yj202588.top/gtxxxjfced.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtqyftlaou.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtclfpmqhw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtaiulgnwk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gteqoaqpcs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtmvepwfse.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtdruidodr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtiishwmjn.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtupasooph.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtkikekmal.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtdajoydss.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.kuanghao11.cn/gtzoxcteit.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtmewqlapx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtsqpfqpha.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtiedjxutv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gthabnzkip.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtlovdfpfb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtrxwpgmso.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gthnbcuhej.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gthdpfwxeb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtlaztjlsh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gthzjoqwrb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtntyigyxp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtgfinzyoj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtmswflvpv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtqtphncib.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.snrcjt.cn/gthhsnkirc.html

[J09] 时区处理
来源：http://hz.feifeiyinyue.top/gtqfvqqqrq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnxiangtu.top/gtvdyugpdg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtmeikkqrd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtedkfljog.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gthglrvjlk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gtnmsnvoff.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gteudlfjsi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hfpthk.cn/gtdztkfsww.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtiyvutpvd.html

[J10] 取今天 / 本月第一天
来源：http://hz.guannengcc.top/gtudxfvedq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.c1oappe.top/gtkxujgpeh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtpwrtaxvp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtmmzrllwr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtwwsikzkq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cashguo.top/gttoxjvzkv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtaerxyitb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtawqttiua.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hammf.cn/gtxblktqiv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtnvmnabwx.html

K. JSON 与序列化
来源：http://hz.andypj.xyz/gtihigoivr.html

================================================================================
来源：http://hz.daxiang520.top/gtxbrdyrya.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtxiynopip.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtmauoqqzp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtyjmevlqr.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtbheidlxo.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtuhumiydw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.316326.xyz/gtguumzpqr.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtwogvsoto.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gtuapouqsh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fengsongda.top/gtehkojfog.html

[K02] JSON 字符串转对象
来源：http://hz.cucudq.cn/gtkuqyolee.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtgythpgws.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtntdgiswu.html

JS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtvszxtpkc.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtmkwmnhot.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cucudq.cn/gtgcrmcxof.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtmglhpypt.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtzrjdccjg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydzc1.top/gtjrngyhlw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guowangkeji.top/gtwjraqvzh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtcymcvaxo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtdnapvthc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gterdffqky.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtyazkofya.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtiyvchpdz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtpbaxqaou.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtjjlnpiue.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gtqdnotsvl.html

[K04] 读取 JSON 文件
来源：http://hz.nanxinkj.top/gtnmvsnmky.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtyjqnrywp.html


<!-- 参考信息 -->