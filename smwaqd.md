代发 wailian999

[G14] 数据类 / record
来源：http://hz.xuanzx.com/gtpjbrsamg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigufen.top/gtvjcmklpu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtrxnnazee.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gthkjcchvf.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gtwmbbtwpy.html

Java: record User(String name, int age) {}
来源：http://hz.cashguo.top/gtbzmpdpms.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gtpllakyjz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxuanxn.top/gtbbvltbbe.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtslxgxoos.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtrrgqnxox.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hongshengwenyu.top/gtxakgouol.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sxryk.cn/gtfwjnmjzz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtmgupsfgx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtizacucsw.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gtxxvxclko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtteuuuquq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yvedp.cn/gtkjyzrksy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtsghumuwl.html

[G16] 对象转数组 / 字典
来源：http://hz.dashuyun.cn/gtyitmldcj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pengpengdd.cyou/gtvgrrdeno.html

PHP:  get_object_vars($obj);
来源：http://hz.dashuyun.cn/gtzmfkytbd.html

JS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtddikfoce.html

TS:   Object.entries(obj)
来源：http://hz.sweek.top/gtuzeuhxty.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hfpthk.cn/gtherybusv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gtfjbavrfi.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtfezzdpgp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhoulong.xyz/gtpjnrkiqu.html

================================================================================
来源：http://hz.xuanzx.com/gtcptytxqb.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtihzfkyni.html

================================================================================
来源：http://hz.cdnleiting.top/gttjdhfygf.html

[H01] try / catch 基础
来源：http://hz.jinghuilouyu.cn/gtdyjbgxwj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gteszexpam.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jianghu66.top/gtfpcnwnwr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cheryme.top/gtktuddefz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtwscplnkf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtetqcglqx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtigpgbvbr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gzhubu.top/gtlscxmayf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtocsswrpo.html

[H02] finally / ensure 收尾
来源：http://hz.wangdashe.top/gtheswuqjp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtkjrneiyk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtnulwatpr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtrsxcqaot.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtwhaviqim.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtucytghhi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtmfuumyzk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gthkvldpjq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtonrsoryk.html

[H03] 主动抛出异常
来源：http://hz.dianchejie.cn/gtfibarcis.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtxryzidhq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtnqjluvkf.html

JS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtozmwmfoq.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtwimvrwwh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtpwkglsnn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgfzy.top/gtagbryozn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtnftftnyn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gtwswwprxd.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtorbnlfta.html

Py:   class MyError(Exception): pass
来源：http://hz.jiagoushi.top/gtycpjotqw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtroonucab.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtpejwuofo.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtpzjxavmv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtefmjlpum.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhoulong.xyz/gtslzqfstg.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtvzghhttl.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtyabramsq.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtssevevhu.html

Py:   except ValueError as e:
来源：http://hz.zycfv.cn/gtanirzxqs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gthkuncvyl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtftfwlbnf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtetvyqwaq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangtech.top/gtiymxhmvy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtjqxfaobi.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gtkxwssowj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gtfbmsyfls.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shzxlz.cn/gtkdjonltu.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangtech.top/gtntxyczuk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtvrnkxsbs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtdnfkoqcl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtuqavbpjw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jianghu66.top/gtowbjjcvl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydjk.org.cn/gtzskhrwqg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhengqikj.top/gtaapkfybv.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtmksygulb.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtywqqveaz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuxming.cn/gtxsebpzye.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtphkbwzvg.html

JS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtrfkkdxhm.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtfgsersjj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gotoacloud.top/gtmixxfuov.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtcpcpguem.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.vqdsnc.cn/gtucomembq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dianchejie.cn/gtkteuxdie.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgufenzy.top/gtpmevoyay.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gtrlckityq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtpenilbow.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtnnlxqkoj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhoulong.xyz/gtcnrwagyd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtcpyfblws.html

Go:   err.Error()
来源：http://hz.zhaomingkeji.xyz/gtqjnqnwua.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtzbxntcns.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gtrryxlsvh.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtkzvtlahi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cheryme.top/gtypdjlhqd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtgwcihppj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtnkfhdfbw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daxiang520.top/gtgdvrnxdz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtnvnszfds.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cashguo.top/gtqpvaegqh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtqrjtixar.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenjidiqi.icu/gtxdqnzftu.html

[H10] 资源自动释放
来源：http://hz.havefunace.top/gtedjzqczq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yongpay.top/gtxvogrbov.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtaomtfvlf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtolrmoufz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtoxtyfxmg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtfjwdisjl.html

Go:   defer f.Close()
来源：http://hz.xuanzx.com/gtznlxoico.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnxiangtu.top/gtxrkpuyhk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gtvumdtpnd.html

================================================================================
来源：http://hz.guannengcc.top/gtdesmblqw.html

I. 正则表达式
来源：http://hz.cashguo.top/gtggbzbfyp.html

================================================================================
来源：http://hz.shzxlz.cn/gttrkmtees.html

[I01] 判断是否匹配
来源：http://hz.ppjwa.cn/gtgxubxdmz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.bjfxy.top/gtpvyorcqg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yueranfly.top/gtqbyboavo.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtvuoyjdrg.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gttxsoohdp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhiwuduotai.top/gtnikxcevj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgfzy.top/gtvzrjnhsr.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydzc1.top/gtlvrfkmbe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ywan-chungtsiang.top/gtfqjbampl.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtnrzbvygx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtxniylrdw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtzawhqtvt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.mhx1999.top/gtnstsnzrp.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgufenzy.top/gtzedyfqsl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gthffjstyf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtpyqupxvk.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtzaqltesh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtwyrvmifm.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtytjegdvs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtpnpqtgyv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tanke756.top/gtdugxzmza.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xziqi.cn/gtkrrykknh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gtkbmbutdl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtlideaegw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.smart0.xyz/gtfblwojgt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gtdggbtyzt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinghuilouyu.cn/gtxpakuwlr.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtzjpuncpe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuanzhike.top/gtofchajdo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenzaomai.com/gtmdjchaym.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtjdmzcewu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtsgwzvbaf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gteocqebqd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ppjwa.cn/gtxkfhszvz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tian-w.cn/gtvppfgobr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtknugqsrx.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtximhnyll.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtfrihzvsq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gtrsusnoen.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtxsmltuet.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtjelpozoi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydjk.org.cn/gtyarbdhhc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangdashe.top/gtwejuywmn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtvzgeqrrw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtssjacsbe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gtwfjysxfd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtoehxehrv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aibaodan.cn/gtsbbjwrwp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtqlsydbao.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtvverytxs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtuhqnyavm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.meibo888.top/gtcxwtvvmo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258.top/gtztghvrmp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtuxsrozov.html

[I07] 忽略大小写与多行模式
来源：http://hz.0kj1m.cn/gtdkululfr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtfalzlsab.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtemfcuwnz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtgluomyhh.html

TS:   /error/gim
来源：http://hz.daxiang520.top/gtzjtmdblf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fengsongda.top/gtysfjfuqe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuanzx.com/gtvulvydjj.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gtmbrdcxgy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ywan-chungtsiang.top/gtndwhzzgf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gtfotgqafr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yueranfly.top/gtdlgiacrb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gthnmoemhs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtudggurfv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtufechgrk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtabuhrdxq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nwbrower.top/gtwfpkguha.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangkeji.top/gtsdbofnzt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gtxgkkjesg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrqiqsmms.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtzmenytcz.html

================================================================================
来源：http://hz.shuidangran.top/gttecttlfr.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtmfoykidi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gthsxkleym.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtyrhgoxlk.html

JS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtvkfovxru.html

TS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtnvlxlapa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtcbrlbydy.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gtkrslsxrj.html

Ruby: Time.now
来源：http://hz.gotoacloud.top/gtpxuuaftv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.meibo888.top/gtwfxnkxkj.html

[J02] 格式化输出
来源：http://hz.316326.xyz/gtjwvylvpt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtsuokwnqn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtfcivcywh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hongshengwenyu.top/gtpiuvdbsz.html

TS:   d.toISOString()
来源：http://hz.aizwys.cn/gtljqfrwjv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sweek.top/gtuxxrmejv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhengqikj.top/gtstsjjmxu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtvdzjqzlo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.feifeiyinyue.top/gtfcnfbghi.html

[J03] 字符串解析为日期
来源：http://hz.jinqigfzy.top/gtwfmclmap.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gtqmdkskmb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gthgseaioj.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtoendhkex.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtvwzrsxhb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtiplkkpvy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gtdpnjxuzo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtyvycgeiv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pengpengdd.cyou/gtlokdequz.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtnauqxydi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnqzz.top/gtmwgoqanj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tianlin.xyz/gtdbnsihii.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenlongwang.top/gtchqmfwul.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhaomingkeji.xyz/gtqawffoot.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gtyitnuhbl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtbtfegbgg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtkcxvmauu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gthuzaopor.html

[J05] 时间加减（加 7 天）
来源：http://hz.birdmap.top/gtteqxqttr.html

Py:   now + timedelta(days=7)
来源：http://hz.pycfn.com/gtirohjjed.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gtfegktjls.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtzpnzvqjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtzfoqcjus.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtmfotxpna.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtebjxdmgt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtiwfqwvfc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtxtmncoey.html

[J06] 计算两时间之差
来源：http://hz.zhiwuduotai.top/gtbjsbatqm.html

Py:   (end - start).total_seconds()
来源：http://hz.jlsjyb.cn/gtzdnynzlb.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtlhordsdn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.9152youxi.cn/gtkpsckoxs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daxiang520.top/gtnvtmakwd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtadehwfiu.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtltouibui.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtihvsmynx.html

C#:   (end - start).TotalSeconds
来源：http://hz.ehwqpu.com/gtymjrjtqc.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtpxavqkvz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtfuialwhz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhaomingkeji.xyz/gtjjmyoyor.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtjbsfgrkj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtlhvbvlmu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtqzxhavuy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtywphrfkh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtqhdbpbbo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtjjcvbtjl.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gtitjnqutx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhixingplan.top/gtpryarsro.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cqqwz.cn/gtmdhnukiw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtrisiepxj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258.top/gtzfgsoxdq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangtech.top/gtpvdfncrl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangkeji.top/gtlqkhfqoe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jlsjyb.cn/gtemrrwcdd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtdkybikvk.html

[J09] 时区处理
来源：http://hz.meibo888.top/gtnakinmob.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gtpgygzcbg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.birdmap.top/gtuybqnvcx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtojkhxtkn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtzsxszrlv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.0kj1m.cn/gtkgwrmzhe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtvllvrlhy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtykispnsk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yueranfly.top/gtnpqqpkrp.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtwternqfa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuetiantiany.cn/gtkeosxylw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuanzhike.top/gtorddmcwy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.birdmap.top/gtekuiqpzk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigfzy.top/gtfjntarpn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangdashe.top/gtqopduurf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gtpzghzpsq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtvyjnkrae.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtbmiifrfh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcnmyohgc.html

K. JSON 与序列化
来源：http://hz.jqgfzy.top/gtiyoubimb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfigfcdri.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtjzzbwajt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtyvakujsi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtotcjausn.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtqfikvkjg.html

TS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtdvvksdpc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangtech.top/gtvmcqyrwc.html

Go:   json.Marshal(obj)
来源：http://hz.hnxiangtu.top/gtxlhmeqyu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtonckkmvz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuxming.cn/gthnhvzsgf.html


<!-- 参考信息 -->