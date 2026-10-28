代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtmmjgtnso.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gthxmyzuvj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gthdzwmcik.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtrqwaxckn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtmoibetmc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtvhjccsxg.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtpmnpjxfd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gtestvvxcw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ppjwa.cn/gteiuahtni.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtmtmapqll.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gttpxvmzgz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtrdprnobc.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtpffnvpux.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtgglamypc.html

TS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtyaikuykm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigufen.top/gtevlnfhtp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtgtkzccxs.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtcqxrlgjh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtpcqyzlgm.html

================================================================================
来源：http://hz.yonumen.top/gtgivnhhmh.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtlapvckcb.html

================================================================================
来源：http://hz.tanke756.top/gtmbvhxroi.html

[H01] try / catch 基础
来源：http://hz.shzxlz.cn/gtxhjqamml.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtqyhwsgfl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aibaodan.cn/gtxkeaexyj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gteiehnvbi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtkxoinjbg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guowangkeji.top/gtjpefibmu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtrkervzfk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuetiantiany.cn/gtefiflira.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shuidangran.top/gtjcdmxitk.html

[H02] finally / ensure 收尾
来源：http://hz.mhx1999.top/gtbatimufz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tianlin.xyz/gtpzlsyeuh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtnfweyybc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtimogbmva.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtjudtjctu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtsgewwcin.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtnbgkskuf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jianghu66.top/gttcqkpxoo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gthtxyqbzo.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtgbumdnwo.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtbwrhhypz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj202588.top/gthkmnnoyo.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtimcqbabz.html

TS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtnlxttfzg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gthvmmouxl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhongyouzk.top/gtetctokej.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gteoqebfsq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtoztyymuh.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtoafkphez.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gtvqefriux.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtjkqivroh.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtvvcqzpfb.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtdxmqtrrj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtmhzajgzv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nwbrower.top/gtvvvibxmk.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtpxtkjkbm.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtnyngoeax.html

[H05] 捕获特定类型
来源：http://hz.316326.xyz/gtbmrijuft.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gtkdxjxfrn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.meibo888.top/gtfavzgtes.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtbigffwva.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtwkmzntlp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtiugnpaft.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yvedp.cn/gtjafctepo.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtsmeuthen.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jlsjyb.cn/gttlwgdeye.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtqkkxrkwi.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gtfjlatekm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.0kj1m.cn/gtbmikqkny.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtxpgahani.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtjboldqoh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yonumen.top/gtnrsxfrxb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtcutztcmt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtjjvkhurl.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtuwgyvtxg.html

[H07] 断言
来源：http://hz.bjfxy.top/gthocrnolw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnxiangtu.top/gtoxjyjwuu.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtwgfsajld.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtglpoxwpn.html

TS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtnefmffzl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.andypj.xyz/gtnjvkeqvz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jianghu66.top/gtrdvcrgee.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangtech.top/gtqjcfopca.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtbauybgcq.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gtceitxgup.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtjxliwgyc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangdashe.top/gtsaihbaoy.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtovilwdql.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtuvydhssd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuxming.cn/gtemvzplpm.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gtodnxwbpe.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtndihaccf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guowangkeji.top/gtuvwibwhm.html

[H09] 带错误码的异常
来源：http://hz.hnxiangtu.top/gtqdoabknx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shuidangran.top/gtqkzksgii.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtyhzxnkef.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yueranfly.top/gtzdwlkysx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.mhx1999.top/gtmkvvwakv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtmtaxavcr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtgxabmyfl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtweqotcdp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daxiang520.top/gtxkiejukb.html

[H10] 资源自动释放
来源：http://hz.jlsjyb.cn/gtgwubprto.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gtosfljisp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenzaomai.com/gtnxapabwy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtfautnoyg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtjulbfsdh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jlsjyb.cn/gtwlwnyrio.html

Go:   defer f.Close()
来源：http://hz.sxryk.cn/gtcpnntwwb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtwkqkxrnu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ppjwa.cn/gtfyzilaxf.html

================================================================================
来源：http://hz.zhengqikj.top/gttwpuizgc.html

I. 正则表达式
来源：http://hz.ybcxt.top/gtrdvhnazg.html

================================================================================
来源：http://hz.yuanzhike.top/gtzwxtmbdh.html

[I01] 判断是否匹配
来源：http://hz.hysaishi.cn/gtfeggzraw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.c1oappe.top/gtcawfyeqv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ivvv.top/gtkyobobea.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtxldhjmdw.html

TS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtwyaldffm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guannengcc.top/gtkflyxcps.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgufenzy.top/gtdoeyybth.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtlpyqhpav.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.316326.xyz/gtxsiylzck.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtcwhbjhxw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258.top/gtptkwfwun.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.aizwys.cn/gtqwqexcnc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.52xcode.cn/gtfattipgf.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtlwxramhq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gteclavinz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtfifwvaoz.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtckwtbmhx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ehwqpu.com/gtzzpwjzak.html

[I03] 提取捕获分组
来源：http://hz.kuanghao11.cn/gtcvgusxte.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtijjcgwmq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hywenlv.cn/gtzvxkekxj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtiymadcnh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtxqjdvwph.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hysaishi.cn/gthccswxfs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yongpay.top/gtsfsoofsu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtnneaaxts.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.vqdsnc.cn/gtddllosgc.html

[I04] 正则替换
来源：http://hz.316326.xyz/gtbtusjfnn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yueranfly.top/gtlhxkacwz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtdipfjcjv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtrnxkcsiq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtgrnnjvkf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtsorukwoa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtoguvousx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtsscginwj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtndcncuxm.html

[I05] 按正则拆分
来源：http://hz.meibo888.top/gtgizpbkmz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtnjtyedrz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aibaodan.cn/gtpywjdkle.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtvotebjmk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtkqbdtztg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtmttpiola.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sysykeji.top/gtfkczixtm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtjmgjkrrq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.feifeiyinyue.top/gtaqojxnwt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xingfuxueyuan.xyz/gtjeivaljy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtmjisegtv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cdnleiting.top/gtvgpqondk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtwpqhjxvs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtlltxguna.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ydjk.org.cn/gtqdypkbnt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258.top/gtnxfnyugg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ivvv.top/gtfquwawmq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtuemdqwed.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtbcmtfsqm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtvxukrafx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtentncvvo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtfrbblpjs.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtfdulzeaa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangdashe.top/gtauuzjadc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gtvfevsliw.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtbinnemsp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangshuangyany.cn/gtzineugqk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.redwolf501.top/gtjpgcmejg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hywenlv.cn/gtiqlpckuw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtprjuvjbt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtcgjscxzs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtemnifrmd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gticubilhq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtgysrbgpm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtzcsftsau.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtqjhaukco.html

================================================================================
来源：http://hz.havefunace.top/gthgvonglh.html

J. 日期与时间
来源：http://hz.nanxuanxn.top/gtrgafrfpu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjhdjwzmt.html

[J01] 获取当前时间
来源：http://hz.wangdashe.top/gtbtahvnzv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtpaemobbc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtrqaoonno.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtahxysoxh.html

TS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtjibwqhze.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtczankxcp.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtkffmvdum.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtszqqpmhe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtiybztioh.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gthfakqqfa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtrebqzecz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtpcopjqko.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigufen.top/gtntvlppkm.html

TS:   d.toISOString()
来源：http://hz.xylfe.cn/gtgqbeumij.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnqzz.top/gtkohnhfha.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtdifqndsh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtesfhkmpu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gtluwdwipo.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtlixxdqoe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dianchejie.cn/gtlazgmpms.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ivvv.top/gtexmhgeql.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtxdbvazeq.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtsiyliwpg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtxheiidsb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtacuxzkjs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtqljqpfou.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gttmpxjxnk.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gtselvumco.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtwnhetzky.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jiagoushi.top/gtvkcddkbd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtccnkccur.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hongshengwenyu.top/gtaazqqgsa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtmfsoqycf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtzsugvbkr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gtwrcpbmlo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtnitwpnfp.html

[J05] 时间加减（加 7 天）
来源：http://hz.xuanzx.com/gtzvyniaxt.html

Py:   now + timedelta(days=7)
来源：http://hz.jlsjyb.cn/gtlmhlyezn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtaibjnzoi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtqasdnpmu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtvkfqeguo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guowangkeji.top/gtoesrrzdw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yanxiufei.cn/gtjriquasu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtceomvjer.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinghuilouyu.cn/gtcpnnfuww.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtrsagdxtv.html

Py:   (end - start).total_seconds()
来源：http://hz.zhaomingkeji.xyz/gtzjtzuzuf.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtabzlbabm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuxming.cn/gtljmabfzf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtsqmsvvzl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtpwkygnld.html

Go:   end.Sub(start).Hours()
来源：http://hz.jyoumei.cn/gtjceofqoi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fzhhl.top/gthsnqabls.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtbkaqyroa.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtnokewkfl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtkjbtkaul.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinyuanbaomall.cn/gtlicjvoff.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtadtyrygm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtnxbibqml.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtgkccpidf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.mhx1999.top/gtzualkpxa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtoyfoawph.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtjgrifzse.html

[J08] 提取年月日与星期
来源：http://hz.tianlin.xyz/gtrwytqcto.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gzhubu.top/gtcjhmklhf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.iojbl.cn/gtqmwfqcng.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtoicwlnkf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gtzzwtwagj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtwgadhuau.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj202588.top/gterrahvnj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtazbovfdf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtubgqnadl.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtkbyjbxsy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtzjwujzjt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtdthkvnlj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtgzdytiix.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtmhsznejn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shangyingyoupin.top/gtgvgxskvw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtukzekbfc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.wangshuangyany.cn/gttxesnzhd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtuzaurjkx.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhiwuduotai.top/gtpkgcuhsu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtqcfwuoyh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxuanxn.top/gtpniywuks.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.316326.xyz/gtdsbrnydm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtuqcqnjxx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guowangkeji.top/gtegbttzbj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtiilwqznu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhaomingkeji.xyz/gtlkkmcedl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jiagoushi.top/gtfjrbqnqx.html

================================================================================
来源：http://hz.hysaishi.cn/gtgbzfawzj.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gttgrnbefw.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtpwxtrkos.html

[K01] 对象转 JSON 字符串
来源：http://hz.c1oappe.top/gtemdpnyjc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtfzzawlce.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtddcblewh.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtkxqzxvww.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtkgpcbulz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtppfziabs.html

Go:   json.Marshal(obj)
来源：http://hz.cucudq.cn/gtdptlwyny.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenjidiqi.icu/gttaptvrfu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuanzx.com/gtxwzfyqwq.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtylcnzhtm.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtvaxppdqh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtccgqpkha.html

JS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gthohqcuzo.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtgicfhzxe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtienmtnie.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtbxgklnke.html

Ruby: JSON.parse(s)
来源：http://hz.yonumen.top/gtmnmxdkiz.html


<!-- 参考信息 -->