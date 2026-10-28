代发 wailian999

Java: u instanceof User
来源：http://hz.zhoulong.xyz/gtlngrfdmx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gtctjcojgn.html

Ruby: u.is_a?(User)
来源：http://hz.jiagoushi.top/gtozpvqaxx.html

C#:   u is User
来源：http://hz.pengpengdd.cyou/gtlhagjuol.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtkznmxjtc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yonumen.top/gtntwltplb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sxryk.cn/gtbimrmuex.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtwrjtvysg.html

TS:   type User = { name: string; age: number };
来源：http://hz.svipenyu.cn/gtwsmnvieu.html

Java: record User(String name, int age) {}
来源：http://hz.tianlin.xyz/gtccwcbuxx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtkkmwosbg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gtmjosyxoj.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gtpzraxiqi.html

[G15] 枚举
来源：http://hz.yj202588.top/gtdoddekjo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shuidangran.top/gtkdvlwjau.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtpxarcbvc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gtlaqikbzb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gtphcnlutx.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtfrbziivd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.c1oappe.top/gtyfbeaggq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tanke756.top/gtinzswjtw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtxjbnxxzm.html

[G16] 对象转数组 / 字典
来源：http://hz.gzhubu.top/gtndxqblbq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtibctxhli.html

PHP:  get_object_vars($obj);
来源：http://hz.mhx1999.top/gtnburgxbd.html

JS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gthjyrweyf.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtsghxucvr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sufxvd.cn/gtreprpdim.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gtglmahwlz.html

Ruby: obj.instance_variables
来源：http://hz.quarkkingdee.top/gtjcliulrp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.redwolf501.top/gthmttkwfo.html

================================================================================
来源：http://hz.jinqigufen.top/gtybxlxtxu.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtywimrsto.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqewfubet.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtcnwxrfnx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtrjetejvz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.haohaochexian.top/gtxezwdfxe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtaebfqqlj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.bjfxy.top/gtbhifrsaw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shangyingyoupin.top/gtlwsrcopp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shangyingyoupin.top/gtxfcbcgla.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinyuanbaomall.cn/gtfzfmzjqx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtjivapkzz.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtvyzzkqgi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtkttaujbv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtutmfqbxp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtvdzthrmb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtrqizlfdg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gthydszhpk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fengsongda.top/gtxpabhset.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cucudq.cn/gtbgmbaloe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhixingplan.top/gtvzkdatge.html

[H03] 主动抛出异常
来源：http://hz.hysaishi.cn/gtpogwixrr.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtoiutidrz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtvlfxucss.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtxmqwudak.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtyjvkbonl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtnxubkzag.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.haohaochexian.top/gtydmpvbor.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtlfpkifis.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtvzroxutn.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gtekizhqfy.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtivzbnfxw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtdfoxxdhj.html

JS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtaxatgnnx.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtdyngovck.html

Java: class MyException extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtafivjwjw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.birdmap.top/gtroiioqrr.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtlvzmwvez.html

C#:   class MyException : Exception {}
来源：http://hz.hywenlv.cn/gtsadbrdwy.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gtmfuaavmx.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gtfbxqgehn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gttcuaxjqi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtvxhwaxxl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtiwvszjxo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhongyouzk.top/gtxcnnrbka.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtskpewdrs.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gtuaasycwh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hfpthk.cn/gtvdurgybf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigufen.top/gtrdiayvma.html

Py:   value = d.get("k") or default
来源：http://hz.dianchejie.cn/gtilsrgdss.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtjdbdirxl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gttcdllnah.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gticbpirie.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtjsdrexxs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gttyipmyzy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtajihklvm.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtllicatyz.html

[H07] 断言
来源：http://hz.havefunace.top/gtskgcasjq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.meibo888.top/gtvtlbrdjt.html

PHP:  assert($x > 0);
来源：http://hz.jinghuilouyu.cn/gtoxahvzcc.html

JS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gthpwpfuvc.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtykuvwgci.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtyisfqfom.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gtryruvmhn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cashguo.top/gtxgswpuac.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gtmniiqtvp.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtfotzckmr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtvkzneouf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnqzz.top/gtqpiggsmn.html

JS:   e.message;  e.stack
来源：http://hz.jianghu66.top/gtncscfwys.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.quarkkingdee.top/gtnxyyxero.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtfoqzhqeo.html

Go:   err.Error()
来源：http://hz.xylfe.cn/gtmvskfkxf.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtevukjwef.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtvcewiedu.html

[H09] 带错误码的异常
来源：http://hz.cqqwz.cn/gtssadsfuw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangkeji.top/gtngbpndxg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtisabqajk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtkruwyahe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pengpengdd.cyou/gtlrqnyxbv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.feifeiyinyue.top/gtgockthos.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtdofjgsqe.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtnirajljn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtwzqswdag.html

[H10] 资源自动释放
来源：http://hz.ivvv.top/gtamobniol.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gtycweumde.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtbuensugt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtjgpmxtcv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtofqnkila.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtevvikodg.html

Go:   defer f.Close()
来源：http://hz.sxryk.cn/gtowwdtpmd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gaohongyu789.top/gtnnerjkkc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtqseecafw.html

================================================================================
来源：http://hz.jyoumei.cn/gtimpymrnj.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtfcftkslr.html

================================================================================
来源：http://hz.tanke756.top/gtlbeffqqj.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtthnonago.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtpmhvkhvz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gtrmsdzvnt.html

JS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtlbyvpruh.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtcdjkbeyu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtdtcqiqdx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtzsyribhu.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtuabtnhxk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gtmgtmvawa.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtsgjvscqw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhijiandao.cn/gtfgexkrgf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtsdjyomcx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guowangkeji.top/gtvpvdrclv.html

TS:   s.match(/\d+/g)
来源：http://hz.zycfv.cn/gtwthiewrj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtmfetnsob.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.aibaodan.cn/gtgzmraabx.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtcdpsadgg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gthwhhddva.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtgfrgapfg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtaduefnkz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtnofdmhxc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.haohaochexian.top/gteyllmfmq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cqqwz.cn/gtrtiylfzs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtlcgbrago.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtacpkcmdn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtczokyoqn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtdhpuxflu.html

[I04] 正则替换
来源：http://hz.pycfn.com/gttfptsjes.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangkeji.top/gtvdszjhnt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtnwzpvlld.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtxgmbhqwx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gttuupjeph.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtzstgqsys.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydjk.org.cn/gttihnvjsn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gtkiopmlyy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtwvjjxavp.html

[I05] 按正则拆分
来源：http://hz.ydzc1.top/gtlvrpiuwc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dianchejie.cn/gtwupnmahr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydjk.org.cn/gtmjjjmlnj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtsezatsuv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtostqkyns.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtrntacjts.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangdashe.top/gtocmytcsl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtqdcrhxhg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtlvvxjnzo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gthxonggla.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtiofhyiep.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtzpvkvpkb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtkjittkwv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtjvolpnkb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.meibo888.top/gtfpfumfdp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtplrfngmf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenjidiqi.icu/gtmgqskgig.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtkwlzqrhn.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtpvqetdyr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258.top/gtsnijwbaq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtplsvpfvj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuetiantiany.cn/gtzwhbfwgz.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gtospncric.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtwymmibob.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtbqtciaxn.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtwjceukmn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtfrjwbqhc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhongyouzk.top/gtlxghtbzn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.birdmap.top/gtkrbhsvby.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtwufvplgo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtrjztgpct.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtirgmwlbi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ybcxt.top/gtndkkbxfz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtokkomeev.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.snrcjt.cn/gtzvilzemo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sysykeji.top/gtaamddpfy.html

================================================================================
来源：http://hz.jiagoushi.top/gttimaytuo.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gtgkvyqzkz.html

================================================================================
来源：http://hz.sufxvd.cn/gtqvyvsuxf.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtipidqumo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daria6918.cn/gthasfcjbm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtxgrcifpo.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtbfipszzn.html

TS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gtirjpaisd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtzqraeemk.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtqlitvluj.html

Ruby: Time.now
来源：http://hz.xinyue.icu/gtvywuyswp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gtdvworkci.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtrtjsdjnk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtnjgqslpp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtjoltcwce.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.kuanghao11.cn/gtlynykklj.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtcfhxmuxt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtfolgsfuy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gteukishqi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtnuthledw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gtmvsvzjpe.html

[J03] 字符串解析为日期
来源：http://hz.zhengqikj.top/gtnbojhkab.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtyvcndpno.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtvgbntrfa.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtehmjzsqh.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtujvkufdo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtejmcsndp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gteydjtbwo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ivvv.top/gtqiporsmn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtjhencndk.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtllqpxmtj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yueranfly.top/gtvqgrxcqa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtdsicowby.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dianchejie.cn/gtrspwgwta.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtyeesrodv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtilmjjiov.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuetiantiany.cn/gtdzlcijpp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtraadhimf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhixingplan.top/gtapnayyop.html

[J05] 时间加减（加 7 天）
来源：http://hz.hysaishi.cn/gtticglkbx.html

Py:   now + timedelta(days=7)
来源：http://hz.tian-w.cn/gtfjyssthd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtqmtotqhg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtsgeuxsrr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtclmanopb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gthqqbvaqs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gtdylvfbqe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtpljmcyla.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yongpay.top/gtlmyrymnr.html

[J06] 计算两时间之差
来源：http://hz.yj202588.top/gtxcrdvgbr.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigfzy.top/gtensrcscm.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtrrzxtrsv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtaqmyjrme.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hysaishi.cn/gtqwocrqpk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtntrtcanc.html

Go:   end.Sub(start).Hours()
来源：http://hz.shuidangran.top/gtjitmjwjc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtksifhbme.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtrvpjkgkj.html

[J07] 比较两个日期
来源：http://hz.nanxinkj.top/gtarrpelyv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtsxolmwjs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuanzhike.top/gtwyausyyj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtzcpnwbxb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtliowuyhh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtgjupdsrt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gaohongyu789.top/gtubjezucj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtcpgrylua.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtjizvvxti.html

[J08] 提取年月日与星期
来源：http://hz.cdnleiting.top/gtsbswaitl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtytvmsccg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtwohplevh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.9152youxi.cn/gtgrwjfviz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gtryaphhqi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtckciiwhv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtuyvmcifr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtimuidvmn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cashguo.top/gtzgprkoft.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtfwhzdhbr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtbzyikhid.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.vqdsnc.cn/gtifgxjgsq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtbvmhfoab.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtkkiweunp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sxryk.cn/gtuwtgwvlf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gtrrcuonvx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gthjlfomnp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtxztwulys.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtgmrllaiy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtuhunmdnt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtcbtniatw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.andypj.xyz/gtchayezzd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtquxlzdpf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.meibo888.top/gtdcozpfez.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtaonpxbiw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shangyingyoupin.top/gtbkmvydto.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtzlmhnbwd.html

================================================================================
来源：http://hz.ydzc1.top/gtdypuokex.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gthtvmsrzo.html

================================================================================
来源：http://hz.gogol.net.cn/gtnoefpnni.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtiffirmuw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ivvv.top/gtycgbxoht.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtiwqyimzp.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtuaorggri.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtxtfgttaf.html


<!-- 参考信息 -->