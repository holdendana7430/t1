代发 wailian999

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtkgagprfz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtggtmnxqw.html

Ruby: u.is_a?(User)
来源：http://hz.hnqzz.top/gtqzeyxzyu.html

C#:   u is User
来源：http://hz.xziqi.cn/gtpedpbcob.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtyhxwulbk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtwdrjffxz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dashuyun.cn/gtdyrrydnf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenzaomai.com/gtnhiboixp.html

TS:   type User = { name: string; age: number };
来源：http://hz.yueranfly.top/gtkvvrdjkq.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gtckshqvhi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtsuyywanb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jyoumei.cn/gtzhrkihqy.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtmnvtnrwd.html

[G15] 枚举
来源：http://hz.kuanghao11.cn/gtoftvelkn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gttpvdydxc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtxjwhfoxw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtuwuxbdjv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtojmzpqme.html

Java: enum Color { RED, GREEN }
来源：http://hz.guowangkeji.top/gtxojbufyk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jyoumei.cn/gthfvqrnbu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinyuanbaomall.cn/gtpxfcinfd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gttqegxgxg.html

[G16] 对象转数组 / 字典
来源：http://hz.zhijiandao.cn/gthlhuvekl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gtwydpldqz.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gtdcalsqbh.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtsjycnhfk.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtvnvtaqnk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.redwolf501.top/gtvkeywjrl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gtucjbzgay.html

Ruby: obj.instance_variables
来源：http://hz.yuanzhike.top/gthflkispu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenjidiqi.icu/gtvdvvmxaz.html

================================================================================
来源：http://hz.sxryk.cn/gtqgwlhdsx.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtannkguge.html

================================================================================
来源：http://hz.sxryk.cn/gtzlfkqqwi.html

[H01] try / catch 基础
来源：http://hz.guowangkeji.top/gthkwbjvea.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gthfvwfuhd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.svipenyu.cn/gtwrgktpjj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtucpemegj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtwtutuofo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtanhdwjzc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtfcqedhsq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtnyydgpzq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtgnofsnxf.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gtkpuhhsuh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cucudq.cn/gtbkruuzee.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtwdffcnpy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtmkvwaomy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtttnyzwwz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtwzaiubxs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtvjubkgqd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.mhx1999.top/gtfspgtzft.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zycfv.cn/gtbybpugdt.html

[H03] 主动抛出异常
来源：http://hz.tianlin.xyz/gtkeekvzsw.html

Py:   raise ValueError("错误信息")
来源：http://hz.yongpay.top/gtnfaisjqx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtpclzcdjt.html

JS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtbphygnlo.html

TS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtjvaxlysi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xylfe.cn/gthluvgcxu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zdqjudy.top/gtvnlgzmlf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtnxrurmmv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtndvlbscu.html

[H04] 自定义异常类型
来源：http://hz.meibo888.top/gtcyuhgxhw.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtvjffiukz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtfyfgwqgw.html

JS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtcptfrfvd.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtxysukgft.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtfwpjvoeq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtwwyhqszc.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gttpsnjfug.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtnoiellqx.html

[H05] 捕获特定类型
来源：http://hz.chenzaomai.com/gttgkjyhyv.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gthkhkyjyx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daria6918.cn/gtojlrxysg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtatxkzggc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtxrolrmbl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gtoelepfgw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jyoumei.cn/gtxfddlaci.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtywfktlkh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gtxieohwqc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yangfankeji.com/gtzfdfcldh.html

Py:   value = d.get("k") or default
来源：http://hz.hfpthk.cn/gtwfgltsve.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtuoaniidf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gthoywgiiu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtgltlgmvk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtjizitira.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.haohaochexian.top/gtcauremux.html

Ruby: d&.dig(:a, :b)
来源：http://hz.birdmap.top/gtrtebzroz.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtqlqquiwp.html

[H07] 断言
来源：http://hz.wangdashe.top/gtholcrkdj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xingfuxueyuan.xyz/gtveiungly.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtsayuzicf.html

JS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtlilaomky.html

TS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtbyzjmxvv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtxyqlxjne.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxuanxn.top/gtgbshghwe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cheryme.top/gtnwyzihom.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gogol.net.cn/gtaoablets.html

[H08] 获取错误信息与堆栈
来源：http://hz.xziqi.cn/gtuctpgbzp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtnkolgsdo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dianchejie.cn/gtbkfvmpyk.html

JS:   e.message;  e.stack
来源：http://hz.hywenlv.cn/gtqwedulpn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtfeaxqwkv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hysaishi.cn/gtswxgemlt.html

Go:   err.Error()
来源：http://hz.dashuyun.cn/gtqzrniduk.html

Ruby: e.message;  e.backtrace
来源：http://hz.hfpthk.cn/gthiontpli.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydjk.org.cn/gtdbiobtir.html

[H09] 带错误码的异常
来源：http://hz.chenzaomai.com/gtdyutyovw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gtyozwgfow.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.birdmap.top/gtbkyjhewq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangdashe.top/gtmsmbmihp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenjidiqi.icu/gtvvaxngny.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cashguo.top/gtqpnvgdar.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aibaodan.cn/gtajnispte.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhijiandao.cn/gthrmrllfb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtrqfkzomh.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtlremxwgs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daria6918.cn/gtvtmyjskl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtfbijvapv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtyupaxknu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtngtllakj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtbezsqjno.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtckmwbwia.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ehwqpu.com/gtixysjmur.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtkpigiakg.html

================================================================================
来源：http://hz.ehwqpu.com/gtpavidvup.html

I. 正则表达式
来源：http://hz.316326.xyz/gtrxheqiuh.html

================================================================================
来源：http://hz.sweek.top/gtfttgaaju.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtiidtymnv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhengqikj.top/gtyswopnmh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gtmqpolrhz.html

JS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtxsoodouy.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtquuzwutx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.haohaochexian.top/gttwlslcua.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.mhx1999.top/gtzkunafci.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtptjyijmr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jiagoushi.top/gtbkoiceep.html

[I02] 提取所有匹配
来源：http://hz.cdnleiting.top/gtttphhmpd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtfhjltwtw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtyrcocqhb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hammf.cn/gtvixqknad.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtyekhmljb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhiwuduotai.top/gtsictzqrf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxuanxn.top/gtwfoitixu.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhoulong.xyz/gtyddzdavw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtrruthmvy.html

[I03] 提取捕获分组
来源：http://hz.zhoulong.xyz/gtqgcnlpvr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtopxthetq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtqzsuclpd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtyjchfadn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.vqdsnc.cn/gtpwvlxqwr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gttbkegawm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.0kj1m.cn/gtgtiyaplp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gttxuodcbq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.havefunace.top/gthlfimuut.html

[I04] 正则替换
来源：http://hz.svipenyu.cn/gtfnpkrqcm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuxming.cn/gthpeamgcn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtuwkrpdeg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtkqzaprfp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtkdwgqwyi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj202588.top/gtthpnipnr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtmzbjiuzs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtsrjdofnh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zycfv.cn/gtefxahznb.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gtuqwbdsjj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangdashe.top/gthudgsdyo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zycfv.cn/gtqaxbjoxj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtekiteuts.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtylbaspvt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258.top/gtxodfsdvy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.mhx1999.top/gthtdqpstc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtbghphuzx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtxetrxosi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtkytehrjo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtjnmaeypr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258888.top/gtyoljqjza.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gthnsgngzv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtxkdebrle.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hywenlv.cn/gtevszjrjh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtigayruih.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shzxlz.cn/gtwidyegfi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtyuuchdjt.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gtxdjkahim.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cdnleiting.top/gtqehhwwex.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtlomipvvu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.9152youxi.cn/gtguzsyjff.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtmntnfzyf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtfvryhehn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gtqowiwmvw.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtdmricyox.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shangyingyoupin.top/gtwbaftffs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtnbnycpys.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gtissvqghj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gttqnuuudz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtqyajhvjk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtfutfqlve.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gtqaijebft.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fzhhl.top/gtcwawhndd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtppwgcbql.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.redwolf501.top/gtvmlclszx.html

================================================================================
来源：http://hz.xylfe.cn/gtdteedyzz.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtaudhfgzx.html

================================================================================
来源：http://hz.jianghu66.top/gtlbpxwawb.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtmnmtjzyp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tanke756.top/gthwkyknbw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtltbcsmao.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtjygxjitn.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gthhcrvlsi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtvtkywdtn.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtjklolxtr.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtrrwvqwbb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtdntzpmws.html

[J02] 格式化输出
来源：http://hz.jlsjyb.cn/gtchwglxag.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gticdzeeww.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.mhx1999.top/gtvbeyfwgm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtiapuzqcz.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtatumgero.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtbhmalytd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gtydzepuoi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtkcnuoocy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dianchejie.cn/gthwfugujl.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtynvvjukw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgufenzy.top/gtpwtthmse.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yongpay.top/gtyvrjcula.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtzehczzzh.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtegrgltmi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtqavxwnxf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangshuangyany.cn/gtqhqfvmwd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tian-w.cn/gteuourkde.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtqkejmudz.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtvuptfeqk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.haohaochexian.top/gtjbelqede.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shangyingyoupin.top/gtmrpsqbsk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhengqikj.top/gtjaagtlvo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yvedp.cn/gtfozedukk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtdbdvyuvh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtwqhlwaic.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hammf.cn/gtjpsiakhx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydjk.org.cn/gtdutrvmcw.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtlnvifaqa.html

Py:   now + timedelta(days=7)
来源：http://hz.zhixingplan.top/gtcmerbsva.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtigssxrmf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gttoywveuo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtxxrxrpfm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtqodbvbkj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.9152youxi.cn/gtvqzvpend.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtiinfjonr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtcsfkzbct.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gtsjrdsifs.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtongtlbgj.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtapqppfjx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtonefkrrk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hysaishi.cn/gtohuhtmnd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtvkyicilf.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gthkzjomvf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtzzdvhdxx.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhongyouzk.top/gtbcyusdoc.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtgpwwyzme.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtwcfnrrmo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sufxvd.cn/gtcicyqcyd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gthotyqdre.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtrdkhbalg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtilixmzji.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtmlpwqfuz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtvwzoblzr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtabchcqjc.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtcpbtuzxh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangkeji.top/gteeujuafu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gthblejjyf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtfucyeigk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gtigkixmfw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhaomingkeji.xyz/gtxbudqhnf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.redwolf501.top/gtlflplzcr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhongyouzk.top/gtryxcklsn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.feifeiyinyue.top/gtbhszgsdm.html

[J09] 时区处理
来源：http://hz.svipenyu.cn/gtrbjpsgke.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhoulong.xyz/gtgsnxargo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtwhjfulxq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gttzcxolza.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtcaitmfhv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtryouehnb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtsfjlsluk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aibaodan.cn/gtwzgmdixk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuanzx.com/gtracqqmey.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtluiswwwu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtjuhpvttf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtbxgrqhkr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.iojbl.cn/gtlyryotnc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gtqjejosfa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xingfuxueyuan.xyz/gtseaqjhdd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gtpzlkrvxw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gtskcomxyj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtwjvltrhz.html

================================================================================
来源：http://hz.hywenlv.cn/gtycvgyzbc.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtwpxwfwow.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtjqeksxxu.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtzomhaxwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtjghljqkc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtwpujmvrb.html

JS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtkpscmguh.html

TS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtsnzfxgoe.html


<!-- 参考信息 -->