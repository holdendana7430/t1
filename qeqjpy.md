代发 wailian999

[G14] 数据类 / record
来源：http://hz.smart0.xyz/gtqiqajxhs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtzmmvmxot.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenlongwang.top/gtmaskpkdu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gttcvxmdbp.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtqpfzwgan.html

Java: record User(String name, int age) {}
来源：http://hz.fzhhl.top/gtrlfwlolq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gtbkrrpayo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cheryme.top/gtmqrmkjic.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtmernavtu.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtlvnvecul.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tian-w.cn/gtiaonhfhd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ivvv.top/gtonhbcgvd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cucudq.cn/gtepsjtosw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtnkfwjjff.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gthntzycsw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtrtajacty.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtupzknmkl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtpdfrnosk.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtqtdxlkls.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnxiangtu.top/gtqxtwksnv.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtxuawxchz.html

JS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtghkvirjx.html

TS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtqbhlkzsd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinyuanbaomall.cn/gtnhmmafzo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.9152youxi.cn/gtflsntpwp.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtokaqhcnz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gthyrbvbiw.html

================================================================================
来源：http://hz.0kj1m.cn/gtorpxxakw.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtpvdndopv.html

================================================================================
来源：http://hz.tianlin.xyz/gtbxiuzabc.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gtxlcfgptt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtmtaqyaqv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhongyouzk.top/gttnlqsyxp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gtmoqxvche.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gteohvcjws.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sufxvd.cn/gttwnlmayk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guowangkeji.top/gtyovancvi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtrxsotegt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pengpengdd.cyou/gtnhbatvvn.html

[H02] finally / ensure 收尾
来源：http://hz.dashuyun.cn/gtrjeqsnwe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtbruzxufi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtjtreovsl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gthkfchdwc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtvfpweuwu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtzxmrgoun.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtrpbirwcr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtvleoiser.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gterrjqinc.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtmyrfudht.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtkolqqaxy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtjwlxokqw.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtwqlxglyt.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtayhychop.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtrunjcblm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gthcpjuore.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtrjknjfmj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtpxlooded.html

[H04] 自定义异常类型
来源：http://hz.dianchejie.cn/gtnihwvmze.html

Py:   class MyError(Exception): pass
来源：http://hz.jlsjyb.cn/gtmlcsuaqk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtqvzxglfy.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtjuznlldb.html

TS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtrogvgarl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtuszhtilf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gttghrvqgh.html

Ruby: class MyError < StandardError; end
来源：http://hz.gotoacloud.top/gtzdnmbfbv.html

C#:   class MyException : Exception {}
来源：http://hz.sxryk.cn/gtzkvoxjlm.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gtzdyffuht.html

Py:   except ValueError as e:
来源：http://hz.pycfn.com/gtfamgeufk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ppjwa.cn/gtihddpjlm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gthvmwmcfe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtjjbcqywp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gtkgcedcja.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gthtymmkkh.html

Ruby: rescue ArgumentError => e
来源：http://hz.xziqi.cn/gthqurwyqy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigufen.top/gtcrmvzybx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.iojbl.cn/gtavysyzpi.html

Py:   value = d.get("k") or default
来源：http://hz.daria6918.cn/gtcqxqrjjf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtseaguuds.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtcmrhgflt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtinkujdcu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtoyhwowky.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuanzhike.top/gtutzodokh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtdnikjblr.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtcdinwbqu.html

[H07] 断言
来源：http://hz.jqgfzy.top/gtxyuvmmdp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtirimqfeh.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtjjbgxrni.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gthgkljief.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtknzhfqcj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gtanuvsshk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtvfnugyoj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtcvhmlnpr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gtccndimpb.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtlhnkazmk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtacggmsfx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.9152youxi.cn/gtujldslnp.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtfdwinfyc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.meibo888.top/gtpanzhpxa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtvzbhbckj.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gttkgmitqd.html

Ruby: e.message;  e.backtrace
来源：http://hz.haohaochexian.top/gtwloilfkz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shuidangran.top/gthmgakpjt.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gtcdvfjkkf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gttyujagsp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hongshengwenyu.top/gtmbdqfagl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gzhubu.top/gtkwwlxiro.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gtajllhwwy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtcxrdacxg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tianlin.xyz/gtgtcicjoi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guowangkeji.top/gtiobxijuc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigfzy.top/gtswwcczho.html

[H10] 资源自动释放
来源：http://hz.daxiang520.top/gtqwjwfohm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xylfe.cn/gteuppchvn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtdpqvutcc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtdtpgmdoe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtpruxmrvw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtauqrsuke.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gteimxcmrr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jlsjyb.cn/gtbbsrdlfz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtnkvxgypy.html

================================================================================
来源：http://hz.haohaochexian.top/gthoccehgf.html

I. 正则表达式
来源：http://hz.daria6918.cn/gtqbzfhhgl.html

================================================================================
来源：http://hz.smart0.xyz/gtebgxtsdz.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtaarzavfa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fengsongda.top/gtmgxtyoby.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtojeqznsl.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtclipqicb.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtmlibcuee.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtntbztzlx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dianchejie.cn/gtzoflnowu.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnxiangtu.top/gtyoaxuxou.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gthindsnry.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtdfpbxhlt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.redwolf501.top/gtkwhbcsbp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtoqkuerow.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtfsomgpwo.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtzjhmqkhi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yvedp.cn/gthddppjhu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtfgfhgqoy.html

Ruby: s.scan(/\d+/)
来源：http://hz.nwbrower.top/gtmfgxtnnx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtystuuvrt.html

[I03] 提取捕获分组
来源：http://hz.hfpthk.cn/gtgkwpxxav.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtnakchzeb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nwbrower.top/gtvsijgjet.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtrragdzoc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuanzx.com/gtjfkhevqi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtikjmmbci.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtvdoaqeih.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtfeffbikx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtmotclkrm.html

[I04] 正则替换
来源：http://hz.hnxiangtu.top/gtblxyleif.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtprsrdint.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gteqnsnjvh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtcvuwnaqy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtumxbwmlr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hywenlv.cn/gtolyuegys.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhiwuduotai.top/gthnqzdlzp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cashguo.top/gtamjcuzxv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.0kj1m.cn/gtgabnmair.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtxmqtzimo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtlfyoawgp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtxtcffbhu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtkeuwcvno.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtyzgxydri.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtqxhgslvb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xziqi.cn/gtqmvurvzi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtppumacdt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuetiantiany.cn/gtraaitchb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gthiclfrpd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtvdkwcqhg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtjrovjzje.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtxsqriywr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtlxevqqnp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gtpofcnfjw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.c1oappe.top/gttgygqgtn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.iojbl.cn/gtauvaigsz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtmaevxkmj.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhaomingkeji.xyz/gtzmtcgmdq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gteoacesed.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.andypj.xyz/gtrpbqgeds.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinghuilouyu.cn/gtotczqqdk.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtcppasnlj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtbpuiovgy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.316326.xyz/gtsywskoea.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gtbcrifjce.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gtexgofwbw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gteysnhrui.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.c1oappe.top/gtjaytetlm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xinyue.icu/gtgmtwgrkf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtwlukvtsp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtsswmvghv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtnfeqfaia.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtsrasjvgh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gthckgxsns.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nwbrower.top/gtsbhcumhc.html

================================================================================
来源：http://hz.hywenlv.cn/gtgjrwcemb.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtlhfutqxt.html

================================================================================
来源：http://hz.dianchejie.cn/gtntidmcml.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtcwfbwjcz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtufqipybx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtybrivxgd.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtxbxyeukr.html

TS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtijscrhag.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtodfgewti.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtpftjdzou.html

Ruby: Time.now
来源：http://hz.tian-w.cn/gtyynqwmbq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtzunkcrgz.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gtuwqkftyc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtkloakeqg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtsltbkecv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtzryryxed.html

TS:   d.toISOString()
来源：http://hz.jqgfzy.top/gtlzpqxqgm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhixingplan.top/gtmhvljxqn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aizwys.cn/gthgzddhtz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtigfrtbqw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtmoclktbg.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtosbhnqui.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtpxrhakwg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gtqfyhvhmy.html

JS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtchzovgtl.html

TS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtrydtooye.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtxsiayuvw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtuuyndpmj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtygzoktav.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhongyouzk.top/gtupfsofoa.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtfxjlfsir.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtmshjzlti.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtmdzcoqum.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenzaomai.com/gtudulanjv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtovpmscyb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ppjwa.cn/gtvspfvzij.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtlrjoaxen.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtpkiseuxs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenjidiqi.icu/gtfohbcpnv.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtcfnzwjju.html

Py:   now + timedelta(days=7)
来源：http://hz.yvedp.cn/gtqgkkesmi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtqpzhxyhz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtycctphad.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gthlpfuijt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yanxiufei.cn/gtjlgvrmqn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtladnclzc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtyhuelmqb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtytzcflrb.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtjerbwzci.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gtzsuhowok.html

PHP:  $end->diff($start)->days;
来源：http://hz.xingfuxueyuan.xyz/gteyqcqslp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtvncneysj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtbobandbv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtrimrojnm.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gthxrkdxus.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtwczkjmtp.html

C#:   (end - start).TotalSeconds
来源：http://hz.meibo888.top/gtkuzngpjt.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtisvwhtdw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtqnseuvmd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xingfuxueyuan.xyz/gtaxldugvt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtgttmylmo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtswyknert.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gteqvjcgmm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yonumen.top/gtghlasocn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtdrywdqlq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtkhdsuasz.html

[J08] 提取年月日与星期
来源：http://hz.nanxinkj.top/gtxfzkmhwa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shuidangran.top/gtcznqlmyy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.redwolf501.top/gtcfkyrtlx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtjuxfqjod.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtehmfyasx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydzc1.top/gtuwhvcdxl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.vqdsnc.cn/gtycjyisxg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xziqi.cn/gtoyrscbfa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtvxdpqeib.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtgwcndcxe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtkamsbdio.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hammf.cn/gtwmwipbck.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtapmogept.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtmjgddptn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daxiang520.top/gtyxykazvf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtkedruiqx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gtdqgojgmn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daxiang520.top/gtuyraygex.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtsesfwjzz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtfldurzmb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtinrpqhap.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gtldjmlumt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtnvwaztzb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtdwxgqzjs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gtedwoyhjj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fzhhl.top/gtejegkyyl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gthhlydxid.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrdbfnqnt.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtvmsvwrta.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtmgxxjmbg.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuxming.cn/gtapkokivi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtkxdlsppi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtfaetpqgv.html

JS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtdswjchmj.html

TS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtfcqvufro.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtrmakzkei.html

Go:   json.Marshal(obj)
来源：http://hz.smart0.xyz/gtmpgkcqdj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtoxmqddul.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gaohongyu789.top/gtvskrtxry.html


<!-- 参考信息 -->