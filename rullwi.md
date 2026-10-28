代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtjkaqcned.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtctxodzzv.html

Java: enum Color { RED, GREEN }
来源：http://hz.dashuyun.cn/gtmmmujvpa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.bjfxy.top/gtfqkkqhtc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtrvozmxjd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtfvouufcb.html

[G16] 对象转数组 / 字典
来源：http://hz.zhoulong.xyz/gtmkxfiomo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.vqdsnc.cn/gtyxqiioav.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtyqdkmmqe.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtwrgxuecj.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtkrlfalvt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gtniyiywhk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ppjwa.cn/gtfjzyylxl.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtgwrudhgp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zdqjudy.top/gtvcloyvoj.html

================================================================================
来源：http://hz.zdqjudy.top/gtaogfbuif.html

H. 异常与错误处理
来源：http://hz.haohaochexian.top/gtukmdwjxs.html

================================================================================
来源：http://hz.52xcode.cn/gthhqdmmjw.html

[H01] try / catch 基础
来源：http://hz.zhixingplan.top/gteunniofq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sweek.top/gteuslxdvg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.havefunace.top/gtqzemnffd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtpllqzkgp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gtthnprkri.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtggaqszci.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhoulong.xyz/gtzxlumesx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dashuyun.cn/gtwwsxuzat.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtmscxxnrf.html

[H02] finally / ensure 收尾
来源：http://hz.zhengqikj.top/gteyclnjxw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nwbrower.top/gtkebozqqv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtevbuxqmc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gttasywuvy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtjqeorwth.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtkgunriwh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtxcbhbzkd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xinyue.icu/gthuvfriui.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtmamukxtq.html

[H03] 主动抛出异常
来源：http://hz.meibo888.top/gtvvvtbwtr.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gthekpfzgm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtpcrdiaee.html

JS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtgvaofacx.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtupcoounh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtqxzbohyc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gtfbxeommc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhiwuduotai.top/gtidhdszux.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtlyqallke.html

[H04] 自定义异常类型
来源：http://hz.gogol.net.cn/gtahopxqlw.html

Py:   class MyError(Exception): pass
来源：http://hz.snrcjt.cn/gtvxxsxobs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtgwvkihzf.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtaptxqwpa.html

TS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtjskgjfwi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gtsdlhszil.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pycfn.com/gtbrasawgb.html

Ruby: class MyError < StandardError; end
来源：http://hz.vqdsnc.cn/gtyjhbhpir.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtkdazpykl.html

[H05] 捕获特定类型
来源：http://hz.jlsjyb.cn/gtpgvibpia.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtikmgmsbb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtcaioxkwk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtcjnckimz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtftilqgdj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.andypj.xyz/gtdslrufyn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gttsopubuf.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtimiixtto.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pengpengdd.cyou/gtuvwyhmro.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gtdloldwhq.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtyklwpkwv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtzcrzjjhl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtipnuxgml.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtxictvkvv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fengsongda.top/gtubutbhxh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ehwqpu.com/gtrkutibsm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.aizwys.cn/gtbduljuco.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtxxsolzzv.html

[H07] 断言
来源：http://hz.daria6918.cn/gtsulgkozx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hywenlv.cn/gtxccfcvrn.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtbgnxxomx.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtctxqhcak.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtjmldodnq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dianchejie.cn/gtnbuyppzo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gtpdbdebqt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.andypj.xyz/gtmvvxztgh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj202588.top/gtkjromayz.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuetiantiany.cn/gtpzljdtly.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gthnnspzbh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gtgsjebovc.html

JS:   e.message;  e.stack
来源：http://hz.yuxming.cn/gtjhtsolnx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtyixklvrh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangkeji.top/gtxtcezsfz.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtaqcpchah.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtghepojik.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuxming.cn/gtkntlrhdb.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtqbuyztao.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cucudq.cn/gtqjbgdxjg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cashguo.top/gtnpstsjrd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtafkklscn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtstxzjvbl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtpivwlpwp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ywan-chungtsiang.top/gtfvakjcia.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuanzx.com/gtvzfujdqp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.havefunace.top/gttmnqlkoa.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtajppzygf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtzmmjlocu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtkvpxzoxo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtzfsmipxb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtboyjqjux.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtrotwqlpc.html

Go:   defer f.Close()
来源：http://hz.ppjwa.cn/gtopipgozy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtsitcwlxs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtxoslblmv.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtguyvbqwo.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtgjxbbjeu.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyhnhoeex.html

[I01] 判断是否匹配
来源：http://hz.ydjk.org.cn/gttfanymmf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigufen.top/gtwewaouny.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtijkdnlgj.html

JS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtbxajttaf.html

TS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtaikzxfee.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtlcxzeoua.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.redwolf501.top/gtgfuvdkxg.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtbxogrolf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtogaqfkiz.html

[I02] 提取所有匹配
来源：http://hz.sufxvd.cn/gtomubnyck.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtufaalrjr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtnevstcnq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxuanxn.top/gtwyowmjqp.html

TS:   s.match(/\d+/g)
来源：http://hz.aizwys.cn/gtdnicyrwe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtpjobgvwl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtxespzlpv.html

Ruby: s.scan(/\d+/)
来源：http://hz.iojbl.cn/gtcfohenuo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtunldzele.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtgijjqnex.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtuyiydfel.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhaomingkeji.xyz/gtrqzzxzfl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtqziqsttb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gtdeantmzc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtumlhftyi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhongyouzk.top/gtyyvqpudb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gtfzrbweup.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gthvclyxwm.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gtivxhyrxq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gtbfkunyor.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tanke756.top/gtxycqhxdg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtvrhvwrhe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtrehajeyo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yvedp.cn/gtxikkongu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fzhhl.top/gthdhumleq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gtoeafkuxn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtmnntgplb.html

[I05] 按正则拆分
来源：http://hz.tianlin.xyz/gthcvwpimf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cqqwz.cn/gtmmvrikoi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gotoacloud.top/gtamdkiqvk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtxjmwzcua.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtgcftpqcg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtmyxerzde.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtsnecwamt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtsqydohir.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtipxadnnf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gtjlyvctby.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtvapemjxs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangshuangyany.cn/gtgbeocabd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtsajntaqi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtiiuswewa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gtdhtaybxo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtgpnogvhi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hywenlv.cn/gtupymkogs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtnilgzijq.html

[I07] 忽略大小写与多行模式
来源：http://hz.meibo888.top/gtfovufiho.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnqzz.top/gthkdpjuao.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtfmprrtuy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.havefunace.top/gtsznatiml.html

TS:   /error/gim
来源：http://hz.jqgfzy.top/gtxuruhawe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtrqtpywho.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gtmsejrojo.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258.top/gtuatbuecm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.mhx1999.top/gtihswjofo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtywwzoxvl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jyoumei.cn/gtramevnmk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtglnyrnvs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtarwdshnx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtpedemvhn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtqjskgntw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hammf.cn/gtqcghpgbb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gttfbtvaih.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtwpiirpsc.html

================================================================================
来源：http://hz.52xcode.cn/gtqnclafzw.html

J. 日期与时间
来源：http://hz.xuanzx.com/gtrszxcfbf.html

================================================================================
来源：http://hz.jyoumei.cn/gtqqwsvkzq.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gtifgapsid.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gtdpdpttgi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtjuvvhxso.html

JS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtjmqochui.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtgzsbqyyx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sweek.top/gtuuxpaerw.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtfuvpefpf.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtczbhtagx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guowangkeji.top/gtuxjvmrvo.html

[J02] 格式化输出
来源：http://hz.hammf.cn/gtrktrjijc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtltbnjkou.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtiqcytinu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtsznbzptf.html

TS:   d.toISOString()
来源：http://hz.ehwqpu.com/gtnwttquet.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtybkounpj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtxycoppcn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtsyjrjlsr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hywenlv.cn/gtntoztdqo.html

[J03] 字符串解析为日期
来源：http://hz.cucudq.cn/gtudkiarze.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydjk.org.cn/gtrobmczop.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.meibo888.top/gtsexpqtdx.html

JS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gthzhnekvk.html

TS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtqvayprzb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtnlrehoch.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gteiuuwkuy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtlnlzthxl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhongyouzk.top/gtwejmsjas.html

[J04] 时间戳与日期互转
来源：http://hz.hnqzz.top/gtblvoedar.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.guowangkeji.top/gtqsjndbjt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhaomingkeji.xyz/gttsgonaig.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gtahlrxwsp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gtiorkpkar.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtbfinqztj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtaxsnxfqv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gtwhqefhkh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtbgobtdox.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnqzz.top/gtfeltynft.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtpkincjxo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gtwgpdrhfh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gttggvexuh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gteuqaktfn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gterlnhbnp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pengpengdd.cyou/gtvixvoaut.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenlongwang.top/gtrcftatzg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtwgkmschk.html

[J06] 计算两时间之差
来源：http://hz.cheryme.top/gtfninkmfc.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtlsyguvpx.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtfcgqkgtt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gtmfodxool.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yongpay.top/gtpircpqoa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtqlqfaffj.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtyzgklorl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.svipenyu.cn/gtleusrcqo.html

C#:   (end - start).TotalSeconds
来源：http://hz.52xcode.cn/gtstobhoch.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtpknzbcvc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtzrpkispr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtnpxxbrnc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtzcxrcnjs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtgztkglct.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtwksheweu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tian-w.cn/gtldqwyauy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtgbzftver.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtgbmnspoa.html

[J08] 提取年月日与星期
来源：http://hz.sufxvd.cn/gtoszfoplr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hfpthk.cn/gtkiwkleji.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtywlirmuq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tanke756.top/gtvureqaos.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtmnckqufq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gotoacloud.top/gtccpvhvgf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtprdivcpn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtbjereiqz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.mhx1999.top/gtblcwhxgk.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gttjhiommh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shangyingyoupin.top/gtgouvpzve.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangtech.top/gtxdfazodi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtjpkghkzr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtderkeadx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtqgtttoju.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtwhwrocav.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtokqzyhtb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gtzxajglkt.html

[J10] 取今天 / 本月第一天
来源：http://hz.nwbrower.top/gtwdzvipvu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhoulong.xyz/gtoadgajyy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gteczezsdf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guowangkeji.top/gtirokpzjh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gthqtzvboe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gthwhrixqj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gtpxrgwtmv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.kuanghao11.cn/gtxkwctuli.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yonumen.top/gtwxxxccyq.html

================================================================================
来源：http://hz.sxryk.cn/gtvjxucxuu.html

K. JSON 与序列化
来源：http://hz.wangshuangyany.cn/gthuqgfvwf.html

================================================================================
来源：http://hz.cqqwz.cn/gtxqulapid.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtardeytai.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtozdxppvu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtgzubhdek.html

JS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gttmqruesv.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtqzeayivf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtymcojovn.html

Go:   json.Marshal(obj)
来源：http://hz.xinyue.icu/gtjrmqptri.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtwnzwhscb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgfzy.top/gtxbdffmol.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtbinayfzb.html

Py:   json.loads(s)
来源：http://hz.zhiwuduotai.top/gtvhqbygez.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gtgoylqaxz.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtlswlgizt.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtbsakkugd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtbqwypkru.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtgcrsgkme.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtwgamlfmz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtxgghzbzz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gogol.net.cn/gtmijeaymp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtwbkosstj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gttgzdmuwg.html


<!-- 参考信息 -->