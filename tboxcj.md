代发 wailian999

Java: u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtzcdivvvy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtvcdmciws.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gthmyljjxk.html

C#:   u is User
来源：http://hz.yongpay.top/gtlrakhkjg.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtoqjygjjv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtgmytlqda.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtthmycrpj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sxryk.cn/gtgabvliju.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuanzhike.top/gtacxdrafs.html

Java: record User(String name, int age) {}
来源：http://hz.hywenlv.cn/gtrtgzijbb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tian-w.cn/gtdzoezeyi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gtkfanivhp.html

C#:   record User(string Name, int Age);
来源：http://hz.guowangkeji.top/gttqzfqsxu.html

[G15] 枚举
来源：http://hz.yj20258.top/gtqlgyhizw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gtqyviktlg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gttawenife.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangtech.top/gtzgxxxuzi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtrkoobpeg.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtpmsgoeof.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gtubyeomcp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtfqsigdsx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtcsemtnbc.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gththktjgr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuanzhike.top/gtajyedyvu.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgufenzy.top/gtlsqswrtf.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtoxwwgmdh.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtstqtbklz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yvedp.cn/gtdiuwaxvw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtzhogllvh.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtemtauhxe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtevrjfzfb.html

================================================================================
来源：http://hz.cucudq.cn/gtovrvnvvq.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtivjxbwyg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtlyikkdeo.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtpwspzywm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sxryk.cn/gthqettroq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgufenzy.top/gtbwgrxwnj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtcvkmmbif.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gtsymvorvu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtsprgneri.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtpxssdnml.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtixuaxogm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtrgvmpykc.html

[H02] finally / ensure 收尾
来源：http://hz.aizwys.cn/gtfinsuzhe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gtnjlqirrm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtrpbohyzq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtiqailgmd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtnwoatcjq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtzlkjkmtr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangtech.top/gtseqaladw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gteystxwrz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtxilcbuvf.html

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtdqcqzthx.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gtvnrsqmyh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtrbyhlumw.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtklqbhbhk.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtzfnsobek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtouyupxzl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nwbrower.top/gtfyrsnscj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jyoumei.cn/gtcjhegixm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtheaihzyw.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gtemaszkdy.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gtletmoooc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtjbrahvvv.html

JS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtbiyceqlz.html

TS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtldvvivzu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtbrloqciq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydzc1.top/gthiszdsnh.html

Ruby: class MyError < StandardError; end
来源：http://hz.c1oappe.top/gtvatiolpa.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtuwudqkmr.html

[H05] 捕获特定类型
来源：http://hz.nanxinkj.top/gtxxprhgve.html

Py:   except ValueError as e:
来源：http://hz.cdnleiting.top/gtzncjdhlj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtotnsnhen.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gtbzmhhpwe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtiepfyyjp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hongshengwenyu.top/gtaqiaxuei.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtjzbnldpy.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtzlvfyfuy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtbikbntcr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.0kj1m.cn/gtnpwbqije.html

Py:   value = d.get("k") or default
来源：http://hz.fzhhl.top/gtgnfforaf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258888.top/gtmayyhrhi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtqgcowxzk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtzsmruejx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sysykeji.top/gtppkcwecc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenzaomai.com/gtcayaspbc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtbaclyqzn.html

C#:   obj?.A?.B ?? default
来源：http://hz.guowangkeji.top/gtdzpvwaia.html

[H07] 断言
来源：http://hz.ybcxt.top/gtxdinfouu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.vqdsnc.cn/gtpeepciig.html

PHP:  assert($x > 0);
来源：http://hz.yj202588.top/gtognccrdj.html

JS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtooeasrdx.html

TS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtuzxixcqa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtwxcgjppp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shangyingyoupin.top/gtsyhnyxvw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtwzgedzjv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gtxmtukpwk.html

[H08] 获取错误信息与堆栈
来源：http://hz.daria6918.cn/gtsuxrtmbu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fzhhl.top/gtdemqihtw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtflnahvuo.html

JS:   e.message;  e.stack
来源：http://hz.ivvv.top/gtddgpstbg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtjmjjmdvz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtzgrmmkag.html

Go:   err.Error()
来源：http://hz.ybcxt.top/gtmijwcusf.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtoexioovv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gteqbxqvmz.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gtsfnovzav.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtmacjlglm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtncpphray.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtxoyfymhc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtdvpsvykh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtrdvbiwyb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gtbaejvalo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtchorqqim.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gttkxtqzsm.html

[H10] 资源自动释放
来源：http://hz.fzhhl.top/gtieugzdvi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtvnwwtrpa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenzaomai.com/gtfbafzxwt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtlzbvwiyh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtjgappryi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shangyingyoupin.top/gtbikflopp.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gteupsomjo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtmpwgpapo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yonumen.top/gttaydpcpc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtztgemgtt.html

I. 正则表达式
来源：http://hz.pengpengdd.cyou/gtirjjqkyy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtirdzezol.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtixijsobo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtnyqqnvbn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.andypj.xyz/gtoxppeoqw.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtdpuiwkbp.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtanxlncxb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gtscpqvbdv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtigzspcft.html

Ruby: s.match?(/\d+/)
来源：http://hz.iojbl.cn/gtjntlheey.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtriosxssn.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtcvhfjvaj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aizwys.cn/gtpurpxqsa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtkgadqacg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinyuanbaomall.cn/gtjyyuufpr.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gtaafsbdru.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yueranfly.top/gteoklfbpn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinghuilouyu.cn/gtriarwfhs.html

Ruby: s.scan(/\d+/)
来源：http://hz.guannengcc.top/gtxodlkfwh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhoulong.xyz/gthjzmnhhl.html

[I03] 提取捕获分组
来源：http://hz.yangfankeji.com/gtdyfscihc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtorlxycbi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zycfv.cn/gtqwovsksi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jiagoushi.top/gtzkvxzmtq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gtsogzufvd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gttzsrjqct.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258888.top/gtrcaechxm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtxumtujya.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtwdayhknw.html

[I04] 正则替换
来源：http://hz.pengpengdd.cyou/gtxexanqjr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtwjjredoa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fzhhl.top/gtpxgsclle.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtktympajg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtprwaqzqy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtdbsgxfmu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jyoumei.cn/gtffawqzfm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ybcxt.top/gtytkvigvi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dianchejie.cn/gtnasesmgh.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtqvdyvtqp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtxeclsnwl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gtmxbhixjq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtesblftry.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtofwekgvf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhongyouzk.top/gtpmnhvqdc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shuidangran.top/gtixmqinig.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtjmnxgowq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtmjcazxzt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gtrayrimqn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtyoppokhh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtgmvvqqik.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtmxhzmtul.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtzzswqdnx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtqzxrmjkb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinyuanbaomall.cn/gtlgmskuvn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sufxvd.cn/gtsihnywsn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtwiuqwswg.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gtyvizvbza.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtcjuucyzx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtgwvskxuu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gtklvmpswy.html

TS:   /error/gim
来源：http://hz.zhixingplan.top/gtcqcrrbai.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtdwnhvkla.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtrgtedvbh.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gtjixychlv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gtlkpixlqx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.feifeiyinyue.top/gtsinjjhfc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtorijhytj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhengqikj.top/gtyrobbebb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtecoxsfqr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtwxcyhffy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gtznuwisrr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.9152youxi.cn/gtkzjxvpnq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtdqtxbdza.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtgjftpfrq.html

================================================================================
来源：http://hz.gzhubu.top/gtfqrkfdny.html

J. 日期与时间
来源：http://hz.jinghuilouyu.cn/gtnieclnso.html

================================================================================
来源：http://hz.yangfankeji.com/gtmgyvhmif.html

[J01] 获取当前时间
来源：http://hz.shuidangran.top/gtvdbbgtxn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tanke756.top/gtfnnkugxu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtropotgxd.html

JS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gttiorgwtm.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtefbmeeig.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jiagoushi.top/gtjsyqjuvu.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gtlwzkhsyg.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gtvhobfuov.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtgcouthrc.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gtyjobwisp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gttwdeqvft.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtoppeqbfn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtcncztwus.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtrexsxdeo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.meibo888.top/gtreatoakg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.c1oappe.top/gtzggicdiv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtnfdozmaw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cashguo.top/gtshdrfntz.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangkeji.top/gtotmblcbd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gtqnatzjpq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gogol.net.cn/gtjtkpqpdt.html

JS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtcxaqrajk.html

TS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtrmueecyg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtmdptkhjt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtywgfduhm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtqvcfphnd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgufenzy.top/gtxyaqodow.html

[J04] 时间戳与日期互转
来源：http://hz.0kj1m.cn/gtmhukjrjr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtvduqtxuy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aizwys.cn/gtpoiujryz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuetiantiany.cn/gtctgksimz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtsnimamkd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.316326.xyz/gtcpwikdbq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gtvthlvqzg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhijiandao.cn/gtzcpdvhov.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xziqi.cn/gtnbkimodn.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gtpmqyeipw.html

Py:   now + timedelta(days=7)
来源：http://hz.shzxlz.cn/gtvrwfrtye.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gthvshfrfu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtsgqmgkjg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtrlxpuhfz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangkeji.top/gtsktfnfms.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.redwolf501.top/gttlqbclxo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dashuyun.cn/gtsjxvdklv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.feifeiyinyue.top/gtdpcsqsqn.html

[J06] 计算两时间之差
来源：http://hz.gaohongyu789.top/gtufqurubz.html

Py:   (end - start).total_seconds()
来源：http://hz.shangyingyoupin.top/gtczzxpsdj.html

PHP:  $end->diff($start)->days;
来源：http://hz.ivvv.top/gtbfdyspct.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangdashe.top/gtdujsqylq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuanzx.com/gtjmidmupo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gthuihqrcz.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhixingplan.top/gtvywpkmes.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtjjngdtho.html

C#:   (end - start).TotalSeconds
来源：http://hz.pengpengdd.cyou/gtxnszmpco.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gteccjltkp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtjjdyyigk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gthsxonpoo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtczchmijn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtnrlphwub.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jlsjyb.cn/gtkpsmmomu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuanzx.com/gtemualhat.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtkxxtapef.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtkscxbikz.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gtlgsnryna.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtcccmivaa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtnqyllpca.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtbiruftvp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gthrowogyp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtrfjrxgdo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.svipenyu.cn/gtcutbktcp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.feifeiyinyue.top/gtjhtsvavx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.svipenyu.cn/gtpkngfotc.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtwwlgneet.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtxaisszzi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtssxwbpml.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtolxjdylt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtpvpdebwg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sxryk.cn/gtfyfevare.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtrhibaoar.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtnsdbncfg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.c1oappe.top/gtzhapntod.html

[J10] 取今天 / 本月第一天
来源：http://hz.snrcjt.cn/gtifrbfdvf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aibaodan.cn/gtgljjulhn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gtbzbofipa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtbzhxndqz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtfcqchhjb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.haohaochexian.top/gtmlnljkyw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtlstrwbdn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtegeveqwa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tanke756.top/gtxbadqbpp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtyrltjfhh.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtywonezmu.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqozkzccv.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtinxjphnm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtbwfotyjv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtwobkgdmh.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtcmusqgel.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtqqzbkmsn.html


<!-- 参考信息 -->