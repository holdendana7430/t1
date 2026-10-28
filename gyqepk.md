代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.hysaishi.cn/gtmahwoqcg.html

Java: record User(String name, int age) {}
来源：http://hz.haohaochexian.top/gtnnhxoqua.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gtlcduvguv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gtbpwklmrs.html

C#:   record User(string Name, int Age);
来源：http://hz.pycfn.com/gtbarkatej.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtjfylcqnp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtgmctpxei.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gteqzzgcdr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtrnkamvwu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtcuqgkvpd.html

Java: enum Color { RED, GREEN }
来源：http://hz.gogol.net.cn/gtizzeyodz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.iojbl.cn/gtnskwnvjz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtotztzwvn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtmugvttrf.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigufen.top/gtkiotpldt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenzaomai.com/gtpqedyjvb.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gtxlbxrdmb.html

JS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtjksrhvep.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtanrgxxog.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtqsiuvfca.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtrvtjilis.html

Ruby: obj.instance_variables
来源：http://hz.yanxiufei.cn/gtcxkgpvcb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtpjkptpnc.html

================================================================================
来源：http://hz.tanke756.top/gthxshdxee.html

H. 异常与错误处理
来源：http://hz.gogol.net.cn/gtrxqyawfi.html

================================================================================
来源：http://hz.hysaishi.cn/gtdqebczce.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gtjawjkfyx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnxiangtu.top/gtfsugepqc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhixingplan.top/gtuiqicmke.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtgqkdxphc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtipelaiad.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fzhhl.top/gttdghdmob.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ywan-chungtsiang.top/gttufmkgfh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gtyzfrxeis.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydzc1.top/gtycohjjaz.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gtrehrkory.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hywenlv.cn/gtjnvrqlrt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gttyugzmag.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtoyxfojpi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtbjjaxylp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtmmlvwgfi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtdkydpuvk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ywan-chungtsiang.top/gtprgizcac.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pengpengdd.cyou/gtbuoknclj.html

[H03] 主动抛出异常
来源：http://hz.hysaishi.cn/gtpbaeyzdy.html

Py:   raise ValueError("错误信息")
来源：http://hz.fzhhl.top/gtdtpkkrrt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtaiwiqyqp.html

JS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtwijwhsls.html

TS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtdldweggo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtmrlffzjp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtibqruxts.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhaomingkeji.xyz/gtcwybmrov.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gttxbmylde.html

[H04] 自定义异常类型
来源：http://hz.havefunace.top/gtikknyvfl.html

Py:   class MyError(Exception): pass
来源：http://hz.pengpengdd.cyou/gtpcrqzzmv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtzayeuhkq.html

JS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtzzebfpuy.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtbcqpkytg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtxumdbyij.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.vqdsnc.cn/gtiocufvjk.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtlowyjftv.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtwgqhszfo.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtzqvxnvoi.html

Py:   except ValueError as e:
来源：http://hz.sufxvd.cn/gtpzspqogx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtwefzoadg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtcjrvzhwa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtbkscsazr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yvedp.cn/gtwmqgogey.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gtefrfdfuz.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtdshhqret.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtguahmbms.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shangyingyoupin.top/gtwtkhoczb.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtnbyxhlix.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtgeelitlj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtpkxeycdr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtihmtvzuw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtwlaiqvzl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtpljbfpyf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtwitbpbks.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhoulong.xyz/gtsyfqdojj.html

[H07] 断言
来源：http://hz.fengsongda.top/gtxaypontj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gtxixplfng.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtedrtasul.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtoseokgnn.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtaxtnamff.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gtgzhitwfh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtffrrydot.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtvjmkktae.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtystoyssv.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtledrzumo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtvccvgnai.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gtavwwqndi.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtaenbiife.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gteborktdb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtupudstec.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtmavdvldi.html

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gtjcwbmebt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtptukyfaz.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtwfzdeqpo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aibaodan.cn/gtooycchvr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gtzjuuqmev.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gtiscxdook.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnxiangtu.top/gtydxggrre.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnxiangtu.top/gtoexfvygx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gzhubu.top/gtaqnsoibo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuanzx.com/gtrqzcprvt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuanzx.com/gtiaxfczch.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtjnousqsg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtmhqmxlyh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtmfchqtaz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtkhjtgyfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtkknukdsg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtsfllhlsu.html

Go:   defer f.Close()
来源：http://hz.ydjk.org.cn/gtrizqphvs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtlehajllt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gtysamqetc.html

================================================================================
来源：http://hz.zhongyouzk.top/gtefoytifp.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtpqcmbelu.html

================================================================================
来源：http://hz.jianghu66.top/gtrxnwkkda.html

[I01] 判断是否匹配
来源：http://hz.ybcxt.top/gtiupftdft.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhengqikj.top/gtdsbidvgh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dashuyun.cn/gtwezgmpzk.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtnozryepk.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtnlroowua.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj202588.top/gtheavakyx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtgvegvshl.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtgkbwvpwx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtnesqybhu.html

[I02] 提取所有匹配
来源：http://hz.pengpengdd.cyou/gtwqmciwqg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pycfn.com/gthlsnwttu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dashuyun.cn/gtczmqmoyg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtpwwunlsj.html

TS:   s.match(/\d+/g)
来源：http://hz.birdmap.top/gteqpqlcsn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.svipenyu.cn/gtxssmjxkt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgfzy.top/gtaiyidwcf.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gthbfbhxrv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dianchejie.cn/gtahcpuiji.html

[I03] 提取捕获分组
来源：http://hz.haohaochexian.top/gtalnwkzbn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jyoumei.cn/gtagcnlsfy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtlrceiatm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.svipenyu.cn/gtszfdwnui.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zycfv.cn/gtlxkxnttn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtaqauxzzi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gttckjmjov.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtimryhgvj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtmqaayklw.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtngvclfwf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gthiyjbygo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gtfeyzcnhl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtehbccciv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtxfmzogjy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtklszufva.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yongpay.top/gttpklhfia.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gtihklokmk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtcedodxew.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gtvgmungsq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gtycvwhbjp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shzxlz.cn/gtoegzwqwe.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtytjviocv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gttwgswpqv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xylfe.cn/gtqcownjgs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtvmoxdkbd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtjriaavqj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtsgjaestr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.mhx1999.top/gthgktdcne.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.quarkkingdee.top/gtilmgmlei.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtvysknuil.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gthdltasmc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtvjumqplt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtdjzyodbt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtbeywaxzb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dianchejie.cn/gttztsbjnp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtmhobtmvr.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtmgchiscu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtlaysciht.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtzgpjnqxg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.snrcjt.cn/gtpqxdhwxp.html

TS:   /error/gim
来源：http://hz.zhaomingkeji.xyz/gtyjacjvuw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fzhhl.top/gtbrthzszb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hammf.cn/gtmeruanua.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtuyoqgtqn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnxiangtu.top/gtpkjnktyh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuxming.cn/gtveinsyqd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtvgouuwkf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shuidangran.top/gtvclsdhyy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtzawdtsmy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtkkutycuv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.birdmap.top/gtimhpomml.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenzaomai.com/gtufnhinrv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gtoxhzpcgm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj202588.top/gtyzspsajh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gturvypzld.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtfkpzximw.html

================================================================================
来源：http://hz.mhx1999.top/gtemvjalxw.html

[J01] 获取当前时间
来源：http://hz.jinqigufen.top/gtqdcgotez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhongyouzk.top/gtguvogsun.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtqnpanbtr.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtwayoitzl.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtjcfnnoyj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pengpengdd.cyou/gtmgqjhxhn.html

Go:   time.Now()
来源：http://hz.vqdsnc.cn/gtdxjttxpb.html

Ruby: Time.now
来源：http://hz.zhengqikj.top/gtunwnfhjb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinyuanbaomall.cn/gtfyfwduge.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gthhbbsyqg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtgpqzyaws.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtradvfsgn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guannengcc.top/gtywpwprlh.html

TS:   d.toISOString()
来源：http://hz.yvedp.cn/gtoihbnhls.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ywan-chungtsiang.top/gterahzbwr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtmjbnjqyb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtzlmqngwb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sysykeji.top/gtaubxaqzd.html

[J03] 字符串解析为日期
来源：http://hz.jyoumei.cn/gtxnplmdtx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gthvrqqoga.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtmvzeihni.html

JS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtwxkwhdtf.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtjlosmhlh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtvlcpioqw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtppgsbnfs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtcjerlsgo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gtdhbgfhbz.html

[J04] 时间戳与日期互转
来源：http://hz.ivvv.top/gtlilhefdr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtdpzdsixy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yongpay.top/gtjjsuizwb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtdyenynba.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtphpzjxio.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.c1oappe.top/gtaiormdvr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zycfv.cn/gtozgmblpi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtvqquazgc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhixingplan.top/gtgdlcecyj.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnqzz.top/gtcqphdssp.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtubxwpuzl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuanzx.com/gtqfvnjfiy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtvupkvqfx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtqaaenclw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtxvxkubnl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigufen.top/gtnxbfxxrt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtjqrdkfly.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gtlqoyanii.html

[J06] 计算两时间之差
来源：http://hz.aizwys.cn/gtrtcgqojb.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gtvcureoom.html

PHP:  $end->diff($start)->days;
来源：http://hz.iojbl.cn/gttllngxeb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtwgdeyrlx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nwbrower.top/gtjrixzktb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtommbsril.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtadwxedtc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtrivphwww.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtgolqzoqs.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtfzamlitp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtneejhbsi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtpmmzcony.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtowrioote.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtqbwzzzbw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuetiantiany.cn/gtqzvzlzyw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigfzy.top/gtroasurzn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtxcdoiwpe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtrzpayxaf.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtrojwzzfu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guowangkeji.top/gtfsstpgoq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtiiufjihy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtydlotbjj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gtoorvgmks.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gtrwlyofau.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtlfajcbpw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gthctvfsmo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtrpbudqti.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gtqxfmixsa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtvmtndolw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtrwykpoap.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtghewnudc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtyaicrcza.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gtgumwaiej.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtwdurnhxt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hfpthk.cn/gtfsjqlfqw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cucudq.cn/gtttbzmqxg.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtptbuqfhw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jianghu66.top/gtvzvvpews.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gthjzlsbkn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fzhhl.top/gtchlceaew.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtaehyxnsr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtagmxxsii.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gttuirnnsc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtvzsouwpw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hysaishi.cn/gtdwmlpxqf.html

================================================================================
来源：http://hz.xylfe.cn/gtxyguxcad.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtkrxcxhsi.html

================================================================================
来源：http://hz.gzhubu.top/gtziucxmmo.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigufen.top/gttgepypgd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtvtmjknbc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtzipvdcct.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtuogpgnga.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtuzcmnkpo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtoexbaivb.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtqbdqlkuq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtflepifbc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shangyingyoupin.top/gtrjzinmla.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gttvjopbzu.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtklqbpdvo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtliostlmv.html

JS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtrrdmmmef.html


<!-- 参考信息 -->