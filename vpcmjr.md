代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.mhx1999.top/gtvlygaadw.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtwxtlpvmy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtddrubaup.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtdnlugccu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gttgfesnmk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtymdqpiwe.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinghuilouyu.cn/gtefvzbwnp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sysykeji.top/gtyhordcqq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gtvvwcpucj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtkfhpzswk.html

[G16] 对象转数组 / 字典
来源：http://hz.hnxiangtu.top/gtgqpgtrds.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtigzhpnos.html

PHP:  get_object_vars($obj);
来源：http://hz.cashguo.top/gtdorlwdym.html

JS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtovdtvisq.html

TS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gtfndgtbuu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtakshmjwd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtoautgsyk.html

Ruby: obj.instance_variables
来源：http://hz.guannengcc.top/gtzqpophxa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgfzy.top/gtgnxxzbfg.html

================================================================================
来源：http://hz.xziqi.cn/gtquvnwehy.html

H. 异常与错误处理
来源：http://hz.fengsongda.top/gtwvuqyxen.html

================================================================================
来源：http://hz.mhx1999.top/gthynmezla.html

[H01] try / catch 基础
来源：http://hz.quarkkingdee.top/gtxozipbsn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hongshengwenyu.top/gtkhbomswx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangtech.top/gthldkllck.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtbgmfufwc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hywenlv.cn/gtsfouzlxr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yonumen.top/gtadkdzpod.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtpehlqsng.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.52xcode.cn/gttldfbtip.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yangfankeji.com/gtsjqsurhg.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gthiazuqlc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtyqammcuu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtxhlzswcr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtctbmcthx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtssajcvsa.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtxgcaoqkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xziqi.cn/gthndeorph.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtescviseh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtbihdyloa.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtwzndxonr.html

Py:   raise ValueError("错误信息")
来源：http://hz.hysaishi.cn/gtsfudgben.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtqagovfhk.html

JS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtyyitnahz.html

TS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtczpahotm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtcactmjhf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtntjbqpce.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yvedp.cn/gttlityfyp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtdgkdmevm.html

[H04] 自定义异常类型
来源：http://hz.jqgfzy.top/gtagfnxdcw.html

Py:   class MyError(Exception): pass
来源：http://hz.shuidangran.top/gtuzrufcbz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtvkhmxdtt.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtajrwqomt.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gttwdmebiz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtgfgeozot.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nwbrower.top/gtnyyjdikh.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtxgvpzpoq.html

C#:   class MyException : Exception {}
来源：http://hz.cucudq.cn/gtgdfkbslm.html

[H05] 捕获特定类型
来源：http://hz.316326.xyz/gtknvccpsa.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtinuiblod.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtwbbljcoj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtkwsbmtyl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtjudbgzdw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtdpbdmcxi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtvvnhqboy.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtgulrqryk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gtlswallvy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhixingplan.top/gtozylsjbc.html

Py:   value = d.get("k") or default
来源：http://hz.guowangkeji.top/gtilvrccpf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtnomslruj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtnjxgcohf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gthrijagft.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtpuhdlrkm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangdashe.top/gtwmppqnhf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.andypj.xyz/gtvhwibqaq.html

C#:   obj?.A?.B ?? default
来源：http://hz.birdmap.top/gtbwxsessg.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtvicjvgmf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daria6918.cn/gtuaikynvx.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gteixtvfzz.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtnoownhmn.html

TS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtrnhvpdta.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtvsxvzrcx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gtvmmxlgmm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtmiogibce.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gaohongyu789.top/gtglvzkvhd.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtmegnbauu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtloyngabn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gthnqjdocz.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtytvirjzw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gtdatkhqeu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtrhewwdsr.html

Go:   err.Error()
来源：http://hz.yuxming.cn/gtokbcqdfb.html

Ruby: e.message;  e.backtrace
来源：http://hz.bjfxy.top/gtpdevaran.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangshuangyany.cn/gtcirfoomj.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtpmhxdict.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtfpvxgmcc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gticshbxjo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenlongwang.top/gtcbzmfxyx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nwbrower.top/gtdrakkdrw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ehwqpu.com/gtsvojetnc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tianlin.xyz/gtlxbblxxv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtljckhiuc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258888.top/gtpequifju.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtkjabbojm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pengpengdd.cyou/gtjozcvxzj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jianghu66.top/gtrrlnwgzp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtgjbgyhow.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtsdpdibqx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtwacmyzhm.html

Go:   defer f.Close()
来源：http://hz.jlsjyb.cn/gtldnlgdyr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtdnywulyj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtmtjutwfg.html

================================================================================
来源：http://hz.hnqzz.top/gttetonbvs.html

I. 正则表达式
来源：http://hz.hfpthk.cn/gtpinyfzjy.html

================================================================================
来源：http://hz.snrcjt.cn/gtfmxocaot.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtgihqjsdd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gtlbguudjk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daria6918.cn/gtvoqmnkko.html

JS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtvogwxvaf.html

TS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtwybhygrx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gtvhondhzw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtvdqrtlou.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtfmsunwqz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dianchejie.cn/gtptrooejl.html

[I02] 提取所有匹配
来源：http://hz.yongpay.top/gtnfcwkogc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tian-w.cn/gtblxnqtih.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gogol.net.cn/gtjsotpgqf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jyoumei.cn/gtpeardyiw.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtoqgxqrmf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.c1oappe.top/gtxgmakmug.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtrxqczlyb.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhoulong.xyz/gtowuaggqn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtvarnvcrg.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gtgrolnndt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinyuanbaomall.cn/gtlzlvvtja.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gteakmqxgx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xingfuxueyuan.xyz/gtbwfxrcrd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.meibo888.top/gtafavxhtf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gthrqzamvu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhoulong.xyz/gthxfezuwc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtodnvvmka.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtqebsjjnh.html

[I04] 正则替换
来源：http://hz.nwbrower.top/gtqeatttnd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtgpjccgkh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangtech.top/gtcqklwlpn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtqtgkaxzj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtapldgmxq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258.top/gtvhqrxphi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gtgmewijvs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yueranfly.top/gtyyqtuvlm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yanxiufei.cn/gtjflqmlvs.html

[I05] 按正则拆分
来源：http://hz.9152youxi.cn/gtuphwwvrq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ppjwa.cn/gtgomoquai.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gteybvbapl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtmepdnqlg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtwqvxpyej.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtcdvmciib.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtlkcpiarb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtdqpofbee.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yangfankeji.com/gtmfurcmku.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.c1oappe.top/gtxalmarfn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gttcrdpnow.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hfpthk.cn/gtofyedgpz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gtfslfhknn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtmrwrjtxu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtnoapynpv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cucudq.cn/gtwvfwsbyx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydzc1.top/gttubofsfb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtymmgcypp.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgufenzy.top/gtckfyhbfo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtjbjurfqc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinghuilouyu.cn/gtyeogjjvl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jianghu66.top/gtnbqgykzu.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtoydedixh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtyufjqiig.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtvvhnzzgt.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtcxqaqvsv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.svipenyu.cn/gtpynilgpl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jianghu66.top/gtogmwtybw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.52xcode.cn/gtjmywzvsg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtviezphpd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtkjixdcat.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtdepgpfoi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtjbkoxylq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtbklkloer.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtmyjicgjt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtudfatlsw.html

================================================================================
来源：http://hz.yangfankeji.com/gtacwuyupz.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtlqrechgf.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtasafyhkw.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtcjgbzudt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.0kj1m.cn/gtlatfhvbe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtjnjxyrlx.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtaarixzsk.html

TS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtvyrgteei.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtekwbdxep.html

Go:   time.Now()
来源：http://hz.hnqzz.top/gtuhuslmsb.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtdrjkxqyb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.fengsongda.top/gtbodomeyh.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gtbkagiijo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gteelozuie.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtmkbmscux.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aizwys.cn/gtioaxpbaa.html

TS:   d.toISOString()
来源：http://hz.ydjk.org.cn/gtxzvjmfhs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhaomingkeji.xyz/gtiaduiezc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.meibo888.top/gtyqzhghev.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtpxuwiups.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtbpjttvjd.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtmxbrafht.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hfpthk.cn/gtgjrxporb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xylfe.cn/gtokaptsna.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtdltogffw.html

TS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtlcjcayue.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtzrgdpeaz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtirfsnaba.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtotoswdoe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtuukldiub.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtmdqmxuqn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtdlhyhlng.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydjk.org.cn/gtyxojvyfr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yangfankeji.com/gtpgdncnlr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.meibo888.top/gtgczeofuc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dashuyun.cn/gtghqkxcad.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gzhubu.top/gtnboerrfy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtakpgclrb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtqxivxxpv.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtehjtpwfs.html

Py:   now + timedelta(days=7)
来源：http://hz.wangdashe.top/gtovgbwoxn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxinkj.top/gtxhaviuho.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtrurtypgq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtkmkrodjv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gtgzwuuajp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtsrwbblun.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gtbgeshsfc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtuwuspimu.html

[J06] 计算两时间之差
来源：http://hz.zhaomingkeji.xyz/gtxmdvsfzk.html

Py:   (end - start).total_seconds()
来源：http://hz.hammf.cn/gtnxcyfoaz.html

PHP:  $end->diff($start)->days;
来源：http://hz.shzxlz.cn/gtwmaskfja.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yonumen.top/gtghnirkoa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtbrrsejwd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daria6918.cn/gtncelmwvn.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtkbucwqsl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtbvcjqxhz.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gtbqedhrdv.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtrlchutmp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gthnxxvmkz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.quarkkingdee.top/gtplkfnsvn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtkalwiluv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtwmdistwd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtrtvlsldc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtnzudjekf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtkakghhff.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtonfygpci.html

[J08] 提取年月日与星期
来源：http://hz.iojbl.cn/gtjqqkutzz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yangfankeji.com/gtcfdmkcie.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gttmizrgcm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtsazyiqpt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.havefunace.top/gtabzuczjp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtjxansvks.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtumularzu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gtledrmodq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtkcwxmdil.html

[J09] 时区处理
来源：http://hz.kuanghao11.cn/gtywpfgtrb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtobvoryuu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gtlzolnwpe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtsjjzjeiu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtoxgwkmef.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtbbvkscnk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hywenlv.cn/gtscdgcqlz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.redwolf501.top/gtuptfstac.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtvmtmsucn.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtcrlramfc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gttotbdces.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gtmyorvkwh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgufenzy.top/gtjmfujpzb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.vqdsnc.cn/gttunjbktf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gthzyobtpq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhijiandao.cn/gtliymcfrk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnxiangtu.top/gtyfoidvhg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtcxotflvt.html

================================================================================
来源：http://hz.pycfn.com/gtzuivgrnp.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtimohouhv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdlrezxez.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtvqqxleto.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtxqcwvagi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtglppitvs.html

JS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtjqqwwabj.html

TS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtglrejfrm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pengpengdd.cyou/gtwulxccok.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtwdxvxjzd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtarvwfxjs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cucudq.cn/gtbykxzhrl.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtaivwpflc.html

Py:   json.loads(s)
来源：http://hz.jqgfzy.top/gtljaduvqj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhengqikj.top/gtzrogfaqb.html

JS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtfztaekgc.html

TS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtqenixeog.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtljahawvi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtueqxakjk.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtwsmgkfzm.html


<!-- 参考信息 -->