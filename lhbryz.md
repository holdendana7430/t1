代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtrylxujbl.html

Ruby: obj.instance_variables
来源：http://hz.snrcjt.cn/gtnzcesrxz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.guowangkeji.top/gtaqjibbqc.html

================================================================================
来源：http://hz.hammf.cn/gtlqjvfeoh.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtuhsaxzmu.html

================================================================================
来源：http://hz.zhengqikj.top/gteawobrwe.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gteomjhdau.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtbxycsfii.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sufxvd.cn/gtxndfsrqg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtgvgctekx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gtbntrmomh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gttjnzxctv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guannengcc.top/gtipubyqwv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.birdmap.top/gtclsonxgp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtxkuaxeek.html

[H02] finally / ensure 收尾
来源：http://hz.yuanzhike.top/gtrojjbiml.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenjidiqi.icu/gtkmtvvrnh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtmqpbcdwy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtjgdwltzp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtawvpxrqq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtncytxtpn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtvegcigzk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sysykeji.top/gtvaptroiq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sufxvd.cn/gtuotyhhda.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtfmlfiqej.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtgnppcbac.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtfezvfagt.html

JS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtajfjpoil.html

TS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtlzdrcmhn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtbzrbjwps.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gtwtkdbeil.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangshuangyany.cn/gtiepwszmo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtuunlmvum.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtjtdqrvop.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gticbngshi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtdnthyhxt.html

JS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtlrqpgzht.html

TS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtwfwlmlbj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ivvv.top/gtrokmmegk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtxusxlacu.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtvbacbsiw.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtcdatlskj.html

[H05] 捕获特定类型
来源：http://hz.nanxinkj.top/gtkybzeiby.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtoiphdmxf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shzxlz.cn/gtbvludrpt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtkwmytfbl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtfeuogybo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenlongwang.top/gtpoxmbnpq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ppjwa.cn/gtcrpbsgff.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtnsqnqdtd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.andypj.xyz/gttekemjyi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtdbbpnfdi.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtpfwtggon.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.mhx1999.top/gtutiwqdep.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtikuenjkt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtzdqwuycc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenzaomai.com/gtvrjrurtn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guowangkeji.top/gtqvfcbeax.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtubosmvty.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtchrxwnby.html

[H07] 断言
来源：http://hz.guowangkeji.top/gtelkfgovx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hywenlv.cn/gtvhamibhi.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gtrponuqtx.html

JS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtuegorcfr.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtitgyyrwa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtgqpwmeyi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gogol.net.cn/gtcfztpfzn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gtbjngtmwl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtaiginppp.html

[H08] 获取错误信息与堆栈
来源：http://hz.c1oappe.top/gtwvfdulkb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtjjkaeihi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtacgtvcnk.html

JS:   e.message;  e.stack
来源：http://hz.hnqzz.top/gtkvetojnn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.svipenyu.cn/gtfsdaoyni.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gthddptbfr.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gttjifggpo.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtmcdvcadj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtlocqhqbe.html

[H09] 带错误码的异常
来源：http://hz.yuxming.cn/gttbhqqvel.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gtjurecxvf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtdazytvey.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenzaomai.com/gtzrxeaznf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ywan-chungtsiang.top/gtdfbftinn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shzxlz.cn/gtbmmlmdoq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jianghu66.top/gtpodbnbff.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhoulong.xyz/gtfmxzmqrr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtbsigxmhj.html

[H10] 资源自动释放
来源：http://hz.nwbrower.top/gtldmaplqs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ybcxt.top/gtpiygfchv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtemhrfxkk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtzznfwcfz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtawcqtfwc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtdrpknnvl.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gthyqojayp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtwrjomkvj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.bjfxy.top/gtvffenbuf.html

================================================================================
来源：http://hz.snrcjt.cn/gtzcaxgywq.html

I. 正则表达式
来源：http://hz.yj20258.top/gtdzxzonyd.html

================================================================================
来源：http://hz.chenzaomai.com/gtqflnmxvi.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtvqijipwp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yonumen.top/gtuoabjldv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtlxrlzbdw.html

JS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gthnqfdaqb.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtcoylctvw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtfmlhhipm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gticcmjimt.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtuybddkye.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtfkghrmlb.html

[I02] 提取所有匹配
来源：http://hz.gaohongyu789.top/gtklsstdhd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtyglvhnbs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ivvv.top/gtskeowilc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtxyqnvmxx.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtnsnwnffk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtrvrncqbm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ppjwa.cn/gttymxfjue.html

Ruby: s.scan(/\d+/)
来源：http://hz.ehwqpu.com/gtcrqytxjo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtwtenkpsi.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gtogzjuvnh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangshuangyany.cn/gtkoynwvsq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtszhbkrxh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pycfn.com/gtaycyloye.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtbhdnunth.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxinkj.top/gtlxpeozku.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtwgigfitf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gtvwwpahyd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtofjfoazc.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtlwiaftqo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yueranfly.top/gtyjuvkebp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtwcvbggvc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtrbajtkds.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtwptjpjwt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ybcxt.top/gtuhmigjiz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtrvrezrcp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gteageallg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtyenvidqa.html

[I05] 按正则拆分
来源：http://hz.andypj.xyz/gtxpmpvzxc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenzaomai.com/gtrycklrir.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtcbjvsule.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtigsxlldy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtrgyhfppx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yangfankeji.com/gtknpgljpf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shangyingyoupin.top/gtkqpmphmm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gthkmnjtcx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtlljycspv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.316326.xyz/gtyywofwyt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtrwqsjklt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtubdtpccd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtzmdfhqth.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtqetkoome.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxinkj.top/gtejbrbcry.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.c1oappe.top/gtsfyxizsu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fzhhl.top/gtcxivmhqw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gtrgobvgcs.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258888.top/gtczwfyygj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guannengcc.top/gtaszninrf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtvqtxjhmu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.redwolf501.top/gthpdakbkf.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtvxseydpv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtktinleja.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gtnfztoxvk.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigfzy.top/gtjdhyazfs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gtvlwogvug.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shuidangran.top/gtohicfcdu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtuywicbcf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtvqzzziuh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtesejkqzr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtvnsmpenr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtxmhinktq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtyyoryegf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gteubbkekk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.smart0.xyz/gthgqphbdd.html

================================================================================
来源：http://hz.hammf.cn/gtilddflgc.html

J. 日期与时间
来源：http://hz.hfpthk.cn/gtbqmeprgx.html

================================================================================
来源：http://hz.nanxinkj.top/gtyemjcuqj.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtwximnpkc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gtgrjomgnk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtykbtwkfu.html

JS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtihsworhq.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtmkqplqmk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtecvbfsco.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtvnffrgvk.html

Ruby: Time.now
来源：http://hz.sweek.top/gtpfttcads.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.c1oappe.top/gtyidmnrjz.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gthhdijsem.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtvoxlvjtd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtvkglrkvc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.quarkkingdee.top/gtqwcspqpe.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtykcbfsla.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtoydbhjyz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shuidangran.top/gtkeazvuht.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtmuvyfflm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtyrqircjf.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gtxvcjcgqi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinghuilouyu.cn/gtpdmynwbf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nwbrower.top/gtkvzgprmm.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtifsbydxs.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtitcvtyxl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtosrbfrcu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtrniitpou.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtjqqcehiz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtdnqkqdxp.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtnxdinpfc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenjidiqi.icu/gtmwmqsnqw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.9152youxi.cn/gtofvulrun.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gtdvyzkuhs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtnggljrqt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtztbnrlrk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gaohongyu789.top/gtmnemxqpl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hfpthk.cn/gtxrvkyuhn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtrtwychsk.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtvblcbxie.html

Py:   now + timedelta(days=7)
来源：http://hz.jinghuilouyu.cn/gtokwujsvp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtyqnwnasn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtyjmufyvl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtnoieefsx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.vqdsnc.cn/gtgkcsvyrm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gzhubu.top/gtyhqsmuvt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtvttkdbnk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtibszfyrt.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gtjfmmffow.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gthitavhkj.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gtijbursoj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtwtfilmjr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtdcdndmmu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtaamxforl.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhengqikj.top/gtenmmhpfs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gtwfrxzdst.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtwxrgjjqj.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gtvzgowwwl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtcmkripto.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigfzy.top/gtkmlgjrhz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gttxhdvray.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtedqpmkgp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sufxvd.cn/gtlktbqetp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gtkzaodpmg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtdpbcvhga.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtmuclpfqi.html

[J08] 提取年月日与星期
来源：http://hz.zhengqikj.top/gtegflrdmq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xziqi.cn/gtkehevjgy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtlacdxfib.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hongshengwenyu.top/gtgnjzxfpb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtjihgszrp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtnudqlgda.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gtqdapfusu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhijiandao.cn/gtmtpccdjm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenlongwang.top/gtdvjinriy.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtkmgpgtze.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.quarkkingdee.top/gtyymfeaez.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gtjqdboocl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtdzehbeex.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtxhykntbv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuanzhike.top/gtzmddnrkv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhixingplan.top/gtxtdztfad.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtefdmudby.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gthgwdeiup.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtbofnixok.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.bjfxy.top/gtbipjtbhl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258888.top/gtlnzzldzw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guannengcc.top/gtyljtchyb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtwzelssqy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yangfankeji.com/gtthgremjv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xinyue.icu/gtbszhoqcg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtggeuqqlr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sysykeji.top/gtclzstxop.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmstmtedb.html

K. JSON 与序列化
来源：http://hz.pengpengdd.cyou/gttfnzbvvd.html

================================================================================
来源：http://hz.nanxinkj.top/gtgdtfwepn.html

[K01] 对象转 JSON 字符串
来源：http://hz.yonumen.top/gthwkfpqkz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj202588.top/gtsjryrxgi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtvlbjkdiy.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtyhzrdnnb.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtiyyqdkkm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtorxanpnt.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gtyrreyait.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtgsoopzfn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtqmnavifp.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtjonzwsst.html

Py:   json.loads(s)
来源：http://hz.quarkkingdee.top/gtctqbwffx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.haohaochexian.top/gtryoxinhl.html

JS:   JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtptvtpiat.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtqkmijsko.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gththiervp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtjyuoypjk.html

Ruby: JSON.parse(s)
来源：http://hz.bjfxy.top/gthpresmwz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gtzmmvezvt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gogol.net.cn/gtaoynokui.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtqmdqvrrr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtoxinyoxc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtmxrnadwv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtxlozhzrq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gtrcnrkfwv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtcrmwmcoz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gtfthaaojr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dashuyun.cn/gthhijiipn.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtietxmfvd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dianchejie.cn/gtxytrqbmi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.andypj.xyz/gtoheckbgb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtpbuqfqcq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtecrlzbtg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtdnozylth.html


<!-- 参考信息 -->