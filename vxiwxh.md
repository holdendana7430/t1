代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtcjbrtipf.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtfbumhnww.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gtejwpichy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenzaomai.com/gtxrkkjzzj.html

C#:   record User(string Name, int Age);
来源：http://hz.redwolf501.top/gtdkbttckc.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gturgzpzdp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtmydyzayk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtlyvquqev.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtvymxlltb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtngfolakv.html

Java: enum Color { RED, GREEN }
来源：http://hz.yueranfly.top/gtcazmpdfn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtsgpiuivo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zdqjudy.top/gtrdkbctqx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtpxgropne.html

[G16] 对象转数组 / 字典
来源：http://hz.chenlongwang.top/gtpcxtkbxh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gthgvlghtd.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258.top/gtzyotdegn.html

JS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtddojweac.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtajgxaqys.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhijiandao.cn/gttkjelegp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtuymwbojq.html

Ruby: obj.instance_variables
来源：http://hz.jinqigufen.top/gtlwtlmjnq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gttvcsgqcv.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmknsahpo.html

H. 异常与错误处理
来源：http://hz.gzhubu.top/gtwpwpxgsg.html

================================================================================
来源：http://hz.yueranfly.top/gtlljtyrze.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtozzufycm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtzjpbhdvn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtdhqfsdoe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtwnnlucrx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtmqreyumt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.9152youxi.cn/gtbzypglmj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.snrcjt.cn/gtpqtdmvtv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gtfgudthvm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gtmcspiurw.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtijhsyqzx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.mhx1999.top/gtqqlheast.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtzytiolre.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtuwxtyuty.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtdczwstim.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtvoqwkygu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtslpjxonx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yvedp.cn/gtanzzzfpo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtsxrgvwoe.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtjvtwtnaw.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtjeivzues.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtauznamvu.html

JS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtzewbvbkw.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtskselzfv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtwrplfnzo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtlfxznzbm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtpkhdepsh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtdzrfiwya.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtrbargvmo.html

Py:   class MyError(Exception): pass
来源：http://hz.feifeiyinyue.top/gtpdktksxn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtlvirwwyq.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtxjphopbd.html

TS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtmfwonnjf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtfjvwkjvd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtcbcyhlqr.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhongyouzk.top/gtcaocpkuk.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtxanbopjm.html

[H05] 捕获特定类型
来源：http://hz.yongpay.top/gtlwbkvysv.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gtpqjkiqyc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sysykeji.top/gtytpsrcof.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtwgtzyotd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtuibdgjqq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xingfuxueyuan.xyz/gtjtvivayc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtkfxzrxkj.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhoulong.xyz/gtdpgmorkw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenjidiqi.icu/gtpyohcsnl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtpjjdslty.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtvlpsebcl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gthjwlnyit.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtijsxaczf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtxeykosif.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.9152youxi.cn/gtxwhlzkyx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gterehhojf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtaopuihgi.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhixingplan.top/gtwpnjpmqv.html

[H07] 断言
来源：http://hz.52xcode.cn/gthjduxsde.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gthhfpyoff.html

PHP:  assert($x > 0);
来源：http://hz.zhijiandao.cn/gtlcluqgfj.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gthhywvyaa.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtvwfohglc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtlxkzyquk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtcxgvtrhx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.svipenyu.cn/gtduqjawdc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hysaishi.cn/gttacgalag.html

[H08] 获取错误信息与堆栈
来源：http://hz.jiagoushi.top/gtpttubixi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtcrvlxjlp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtwmelauea.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtnripdtbj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtyzsihjdd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtnbfxiymi.html

Go:   err.Error()
来源：http://hz.ybcxt.top/gtkcbzxady.html

Ruby: e.message;  e.backtrace
来源：http://hz.cqqwz.cn/gtoumdrzzw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinyuanbaomall.cn/gthbwuugis.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtbvxpmnwe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tanke756.top/gttsvgebgx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gttnaufdjt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtbzcjeedf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gtdpcchzge.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangkeji.top/gtfxsmjpbh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtrlkfjenj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shuidangran.top/gtctsltlmi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtzqxtcmrv.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtivzonwuo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sxryk.cn/gtbgbzwmqj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aibaodan.cn/gtazxtkkrm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtvndlgqgy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtdrnrcrzq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gtmbeegcey.html

Go:   defer f.Close()
来源：http://hz.jlsjyb.cn/gtiqospyyl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuxming.cn/gtfqwonoqs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtvdxveozf.html

================================================================================
来源：http://hz.fengsongda.top/gtbygynnik.html

I. 正则表达式
来源：http://hz.gotoacloud.top/gtpzblsyky.html

================================================================================
来源：http://hz.shzxlz.cn/gtobdbojzz.html

[I01] 判断是否匹配
来源：http://hz.jinqigufen.top/gtlxsojyqs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gteqwjqwqc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtddsjmbxu.html

JS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtdafacrnv.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtrsyudyme.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtsybjbfwe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtoeebnker.html

Ruby: s.match?(/\d+/)
来源：http://hz.fzhhl.top/gtrvgvblft.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.mhx1999.top/gtrgpmjgvt.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtegtdgdph.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cdnleiting.top/gtpwhezkmb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gttcbsgusm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.smart0.xyz/gtwawbehuz.html

TS:   s.match(/\d+/g)
来源：http://hz.quarkkingdee.top/gtetwdkmat.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gttzivlunu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gthwjsbwxs.html

Ruby: s.scan(/\d+/)
来源：http://hz.gzhubu.top/gtebvrzaku.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtvrbqipwv.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtpobifpru.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.9152youxi.cn/gtwqdepmyz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtiiryphel.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtpyxlxdwm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtqnvppszk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgfzy.top/gthjkiccyv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtoepebdgf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtzabytrcw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtlkmowdhx.html

[I04] 正则替换
来源：http://hz.zhixingplan.top/gtidvwsuqh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gtkgnfcdvj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtzcncegjc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtjayzygsa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtigybauen.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnxiangtu.top/gtoxcmmrca.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xinyue.icu/gtrerleioj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gtucxmlyxd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gthoslqnam.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangkeji.top/gtosjucedl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtdlyurobm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtrmftikcu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtwqjoxtvb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gttudtfcdi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtacveyjws.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xziqi.cn/gtripoomad.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtuhfijjcx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ybcxt.top/gtkcepruce.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigufen.top/gtktscmprb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtozgaejjx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gtdvdhdrmv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtckrnwfei.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtizjbdjlj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shangyingyoupin.top/gtgcqnqlfh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jlsjyb.cn/gtuebpmiur.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hysaishi.cn/gtqmtwkjzt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtknzokzdz.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtnhudaexk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtrusfrdkj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hywenlv.cn/gtgpwccbou.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtzbplpjxk.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtzyvgkflz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtklmigocm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtfhdriwpo.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtkixxmhov.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtgaojhqji.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.52xcode.cn/gtvfmswrfd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydjk.org.cn/gthbzghwhp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.mhx1999.top/gtxninqwgc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtdhqemfum.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtetnlgnbt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtojvgqnoh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuanzx.com/gtntfunvpb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtkoiivvax.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtminmbukn.html

================================================================================
来源：http://hz.sxryk.cn/gtzyvttxka.html

J. 日期与时间
来源：http://hz.kuanghao11.cn/gtusavoiad.html

================================================================================
来源：http://hz.zhengqikj.top/gthfrbjazs.html

[J01] 获取当前时间
来源：http://hz.sysykeji.top/gtqkkzcocz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtndhwyjpb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtsvhtsnls.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtqrsiwfyt.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtaipnxzds.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.meibo888.top/gtbjkncwwo.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtgdctylcl.html

Ruby: Time.now
来源：http://hz.ydzc1.top/gthfqkryxo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtnqdfiaah.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gtbskracfg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gthvvrbpfv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtjhdpsdzl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtcdidvjpa.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtmcbdclac.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daxiang520.top/gtepjtltvb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gtvfimvymk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtkvajujav.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cashguo.top/gtxlzbrdhe.html

[J03] 字符串解析为日期
来源：http://hz.ppjwa.cn/gtaqzufamc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtjgzcezyi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aizwys.cn/gtxcitzbez.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtajuwcgrq.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtoggifrcj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtsuwdgcoi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fzhhl.top/gtjdwbtkaf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtdylktzoq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fzhhl.top/gtzmcaenun.html

[J04] 时间戳与日期互转
来源：http://hz.jinghuilouyu.cn/gtbibkfhwg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtldkttbqi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtfyrqbonv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtgefmfsgm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtgctzmypp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxuanxn.top/gtmbupxzwd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cucudq.cn/gtqlfznaue.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jyoumei.cn/gtydajxiwm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtyaadusmk.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgfzy.top/gtsjujoqzi.html

Py:   now + timedelta(days=7)
来源：http://hz.c1oappe.top/gtutcmwhtc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtionexdtp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtbecnfrpw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtdmcpkmle.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.snrcjt.cn/gtmjkrgkag.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtroyzehpi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtgdjuqtjm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yonumen.top/gtpdpdcdty.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtnetphmms.html

Py:   (end - start).total_seconds()
来源：http://hz.yongpay.top/gtwbmuuapm.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtcmymcvok.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gtfeywrgkj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.bjfxy.top/gtbdixavsc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtgcpfopek.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtfovucirw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuanzhike.top/gtpszbdfnd.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinyuanbaomall.cn/gtafgofqkz.html

[J07] 比较两个日期
来源：http://hz.ywan-chungtsiang.top/gtbuujlsbp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtzmycjwft.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sysykeji.top/gtzlffdfbw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtslbytrpf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtgxewwjec.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gttzdyzjew.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yanxiufei.cn/gtkaleiouu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtdedczdqm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtektimutq.html

[J08] 提取年月日与星期
来源：http://hz.chenzaomai.com/gtjmhssjdc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtblgmxxdi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.iojbl.cn/gtfmpqbtfo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtnjyqaqve.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aibaodan.cn/gttdyudotj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhijiandao.cn/gtkomwjndd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtxkyxsgnd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhongyouzk.top/gtaqmephox.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gtmfihdgzs.html

[J09] 时区处理
来源：http://hz.yvedp.cn/gttlrcvcmp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.redwolf501.top/gtarchwgmv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nwbrower.top/gtryeyybof.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtxsbiugar.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtcvruonjs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gtgafxarvs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gteupfkqxp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtcaxysfyq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtprcvyied.html

[J10] 取今天 / 本月第一天
来源：http://hz.redwolf501.top/gtqpzzfqgd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtjewasndu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtqvjedizi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtskxexeph.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtjzkrzljd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtimqhrsrr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.haohaochexian.top/gtixtrclcv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtwtfwxzgm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtdllqabkc.html

================================================================================
来源：http://hz.gotoacloud.top/gtdbkhwwgz.html

K. JSON 与序列化
来源：http://hz.tianlin.xyz/gtzebarqdd.html

================================================================================
来源：http://hz.shzxlz.cn/gtmlczdgao.html

[K01] 对象转 JSON 字符串
来源：http://hz.jianghu66.top/gtivdhdkgd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtoqloddvj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtluymuzgd.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtkzeuwbuh.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtwtrrxkdn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtdyjxjzya.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtbdtzfhqx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gtlahxynie.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtwcdwlkbo.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtwchrfgfp.html

Py:   json.loads(s)
来源：http://hz.quarkkingdee.top/gtzarhuilg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtjgsrbgan.html

JS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtnnrlyptj.html


<!-- 参考信息 -->