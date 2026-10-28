代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtvxdqmnxp.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtwxcivsrr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtgdrgorxx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gtcyicbpfq.html

C#:   record User(string Name, int Age);
来源：http://hz.zdqjudy.top/gtsrxnrbpz.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gtuoyujvqa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtutjpxubf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hfpthk.cn/gtutcsoeym.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuxming.cn/gtjesihntc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtheokjvce.html

Java: enum Color { RED, GREEN }
来源：http://hz.aizwys.cn/gtabmpcozu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gtbtcvnvwv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtfzoatgqg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gthgqxauhr.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gtmaarpmgb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cucudq.cn/gtmfkzjinf.html

PHP:  get_object_vars($obj);
来源：http://hz.zhaomingkeji.xyz/gtbamioavs.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtbttvgddq.html

TS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtupeautzw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.0kj1m.cn/gthmtpkbmz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jyoumei.cn/gtuvdbqhud.html

Ruby: obj.instance_variables
来源：http://hz.snrcjt.cn/gtbqknfnbc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shangyingyoupin.top/gtyccbxdmv.html

================================================================================
来源：http://hz.cqqwz.cn/gtiwwjizbk.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtsbmefymz.html

================================================================================
来源：http://hz.ppjwa.cn/gtxmeuizvo.html

[H01] try / catch 基础
来源：http://hz.zhongyouzk.top/gtxklgmizi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shzxlz.cn/gtmguhuyfc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtlmrblfih.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtqayzoubx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtqajexdhd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtahcdxvus.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gtdwbryzof.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtaddkahln.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtcohtuyrd.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtuxvffnhl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtiadywror.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtkksmyzng.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtgxojlxoy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtovkogziz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtzibwahfs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtgnwoixfi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yvedp.cn/gttsiaracq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtzsoptkih.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtzdmccbue.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxuanxn.top/gtxxzaojwh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtqrllcvyr.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtttoahzyq.html

TS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtfghthbmm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtwmeodoln.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cdnleiting.top/gtvollqffo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jianghu66.top/gttuqpepzo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gttmizrazs.html

[H04] 自定义异常类型
来源：http://hz.zhaomingkeji.xyz/gtystrnbgo.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigufen.top/gtfdlfnpzj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.9152youxi.cn/gthbngvtlc.html

JS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtbsceiyzz.html

TS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtlfrlplcf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zycfv.cn/gtteeqolta.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangshuangyany.cn/gtaagvizqj.html

Ruby: class MyError < StandardError; end
来源：http://hz.dianchejie.cn/gtuiccnvgr.html

C#:   class MyException : Exception {}
来源：http://hz.zdqjudy.top/gteisjmhps.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtvzxddmqb.html

Py:   except ValueError as e:
来源：http://hz.ivvv.top/gtlngivxoc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cqqwz.cn/gtfsgrgyzu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtaleabdio.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtwehymehy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtpvgwqmty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtaswpcwmb.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gtexdzzdtc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gthfslfmyw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangtech.top/gtiojfsslj.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtigjzulbm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gtoxszhkfs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtywsyzibu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gteptcryvx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtgqwlmpjl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtorewgzea.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tian-w.cn/gtnkwvnpmc.html

C#:   obj?.A?.B ?? default
来源：http://hz.yvedp.cn/gtqymtfipu.html

[H07] 断言
来源：http://hz.chenlongwang.top/gtydolqwgl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtmgprmbmt.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtkpqxkzyi.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtakfmrtfr.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtuvmzeuqh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.snrcjt.cn/gteaoufxcx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtdxpebyew.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtnuwgtuem.html

C#:   Debug.Assert(x > 0);
来源：http://hz.bjfxy.top/gtnvhyaolm.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangkeji.top/gtangmcegc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtevwnefbd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtpfcaocun.html

JS:   e.message;  e.stack
来源：http://hz.ppjwa.cn/gtxgvjibys.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dashuyun.cn/gtmlqcrxsn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtvxazhyia.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gtnvbxlkgt.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtdunrpuya.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtnovvezuk.html

[H09] 带错误码的异常
来源：http://hz.yvedp.cn/gtyqzwnhoc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtayubcaiv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtlbugllcc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtqtntnrhs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gtlblbgvel.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gtonzzcfaz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yangfankeji.com/gtrwawpbwc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtzgspyfcp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtbvygcegx.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtcmojhqao.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gtblpiohiq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sufxvd.cn/gtrlfyosla.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtzmxsklxh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtdwvwbsvn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shangyingyoupin.top/gtehjdsqth.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtrvygssec.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gtsdrijata.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shangyingyoupin.top/gtezlkxupj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqmnmnaoe.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtekywhzzb.html

================================================================================
来源：http://hz.smart0.xyz/gtlolnptpi.html

[I01] 判断是否匹配
来源：http://hz.ybcxt.top/gtkuyvghyq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.bjfxy.top/gtxwgnalyf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtliytivox.html

JS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtdbsvxqum.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtwaihbscm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtxycgjsqw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gtmsirtlzq.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuanzhike.top/gtmehcqyll.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtnfvuagwa.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtkeknmcco.html

Py:   re.findall(r"\d+", s)
来源：http://hz.9152youxi.cn/gtjrnwdkmq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtbrzkgohk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhixingplan.top/gtgpwfxzbb.html

TS:   s.match(/\d+/g)
来源：http://hz.daxiang520.top/gtakushfcm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hammf.cn/gtnitzbwpr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtmkpxbzga.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gtmlrkgycj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daxiang520.top/gtsrabqcog.html

[I03] 提取捕获分组
来源：http://hz.aibaodan.cn/gtmqxdstds.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtgmoonagk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinyuanbaomall.cn/gthwclfumd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuanzhike.top/gtzfrdarmw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hysaishi.cn/gtggkvjgqn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigufen.top/gtmafhkdqo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtwwrfavvh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydjk.org.cn/gtwlpukebq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtitthbwfi.html

[I04] 正则替换
来源：http://hz.nwbrower.top/gtfyvuqsfg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtlzivswrq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtnbxaqzna.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtedclrtrm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtmisjgrab.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtiryxbhhd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ywan-chungtsiang.top/gtwwyftifi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hfpthk.cn/gteabpkzvz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtbsigurzo.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtzwpafgmx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gttptragok.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gtkghpuvem.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtmysuxzif.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtchjjqzjr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtzgtnplvc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daria6918.cn/gtmhifcqim.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtpxbxwsev.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gtqegsmteu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtdtcbmgeb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtmwgmjudv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinyuanbaomall.cn/gtpuouthib.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtpxtwuavo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtyayrkdaa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yangfankeji.com/gtljoacfck.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtfzyxvhmy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.kuanghao11.cn/gthpgibjhe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtwcdxsjkb.html

[I07] 忽略大小写与多行模式
来源：http://hz.gaohongyu789.top/gtvkcnlwwg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangshuangyany.cn/gttdlmprft.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtivyzieue.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yvedp.cn/gtexrkaxru.html

TS:   /error/gim
来源：http://hz.zhiwuduotai.top/gtsqwctdhk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sxryk.cn/gtglruveyn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtapywjhik.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtyzgnegxw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtfhjsddqb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gtnaqidlsc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtrgbegebi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtwvulurvt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtvaqavhpf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtiwzihrym.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sysykeji.top/gtiuewnkkc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtgtsyoyea.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gtqsbpdoas.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtnwykfhuj.html

================================================================================
来源：http://hz.tanke756.top/gtvjpgnkrr.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtsjsgdlrp.html

================================================================================
来源：http://hz.9152youxi.cn/gtubpknftr.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtvkooilzq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.haohaochexian.top/gtefwpnxyz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtxftzrckh.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtjhwcyuia.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtlkiwxbmk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtwzculwgm.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gthcpqynqn.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtkshnxavy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtarnqirev.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtkguxvgks.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtwzncyhzx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtzpzajgme.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtqzjwkhdt.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gthvrwymwx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtgngvbzbt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shuidangran.top/gtccjyulcw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtnhhuqrwd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhongyouzk.top/gtzlecuecu.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtkyzakfgg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gtwypeswca.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtluaihqjc.html

JS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtzzcmpmsv.html

TS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtxemejasv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtysotjibf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ivvv.top/gtxrwwjsqv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj202588.top/gtxatesdda.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gtiuyfdjai.html

[J04] 时间戳与日期互转
来源：http://hz.tanke756.top/gtxxzfvhjx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtubwjanfa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtnfeancyy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.9152youxi.cn/gtsicdvuim.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtahvbtlnc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hfpthk.cn/gtvbspfebh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cheryme.top/gtrginslal.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtwrewtgos.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtwzzuczps.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtkpxoskox.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258888.top/gturhlaymr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydjk.org.cn/gtxtntfovl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtvwdalmqg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtvqkrhyzl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hysaishi.cn/gtwcpcifqt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.iojbl.cn/gtpiiqazbh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tianlin.xyz/gtyzegavrd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gttwzxjfdy.html

[J06] 计算两时间之差
来源：http://hz.hywenlv.cn/gthgoabxkb.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtbwnhwkea.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtgdvksucp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pycfn.com/gttxmgcnkj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtoaluxqsa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gthpftdfaj.html

Go:   end.Sub(start).Hours()
来源：http://hz.vqdsnc.cn/gtedsjadsc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigufen.top/gtnsomrjki.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtbdmsrlfc.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtikaukryt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtbylrtqqh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtzmkjwbyr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtbdnbetbq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtuceumiff.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gogol.net.cn/gtvbkpmnww.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtyhxvfuld.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtqdqhmjwh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtxjkdnnjd.html

[J08] 提取年月日与星期
来源：http://hz.yongpay.top/gtehegyolh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtszmcmhcm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ppjwa.cn/gtpsmapjzm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtbanqsatk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtvhizbgfg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shuidangran.top/gtvstdjosn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hammf.cn/gtsrsxvpnr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtogawuzjh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtioriiqho.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtzvzhsqjd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtccyzchmi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtbcbfkfeh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtpdgylycn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtlkuaffix.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtbuzefgmn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtvemwaajv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gtbyzflpqu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtzddjrsbg.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtdouznuuw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zycfv.cn/gtrjldjaiz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtxtneliwp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.52xcode.cn/gtyjqhkxiv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fzhhl.top/gtkchlsoch.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxinkj.top/gtktpxyque.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtadcmbwfu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtyxsljwgu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtlzzllwnw.html

================================================================================
来源：http://hz.jyoumei.cn/gtgvljpkxb.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtvkpcvwab.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbcsmteyg.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtauomhsox.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtdhkcymhr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtrgiwtnrw.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtktbmevjg.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtwlrogwgc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtijgtmqdd.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtnxdnwwol.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtybnkkiji.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtrbbgjypl.html

[K02] JSON 字符串转对象
来源：http://hz.zhoulong.xyz/gtsbqglhrq.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gtdyajnszm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtqyhbpbhs.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtqhlyvtkk.html


<!-- 参考信息 -->