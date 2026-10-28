代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtnzjqehuo.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtnwkzqzox.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gthgdguozb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gtxgejduku.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtdwvwpcbc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtrfarypim.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtwhxpgtcq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtamkautfg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258.top/gtibzeutxq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gthpnbyxsv.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gthqolrdsf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gtlqqptdgq.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gttqvrrwsx.html

JS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtgzmanjtp.html

TS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtjxxgigzb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtnqhoqhrk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gttxhqannv.html

Ruby: obj.instance_variables
来源：http://hz.gotoacloud.top/gtaifjatbh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtrzcjhlqx.html

================================================================================
来源：http://hz.aizwys.cn/gteueavmhe.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtezkbjqsm.html

================================================================================
来源：http://hz.ivvv.top/gtypyjvsqb.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtnivandhh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtzbxobzkw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sufxvd.cn/gtdckhtbik.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gttplljfcz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtlofyqiza.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gtncqnjtqc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhengqikj.top/gtuejiptkn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtognwmrpo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gtzhkhbqii.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gteorldtrn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtxsebmjah.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gthqfxrhyt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gttqlvplba.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtmwnkpvvz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtlbcxxvnv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.meibo888.top/gtwicouxfm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ivvv.top/gtvjmuwrvd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.iojbl.cn/gtrgsgdsue.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtvmuirhja.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtvqewapyo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtickgwkpk.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtsdogeohh.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtdmbinvzj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtqzuwtfcb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtvkqfpyvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhiwuduotai.top/gthtrxksar.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtsllzgpcw.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtqrfnyfpg.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gtynrzplpc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gtdgyxxleq.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtbaiugnov.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtdxhhqqsa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtucwjvjvw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shuidangran.top/gtpskumtqc.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxuanxn.top/gteegjglws.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtycvrusvz.html

[H05] 捕获特定类型
来源：http://hz.nanxuanxn.top/gtmrpqljhn.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtnfoobqha.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtslpuczce.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtwwvwxvko.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtlidhajuz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydzc1.top/gtdjlkslgp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pycfn.com/gtqgilvmwz.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtviukeuth.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtviryvoma.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yueranfly.top/gtkeupirpg.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtpixgndwd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yongpay.top/gturqgkitg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtlinwdbli.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtwjnqbczx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hysaishi.cn/gthzfphqrb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtdgzstpyd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yanxiufei.cn/gtkptinfcn.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhoulong.xyz/gtqpqkxlcb.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtqcnydcqk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtftqwxync.html

PHP:  assert($x > 0);
来源：http://hz.iojbl.cn/gturwvfpsp.html

JS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtppjzhxqa.html

TS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gtyqmpmoed.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gtunkmjbgk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gtskokcuur.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yvedp.cn/gtfsdzbkam.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtyvdizhzw.html

[H08] 获取错误信息与堆栈
来源：http://hz.iojbl.cn/gtbujjzuaf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hysaishi.cn/gtajjaxhfp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.kuanghao11.cn/gtnypsapzt.html

JS:   e.message;  e.stack
来源：http://hz.gotoacloud.top/gtcjsilzxp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuanzx.com/gtmtzideyg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gthtyoyawb.html

Go:   err.Error()
来源：http://hz.birdmap.top/gtctfyedmb.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtuyzjnmzg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtzvdnzymt.html

[H09] 带错误码的异常
来源：http://hz.wangshuangyany.cn/gtppwmxpcg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yonumen.top/gtwnpoyfld.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtoqqffqny.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydzc1.top/gttkrnomiz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuanzx.com/gtwwsofjqg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.meibo888.top/gturlptiow.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangshuangyany.cn/gtytyudgcv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yonumen.top/gtcqxggrcd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ppjwa.cn/gtppcevhgp.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtwfeljxmo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gttkphbnlf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtgujizkjd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtfoendode.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtzyhjywac.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtcgqxawhj.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtvorepsbd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xylfe.cn/gtlvvobwfh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gtaptmefmd.html

================================================================================
来源：http://hz.dashuyun.cn/gtrgarwbxc.html

I. 正则表达式
来源：http://hz.daxiang520.top/gtzrzqhbyj.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjiqepzqu.html

[I01] 判断是否匹配
来源：http://hz.hfpthk.cn/gtuzgvaoqq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tianlin.xyz/gteuijdyup.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtuyiwrxxk.html

JS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtusdjslhd.html

TS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtsfkfpmus.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhengqikj.top/gttkipjeqp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhengqikj.top/gtkwmmyxxz.html

Ruby: s.match?(/\d+/)
来源：http://hz.cheryme.top/gtospkpxop.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtjrtziqlv.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtlpixruzs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtrivcujlb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gtmrfqlpuc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtjuwlpdwf.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtwsublekn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydjk.org.cn/gthcgspwmn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ehwqpu.com/gtqshoqzts.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtivrvprpm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtdeuqdolx.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtcrmascet.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtzmrwccgz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtovbpqoyy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtkmnrhnan.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.52xcode.cn/gtazegqsub.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtrzwupwdz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtfkjcqxlv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dashuyun.cn/gtrdpjczbe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtvxgztimc.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtdfmwebyi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gthryuljsd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtvklohmqe.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtecmbermm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtnjzmsjay.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.0kj1m.cn/gtievmefzc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shangyingyoupin.top/gtzowwqoqp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtfzqqqqbg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cqqwz.cn/gtdvsrjmxa.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtglnczksd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtmdcdiqum.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtzumrorah.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtrhnfhcgp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtzkwnmnls.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxuanxn.top/gtxgmnsyid.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.snrcjt.cn/gtsucpgozi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtrgdilliu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtoekrwvpt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sweek.top/gthismhfoz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtsvogngtd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtryzzhqdd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtofjguexq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtgusumlji.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.vqdsnc.cn/gtjihtcjfp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtlucqdgwg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxinkj.top/gtudvhichp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtsaucqhzd.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtelhbbuzw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtqurgiccc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gttddcbuwf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jianghu66.top/gtktafebiu.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtgismktbl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtgbglczvh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtjgepuesl.html

Ruby: s.scan(/error/i)
来源：http://hz.jlsjyb.cn/gtfpdyfjzd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtrvzymlie.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtupsyiqfg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gtgkbbbals.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtoiwbvncu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenjidiqi.icu/gtvlikujcn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtuywluhuz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtbiilefcg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtpgbycijj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtpxpeduva.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daria6918.cn/gtyndnktbe.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfwxagfij.html

J. 日期与时间
来源：http://hz.pycfn.com/gtpcrbidlo.html

================================================================================
来源：http://hz.hnqzz.top/gtqfuzkvkm.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtjpnzkiks.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtjqpjzqkf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtfpsdsdro.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtrhdhzuxa.html

TS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gttpebluzc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtytwuewge.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtfhjizlfr.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtcomaandv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhijiandao.cn/gtvtvsnxen.html

[J02] 格式化输出
来源：http://hz.shangyingyoupin.top/gtmiebvqhn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtbqgkmjor.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtypqnxnib.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuanzx.com/gtcoiyumad.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtmwbmjhki.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtdrzabmqf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sweek.top/gtywmabmdp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtxvokopld.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtiqxxuqjj.html

[J03] 字符串解析为日期
来源：http://hz.gogol.net.cn/gthymmpsvq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtyrztqbax.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shzxlz.cn/gtbbkptutd.html

JS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtcsquemxw.html

TS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtxiixvhva.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtmbmcyhlg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gtarkavzoj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtnvtpkwyd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtbxgliqvt.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gtihttsysp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yueranfly.top/gtdzlfwnrc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtdfirrwpg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtvypflhih.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigfzy.top/gtyhdibieo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtymidvbhz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtfdvbdlgh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtcnfwouwo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guannengcc.top/gtenjwabjr.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtfspfmpke.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gttrkfpudv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gthpumstwl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gthpoiaoje.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtmktnltrs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hysaishi.cn/gtsmlyctrd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtqbluyxnq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtlkfjinfo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.snrcjt.cn/gtbjpnvxkq.html

[J06] 计算两时间之差
来源：http://hz.zdqjudy.top/gthvssnjid.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtprqwntat.html

PHP:  $end->diff($start)->days;
来源：http://hz.gaohongyu789.top/gtqfhhzpbw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtprikcwrl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hysaishi.cn/gtornxmseu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinghuilouyu.cn/gtshjulxhg.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtfixpbdlu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xingfuxueyuan.xyz/gtnpmhkdyj.html

C#:   (end - start).TotalSeconds
来源：http://hz.tianlin.xyz/gtzxtmsyct.html

[J07] 比较两个日期
来源：http://hz.hfpthk.cn/gtdexqzzdy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtbmahjnlh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.haohaochexian.top/gtirsrkhyh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gttxnihtbu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtpubnfyna.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtmmomtspu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.birdmap.top/gtioizmxrv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtlsakhwoe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtycfhypnm.html

[J08] 提取年月日与星期
来源：http://hz.sysykeji.top/gtxozzsuqn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gthfzsgmth.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigufen.top/gtiwtzgcmm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtieyrcmlc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtcwxqteum.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sweek.top/gtvnftxzcl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigfzy.top/gtigbewpdc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tanke756.top/gtntkxoqfz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtsarynqkb.html

[J09] 时区处理
来源：http://hz.xuanzx.com/gtpbbedoen.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daxiang520.top/gthodiusjn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtpujjysjd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtwpbesuqu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtihberqwv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gttagduaxv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtimarzhbt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.birdmap.top/gtnpnlpxho.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cucudq.cn/gtqbqmmtqe.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtdcguobkv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnqzz.top/gtptpcrwhe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sxryk.cn/gthqqipsoe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtkpqfmctj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtppxkmbka.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gttykdgdkr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtxvhmbqxv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hfpthk.cn/gtepjrakji.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnqzz.top/gtupddmpbj.html

================================================================================
来源：http://hz.fengsongda.top/gtxudioxvu.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtylickgad.html

================================================================================
来源：http://hz.cheryme.top/gtcbkpqhrg.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtwvzxhxfl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtydowqhfx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtrbtfpvgv.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtkeaqjtiq.html

TS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtiazlymgi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtzucfuaod.html

Go:   json.Marshal(obj)
来源：http://hz.fzhhl.top/gtiemfwnsi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yongpay.top/gtizuibgxk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtswrquwen.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtoevkwmmw.html

Py:   json.loads(s)
来源：http://hz.gotoacloud.top/gtwkqcmezx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zdqjudy.top/gtalytepin.html

JS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtfftjozvo.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtjvrowswx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sysykeji.top/gtcehjikfg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtbhyjymqp.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gtorarshur.html


<!-- 参考信息 -->