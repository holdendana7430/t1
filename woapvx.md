代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtokrtdtgq.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtgktdecxl.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtbbfijhda.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gtttktdtdc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtpomltezt.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtvpsdkhkq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cashguo.top/gthgdozybg.html

================================================================================
来源：http://hz.dianchejie.cn/gtugaqjake.html

H. 异常与错误处理
来源：http://hz.yueranfly.top/gtfxvdxdwn.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgavibrvq.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtyuepllda.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtmmdgpobt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtieomzrmq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuxming.cn/gtpcopfxfs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtknxyqbeh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.redwolf501.top/gtygopvzuz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.redwolf501.top/gtfgtuizjr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtjmbremrt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtezmjuced.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtbmuyemqw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hywenlv.cn/gtpygvqfvd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtqpxxagkt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtrwygcmal.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtuyhecslg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtltetshrg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtygkyyctp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtukoijdbs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtqlwggmhe.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtzlmbigww.html

Py:   raise ValueError("错误信息")
来源：http://hz.tian-w.cn/gtiuvpxoxq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtkajowpra.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtgfjlchux.html

TS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtqrfkjrtq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtekgdgtnf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shangyingyoupin.top/gtqgcczrwl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gogol.net.cn/gtulptpymk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gttldcaakb.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gttdrijrbz.html

Py:   class MyError(Exception): pass
来源：http://hz.redwolf501.top/gtnxxdddtk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtuwwlxfkf.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtbesqlzlf.html

TS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtjefogcfx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.iojbl.cn/gtekrlhuri.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtonybmcma.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangshuangyany.cn/gtkugclzol.html

C#:   class MyException : Exception {}
来源：http://hz.hongshengwenyu.top/gtdhzqqcot.html

[H05] 捕获特定类型
来源：http://hz.tanke756.top/gtxeiqmmtv.html

Py:   except ValueError as e:
来源：http://hz.ppjwa.cn/gtascxgtyn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtcaooutfh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtqlciamgc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtetkabjzu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtaejefmce.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtahkbegob.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gttvnvwkca.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtabghwtcs.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daxiang520.top/gtyatlyujd.html

Py:   value = d.get("k") or default
来源：http://hz.daria6918.cn/gttlvgkfio.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.52xcode.cn/gttxkejezp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gthzcfcaeb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtbtazljql.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yongpay.top/gtggdhxeka.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxuanxn.top/gtkmlqatho.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtajkkhxid.html

C#:   obj?.A?.B ?? default
来源：http://hz.birdmap.top/gtcceknujm.html

[H07] 断言
来源：http://hz.sxryk.cn/gtohtpksjg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zycfv.cn/gtvuectobe.html

PHP:  assert($x > 0);
来源：http://hz.jlsjyb.cn/gtnvsujffl.html

JS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gturasuylw.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtbquyrjfy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hammf.cn/gtjypvyrnu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gthuywprcv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guannengcc.top/gttrtmrusa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtbppfbznv.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtndogwqch.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xylfe.cn/gtrngmpsjc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangshuangyany.cn/gtktvwnebf.html

JS:   e.message;  e.stack
来源：http://hz.zycfv.cn/gtdzikyqjn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtnmvgujyt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhongyouzk.top/gtgnqggxpr.html

Go:   err.Error()
来源：http://hz.sweek.top/gtomaghuqo.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gthjutlska.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gtsofqdhmb.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtvgtlmaid.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuanzx.com/gtzpkdfkrp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gthnvvhnli.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ybcxt.top/gtddjulaxo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guowangkeji.top/gtfpkgzhfl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xylfe.cn/gtvopjtqmh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daria6918.cn/gtqebgaaiz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guannengcc.top/gtsklqbyre.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yvedp.cn/gtukepdnhl.html

[H10] 资源自动释放
来源：http://hz.dashuyun.cn/gtcgyhyxrn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxinkj.top/gtdgrkfrif.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtysatpthr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtvijrknay.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gtlthezthk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hysaishi.cn/gtqpkjtsxq.html

Go:   defer f.Close()
来源：http://hz.yonumen.top/gtdzhbddfm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nwbrower.top/gtqfqunvjk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenlongwang.top/gtnkeifeve.html

================================================================================
来源：http://hz.zhixingplan.top/gtiuwarszi.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtfkvgqxlg.html

================================================================================
来源：http://hz.ydzc1.top/gtyfwnprqm.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtcnjltqdw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtbwpxfbpr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtokmfhttn.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtjxpbqyeq.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtsxzchwse.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgfzy.top/gtyrdjexrp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gtllpwszta.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtmmawaqrf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guowangkeji.top/gtfsrqfgxg.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtsgbgjssa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtosjmzaso.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtxicsxitq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhaomingkeji.xyz/gthmfdjjjm.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtsqctnspc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtqnuliehu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtlkvuvhjo.html

Ruby: s.scan(/\d+/)
来源：http://hz.birdmap.top/gteyjvuefb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guowangkeji.top/gtfsryhlzb.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtazlebauv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sufxvd.cn/gtxtdckeid.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fengsongda.top/gtzasyvivn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtczokgyyy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtwsbyjvfy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtauwtghja.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cheryme.top/gtcfiozqul.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhengqikj.top/gtyyixnlag.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hysaishi.cn/gtxinrlnbl.html

[I04] 正则替换
来源：http://hz.jianghu66.top/gttvmolwrl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gtnzkmicto.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtqpgvxgri.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtzktantfy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtxvplhalf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gtzdlxsrkp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtplpeuuhw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xinyue.icu/gtnglhxyuc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.vqdsnc.cn/gtpqjlrikp.html

[I05] 按正则拆分
来源：http://hz.havefunace.top/gtyxmfcgct.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhijiandao.cn/gtdhpgjnqc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtmdkmjoom.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtwvwkibax.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gthpprgbnn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yangfankeji.com/gtfrbqvolf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gtvxtoealz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtceynliqt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtewrqgexd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gtmhatfdtg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtivejfsty.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinyuanbaomall.cn/gtwcvztaii.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtapmkueub.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtvztuxqej.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtoebprpoe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gtqmluzoqi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cashguo.top/gtlrwzvkpm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtdamrhxcu.html

[I07] 忽略大小写与多行模式
来源：http://hz.birdmap.top/gtuvzlmjvk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtdmdkltjz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhongyouzk.top/gttvkblecn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtxadqnepp.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtcoeorugl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ybcxt.top/gthjjcxqnj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.meibo888.top/gtlxkcrzom.html

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gtzvtuangf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ehwqpu.com/gtwruymhil.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtnaxlgdfo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hywenlv.cn/gtyfjnflmb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtcdifqbdq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtjphrgnup.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtfusiemcn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtqkegvjgg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtkwjmykim.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtuhmfbvop.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtlkgjxhws.html

================================================================================
来源：http://hz.fzhhl.top/gthlvzjoqg.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtkuupdkte.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxphsocuv.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gtgtvzxyzg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gtnvyrlwvj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtkykjbavm.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtelaoxgug.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtnxundjww.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yangfankeji.com/gtkmjxlhle.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtjwzykkqr.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gtckvdtadm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sweek.top/gtrcdlxfmt.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtrkyxhdks.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtrdcpkgzb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtvhgbhlus.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtqdkinyqw.html

TS:   d.toISOString()
来源：http://hz.haohaochexian.top/gtclvrdhhs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtlipgonwu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtqltjwhav.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtafayjabg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.svipenyu.cn/gtogekvjli.html

[J03] 字符串解析为日期
来源：http://hz.tian-w.cn/gtxbjhtzwb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gtwpxyshmj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtekkrpfkr.html

JS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtvdrapjgm.html

TS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gtikrgcuki.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gthmjrvwxw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtvxrbkqcf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtllikbnhz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gzhubu.top/gtmhxsiift.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gtbyfcyzxk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cucudq.cn/gtzpvxhega.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtexivjpxt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtfptuhnkf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sysykeji.top/gtuqyojkcm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gttmwbnrkh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258888.top/gtkeafceyz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtzdlzlyus.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtlskgwkfk.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtnnzdilfl.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gthqvognsh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtskjpblrt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gttjxlkhfl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gttahsbvku.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fengsongda.top/gtnuppsfpq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gtesfzctbw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gtwksqgjat.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ivvv.top/gtypndbjdf.html

[J06] 计算两时间之差
来源：http://hz.dashuyun.cn/gthcjsdjeh.html

Py:   (end - start).total_seconds()
来源：http://hz.aizwys.cn/gttksypgur.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtufpopwkz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtdjbiadrx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtvgoxazmu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gtlpsylwnp.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtducklhuo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangdashe.top/gtkwtmkgpf.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtdbjhdynj.html

[J07] 比较两个日期
来源：http://hz.yonumen.top/gttfvgbmqj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtovhkflyy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yvedp.cn/gtssavmihk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtxofvpovh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtcxvpywrv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtpcoazmvu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtdhiploqb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtfwztzthf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtgynlduni.html

[J08] 提取年月日与星期
来源：http://hz.ydjk.org.cn/gtlerwnimi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258888.top/gthrweiaif.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxinkj.top/gtribdkyci.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtwjxutmav.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuanzx.com/gtdwrwutke.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuxming.cn/gtqgfquiql.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gtrmndlwhf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ppjwa.cn/gtxtawhdgq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydzc1.top/gtsvtfdnir.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtttilkulk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gtwwbvrvdj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtzuskhslf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtuzabqxwq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtgjwoespq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtvknxtcia.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtjecmrzcf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtpyzzesub.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtmcwtfxmx.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtaiayttqj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtavvtdjtm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gttuvbzxsh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hfpthk.cn/gtakvewlcs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtvzoeucyg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtidescryg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtoetcthaz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.quarkkingdee.top/gtyincwfey.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtoteyngjg.html

================================================================================
来源：http://hz.52xcode.cn/gtzalwvbtx.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtswrgwsjj.html

================================================================================
来源：http://hz.ppjwa.cn/gtecisjrll.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gtcofimrge.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtkdxxzrlw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtomsfbbdm.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtldyyrhik.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtakefqehm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shuidangran.top/gtfvuaiuyq.html

Go:   json.Marshal(obj)
来源：http://hz.xinyue.icu/gtlqrovpmm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.wangshuangyany.cn/gtwxjptsap.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtrmtnlchu.html

[K02] JSON 字符串转对象
来源：http://hz.sxryk.cn/gtamcrfdnl.html

Py:   json.loads(s)
来源：http://hz.gzhubu.top/gtcjuigxmz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtcrfsgvsb.html

JS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtosfnzvef.html

TS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtxtubhrgl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtfkwkcjyd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtbowjozfo.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtlvhlwnry.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guannengcc.top/gtzrxgyllc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shanyushiyangkeji.top/gtbwipyzhw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtryhcaydm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gttpbnegep.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtbyvvjbvg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtrbdwbxyb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jyoumei.cn/gtccnixtjk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gtbxwnstog.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtjhafngqt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hongshengwenyu.top/gtqhxxntss.html

[K04] 读取 JSON 文件
来源：http://hz.cucudq.cn/gtphrxymjr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gttrqgdqcg.html


<!-- 参考信息 -->