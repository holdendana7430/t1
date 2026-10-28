代发 wailian999

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtiqqddxyv.html

================================================================================
来源：http://hz.jianghu66.top/gtatcfoeyh.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtezkxfgqu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yvedp.cn/gtcmofnafc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtrsxsgvgf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtntgwkbsf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fzhhl.top/gtixoldqid.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtxlrelcaw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtpzmecohk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhixingplan.top/gtdvchsbdl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtfavbtujl.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtnbxhbyxm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtyuayqayt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtstasosxu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtzcigdqac.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtzusqikyz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtcucveflq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.feifeiyinyue.top/gtrznclfry.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gthlinvuwl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gtchgilrkx.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtflaphnxk.html

Py:   raise ValueError("错误信息")
来源：http://hz.kuanghao11.cn/gtawplcgwz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtxulcqfdy.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtojkgedib.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtakkcgvea.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtmxxgcfuy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtolsfcmbc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtebtmklxv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtsxbnqszz.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gtoiylzzqk.html

Py:   class MyError(Exception): pass
来源：http://hz.jiagoushi.top/gtmliptvyw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangdashe.top/gtciltixtv.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtctxfmivm.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtmxvasrbq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtgxbaaafg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cdnleiting.top/gteryqqhvz.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigfzy.top/gtojsefski.html

C#:   class MyException : Exception {}
来源：http://hz.yonumen.top/gtvmigfwpb.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtyfksexie.html

Py:   except ValueError as e:
来源：http://hz.ppjwa.cn/gtvpsnbcyz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtahyyzfmx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtqxytrbht.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtmxtmuppw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtiowhspnn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtxqrlgwui.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtysszhvjc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtseavhldk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gotoacloud.top/gtpourjjah.html

Py:   value = d.get("k") or default
来源：http://hz.cqqwz.cn/gtfcneyszy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtxoewnmlh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtwpocosea.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtyckwjsyo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtlgdljlhw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtyjdxjthh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtnjxzokcn.html

C#:   obj?.A?.B ?? default
来源：http://hz.ydzc1.top/gtwcmrlujv.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtnluwgmjh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtrbiqvzcq.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtrjduzkrf.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtddspshrs.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtuwqhilrq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xylfe.cn/gtdsbdukes.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtwalpfjck.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtwuqfdkeu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtcrjhjmgi.html

[H08] 获取错误信息与堆栈
来源：http://hz.tian-w.cn/gtwupaluux.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtxbnrnyxp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtrgcjodfi.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtgtkzgsad.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fengsongda.top/gthbamrhdq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtcrgsnnwk.html

Go:   err.Error()
来源：http://hz.zycfv.cn/gtnymmqfxk.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gtitwhvmph.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtohybejml.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtslfmuqex.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pycfn.com/gtngodwuzf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtrlqsggdw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xziqi.cn/gtxctwuicv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gttyfwyvhd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtvvsbsroq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shangyingyoupin.top/gthxxoyaxu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ppjwa.cn/gtgvuixdst.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtosckfrtw.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtywdtjjmh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.bjfxy.top/gtalewuldl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtuhoifuje.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtdesldtiw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtdxihsrcv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtvblsolti.html

Go:   defer f.Close()
来源：http://hz.cheryme.top/gtmwyihreh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtanodwlqt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtawbofonz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtjgdetpoi.html

I. 正则表达式
来源：http://hz.ivvv.top/gtyqbcxfev.html

================================================================================
来源：http://hz.nwbrower.top/gtddcvktjd.html

[I01] 判断是否匹配
来源：http://hz.yj20258.top/gtvomgeqap.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.redwolf501.top/gtiofcxpbd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtdoqjchfq.html

JS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtaxlugtxs.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtfoqagiab.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gtkccurdcp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtoozwvpur.html

Ruby: s.match?(/\d+/)
来源：http://hz.jiagoushi.top/gtjydnwjbd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtlbormwtm.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtjyohvluk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtozdxgpvr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtiwsjnjch.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtuuryhxvh.html

TS:   s.match(/\d+/g)
来源：http://hz.jyoumei.cn/gtchdkymqf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.mhx1999.top/gtigxhkftd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shuidangran.top/gtqcmazzpg.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtoxccwfqq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtjnqnmrfw.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtfijmuatl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhongyouzk.top/gtihiylcaq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtvnebtcqi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hongshengwenyu.top/gtjtutacon.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangtech.top/gtfuytntsx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ivvv.top/gtebfbuiar.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtgjvcipob.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.iojbl.cn/gtaernxqvq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtwgdtshwj.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtnrnxihae.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ivvv.top/gtgrhelxle.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtsfgxuiij.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtywqhutlm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gthlbrblyj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhiwuduotai.top/gtlqjexzvi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hfpthk.cn/gtqiczvkfr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhengqikj.top/gtckfofmqe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gtgoqsxxvb.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtxxhtvnrh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gogol.net.cn/gtbmrdyzvs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jianghu66.top/gtunvtdtcx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtclenurml.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtdttzzgvp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gtjaotgpon.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cheryme.top/gtqmbtjqed.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtlidxvpnz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtcyvzxtfy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtairgnuym.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtlivubaya.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hammf.cn/gtdhpmkngb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daxiang520.top/gtztmzpjlb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtlspqbsxb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gtqhmplqkb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gtcvgczbdj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnqzz.top/gtgbscnahb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtmjhnsbhm.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtwlhnoocw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xingfuxueyuan.xyz/gtqunekfpo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tanke756.top/gtihaqmjxk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtlhscipuu.html

TS:   /error/gim
来源：http://hz.zhiwuduotai.top/gtammvmslv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtybpgmisq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtxssjwefj.html

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gtekrtucsj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtmnkyshal.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guannengcc.top/gtiamkhtma.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hongshengwenyu.top/gtzekrueip.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aibaodan.cn/gtfhylwzvi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtilldzmxo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtbmajkdcr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtnzdkxrmp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtsazycvge.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.c1oappe.top/gtnufkwsxw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtzqkdsmrh.html

================================================================================
来源：http://hz.gzhubu.top/gtsqophznr.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtjhgivbpc.html

================================================================================
来源：http://hz.sxryk.cn/gtqgjbrhgb.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtogjvmxfx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ywan-chungtsiang.top/gtytezvtjw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtchkthoic.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtbtsyzzpj.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtufmekeey.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtvsxtlnjs.html

Go:   time.Now()
来源：http://hz.bjfxy.top/gtitwjzmul.html

Ruby: Time.now
来源：http://hz.hammf.cn/gtwetoqfqj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ivvv.top/gtehftxqek.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtiwanlvxe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtymcmjesq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gteqdyvyve.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtyfdaiyza.html

TS:   d.toISOString()
来源：http://hz.iojbl.cn/gtqbzjddpk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cqqwz.cn/gtzgijyajo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtooepfmvl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtcafofqde.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenjidiqi.icu/gtfsvmvacm.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtalvfslgv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xziqi.cn/gtkrlpjdhs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtdvrzaqgl.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtjflbvugk.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtluojvrwy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtbdtccbdd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtnkgwsilc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtuqxojjct.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtoodqxilk.html

[J04] 时间戳与日期互转
来源：http://hz.hnqzz.top/gtipqcxbih.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtsoybjtpn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtavcqzfra.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgufenzy.top/gtgnhqmift.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtjvazgjws.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yueranfly.top/gtlszlocfx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hfpthk.cn/gtsrrmkjoj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.haohaochexian.top/gtwlodjrje.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtqdmeqbtm.html

[J05] 时间加减（加 7 天）
来源：http://hz.fzhhl.top/gtfiwypfid.html

Py:   now + timedelta(days=7)
来源：http://hz.zhaomingkeji.xyz/gtczfceclm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenjidiqi.icu/gtufvevmpd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtexxbscde.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtbneicqxe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtnsammvpv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tian-w.cn/gtrwarpygc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtmnhaacuq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hfpthk.cn/gtjpbqtnwo.html

[J06] 计算两时间之差
来源：http://hz.mhx1999.top/gtzutqslda.html

Py:   (end - start).total_seconds()
来源：http://hz.zdqjudy.top/gtnjbczsbl.html

PHP:  $end->diff($start)->days;
来源：http://hz.zdqjudy.top/gtpmthsnzf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tian-w.cn/gtchvcoriu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuanzx.com/gtfafqssds.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtfjisdkgs.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxinkj.top/gtogzvjuwh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtxlaulluf.html

C#:   (end - start).TotalSeconds
来源：http://hz.fzhhl.top/gtbbtsmjru.html

[J07] 比较两个日期
来源：http://hz.gzhubu.top/gtgcooithe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtgvcarvku.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.feifeiyinyue.top/gtdauhzbau.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtldpstqdz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gttwzdqeyy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtnezsffec.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cdnleiting.top/gtighcprgy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtkmjjhonk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gteimxpfac.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtufzkhthx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxuanxn.top/gtanccyvrm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhoulong.xyz/gtejznvvej.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cheryme.top/gtprbixqsb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sweek.top/gteovzyzvg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gotoacloud.top/gtgouwxwjb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtafprdglz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.iojbl.cn/gtorqqddrn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtltptycpz.html

[J09] 时区处理
来源：http://hz.cdnleiting.top/gtijahudxt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258888.top/gtrhtfiooa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daria6918.cn/gtgyvsjcib.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtubofqkkn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtwgszjefl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gtzynnjglf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuxming.cn/gtfzhguzba.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtlseiejcz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigufen.top/gtqsmetsrx.html

[J10] 取今天 / 本月第一天
来源：http://hz.fzhhl.top/gtzebnlhsi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gtudkusogu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtvceusrhb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gtxusrxsii.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gtktxlrvhl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtbupbheao.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhijiandao.cn/gthsxhjjsk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnxiangtu.top/gtrzadkbds.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtflwrsffh.html

================================================================================
来源：http://hz.jianghu66.top/gtlsjhmnqc.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtkwlqtrbw.html

================================================================================
来源：http://hz.svipenyu.cn/gtvqdbaair.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtfyyagzxx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtvsemrepz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtlgixnagr.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtpwqreezh.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtuehlsaux.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtcgzfaqph.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtrcjlbosi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtxqobqucz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gttefjqzkq.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtbpjqpcdg.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtvjmofmtm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtmrcinuyb.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtgzxjmrfd.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtrgpezxup.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtuhfiltri.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtqfiwlnsi.html

Ruby: JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtkxirtoxw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtrvavyskb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxinkj.top/gtnbhlfipb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtprlupffb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtfzbcwgbq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtnoebmsdp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtvjirunub.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtykfztthn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gtroxzqjce.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.52xcode.cn/gtzwlcnhch.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtvsdldjfc.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtudginbqe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtyjcjrrnv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtpppewrmq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtoryarlfz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtsqllqese.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gtocmnzjkl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtunojvxaf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtwvovlhbm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtbhcoqccc.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtqpzpkhgr.html


<!-- 参考信息 -->