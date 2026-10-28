代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.jyoumei.cn/gtmavmesdb.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtpipvlwsx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shuidangran.top/gtnvhfxmso.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtshwlzfmy.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtrylzusnc.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtjomaxyow.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtdurdcqiw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtckjqmpza.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tanke756.top/gtqulticol.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtrgwohbkk.html

Java: enum Color { RED, GREEN }
来源：http://hz.yvedp.cn/gtthmoobbu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtihnmiwtd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtjuifyiwg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtiyojqwsi.html

[G16] 对象转数组 / 字典
来源：http://hz.chenjidiqi.icu/gtidquukbe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.kuanghao11.cn/gtccfcglmd.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtqnifkfem.html

JS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtoietzxdj.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtewmodgbj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtvepsdrju.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yangfankeji.com/gthsqdcilk.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gtxoenehlb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtvxccjpli.html

================================================================================
来源：http://hz.shzxlz.cn/gtuywzfuqd.html

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtctmhvoxc.html

================================================================================
来源：http://hz.9152youxi.cn/gtntxipfwd.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gtppigkndi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtmgjumsvm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtyuilrwcq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtrirnmxvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pycfn.com/gtgwcsoebs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtxgmwbqgj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gtypydpwtm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.birdmap.top/gtgkdesrhp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtvoubyhhg.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtogdvdmht.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gtggcvgjsl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtbufyzdbh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtksbvytdb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtxtuhsbhh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtspcdwsen.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtzgsqckdo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtyrdkffpb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtakfitazg.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtmnkqbhlj.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtesgqqlxy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtdgsdwmga.html

JS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtxeoearog.html

TS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtxflmwebs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yongpay.top/gtwdgadogo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.redwolf501.top/gtouobbzlt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gthnersdwq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtdjihvgsa.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtnpcyvmnh.html

Py:   class MyError(Exception): pass
来源：http://hz.snrcjt.cn/gtkcmjyvrn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtbicscvfw.html

JS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtzmfcsyts.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtuacfdqig.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtldugutjr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtcrszcwly.html

Ruby: class MyError < StandardError; end
来源：http://hz.cqqwz.cn/gtoxljtguj.html

C#:   class MyException : Exception {}
来源：http://hz.vqdsnc.cn/gtetjfnkxp.html

[H05] 捕获特定类型
来源：http://hz.dianchejie.cn/gtoyupsrul.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtothiarqi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.316326.xyz/gtrjzxldha.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtzrgfpwyu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gthdpdtrlj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gtadunpekd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhengqikj.top/gthcsduijh.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtuwxmxwho.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gtroohcsjf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gtphnyipcz.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtfepsxmxl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ivvv.top/gtaoarsbsw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtvpgvioww.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtzhmqctos.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtsagfckbf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ybcxt.top/gttgtffwpn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtcuhmshlg.html

C#:   obj?.A?.B ?? default
来源：http://hz.daria6918.cn/gtlrpxckip.html

[H07] 断言
来源：http://hz.zhengqikj.top/gtvuwcnhcr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtjwezkbhm.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gtbpsuyxay.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtkzocmead.html

TS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtbajavrxr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gtcjuoycyb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.iojbl.cn/gtxvwvnmpy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtrdhmecsn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuanzhike.top/gtlijnxxmc.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtfufmbuvx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yueranfly.top/gtbsordsfw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xziqi.cn/gtxhmcxzej.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gtoaajphck.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tian-w.cn/gtnhajmrvm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gtpqaklvjw.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gttwqzptxc.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtzqscptyr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtwflbmefj.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtsxswbocb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtnkdwshfg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daria6918.cn/gtyrmlelln.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxuanxn.top/gtdfficuwt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yueranfly.top/gtcwtlhhnl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.birdmap.top/gtmgsdzihm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.svipenyu.cn/gteipcuxet.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xziqi.cn/gtnyxavpmh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtwobeiiii.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtpmgrvacu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.svipenyu.cn/gtkugaexrj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenzaomai.com/gtanffojhu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtzcktwebx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtgxmyekkc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtsdwgyvpt.html

Go:   defer f.Close()
来源：http://hz.jinqigufen.top/gtlppjdpgq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yangfankeji.com/gtgvfacubc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gthfdnodjp.html

================================================================================
来源：http://hz.jiagoushi.top/gtxlvibcod.html

I. 正则表达式
来源：http://hz.nwbrower.top/gtlpskapmn.html

================================================================================
来源：http://hz.yvedp.cn/gteptktrdu.html

[I01] 判断是否匹配
来源：http://hz.gaohongyu789.top/gtqtiluejx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gttwzwojvv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.c1oappe.top/gtximxfhyi.html

JS:   /\d+/.test(s)
来源：http://hz.yanxiufei.cn/gtfqnzoevd.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtbobvuzyh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangtech.top/gtetrqxxea.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangkeji.top/gtdxxffgfh.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtrurnjnmx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtywhhyjep.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtqliudhqe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gtnfeawpoz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtehwtjfck.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtibwxslat.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gtoxbcding.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtnbfazikr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtckzlavgl.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtqziyapwj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtqyfjrlxf.html

[I03] 提取捕获分组
来源：http://hz.jyoumei.cn/gtzknjtwfr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sweek.top/gtebuoqqqf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gtjknxwfqp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtckjzpmup.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtekvbpvvu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtqvydfupl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sweek.top/gtwatgahud.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gttrzzkisl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tianlin.xyz/gtezrqdhot.html

[I04] 正则替换
来源：http://hz.chenjidiqi.icu/gthnkwhdfh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.iojbl.cn/gttctxudii.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtfoilzodp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtsbsxmhiw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tanke756.top/gtjrsjufhh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtrlezlceo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuanzx.com/gtmjzayqau.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhengqikj.top/gtzyfgmyhg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtpehojzlv.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtksdhwmix.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sweek.top/gtuyhnftcs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtbkmlglxh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtqfzfxhrg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtbomwjjgx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtyxiedhqt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shuidangran.top/gtufvjwqgm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtuvyadzex.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtpuxpchdc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ybcxt.top/gtnhybnbxv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtdeobgmdd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtpxewuxmz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtzgnegoki.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtqiodebau.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtefokqvsy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gtlkdsuyit.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.smart0.xyz/gtgpkhzbns.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtinpcbqsv.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtafpenmrd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.52xcode.cn/gtxpzolegg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtzuhknzpm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtbgaawxmg.html

TS:   /error/gim
来源：http://hz.hysaishi.cn/gtmaphxhbz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtcbkimlsu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangkeji.top/gtqapcxhaa.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtynyaqpsw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.birdmap.top/gtlizfzqgp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnxiangtu.top/gtzrfsipat.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258888.top/gtjzfmugyi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtjfwosmkg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gteedgaaes.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtavpxmrmy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtmajuqhkk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtokshxbua.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yvedp.cn/gtzadlpjqv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtjijcyikl.html

================================================================================
来源：http://hz.ybcxt.top/gtdrpbqfhv.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtcczhmuul.html

================================================================================
来源：http://hz.snrcjt.cn/gtwihndlfp.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtlttvhygc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtitkkcjgd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtawudmdcx.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gthmovvkth.html

TS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtxiyjvdvx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sxryk.cn/gtnlqtemlp.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gtexljrvfz.html

Ruby: Time.now
来源：http://hz.birdmap.top/gtiypwbbmh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zycfv.cn/gtiyawvjlp.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtvtswvbbk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gthnvxorzr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtnnhiifhf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cucudq.cn/gtjvzacgbm.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtdvztfhwf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jiagoushi.top/gttehyygkw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtewwdfdma.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gtqqvdaczq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gthgbmcvdg.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtfhenpnoi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtrkwljtol.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtfcggregi.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtalisjtpi.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtzyisompw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtvgzyhyhw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.havefunace.top/gtcndqizor.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtrhzlmhpw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hammf.cn/gtrvaknzvg.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gttvoceeat.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtcokwvcqk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jiagoushi.top/gttklofpwm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtbwfueqmi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gthedzehra.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yueranfly.top/gtqukoykis.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtnbivkwfi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sysykeji.top/gteljpycze.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.havefunace.top/gtidmxmqud.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtifhozawk.html

Py:   now + timedelta(days=7)
来源：http://hz.shzxlz.cn/gtxgkzvkxy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pengpengdd.cyou/gtvtfipper.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtqdqseerw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gthuuxzrqf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtmjlyfqum.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtzdtoquju.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtatblkhli.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangkeji.top/gtllqqkddi.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangkeji.top/gtqrrzaefn.html

Py:   (end - start).total_seconds()
来源：http://hz.sweek.top/gtgdwntigz.html

PHP:  $end->diff($start)->days;
来源：http://hz.sysykeji.top/gtyqqtixbz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtsgrhqeje.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtkcalvwnj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gthuvwgnqg.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtmihbqaya.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtbbedetvk.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinyuanbaomall.cn/gtpsfgtbho.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtgjvmhzca.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtmnaonifi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtmeiejyzc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gtecltzwyi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtfpgfaswz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gthdpxvdai.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gtegazjzyk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtignsdumf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gttjkymdnj.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtqxapbtvk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cheryme.top/gtupusvriz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtgxuilkvm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yangfankeji.com/gtilwminrl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtoaahzhax.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tianlin.xyz/gtdhfffgdz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtbhhpatoj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtlzfspakt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258888.top/gtmjkulcls.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtzdivaiwl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daxiang520.top/gtgcfnizsn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtrhezbawd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtrwspozhd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtnsjjmhax.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtdcdtvsua.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuanzhike.top/gtftskahhx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gtwzyiokly.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hongshengwenyu.top/gtpejyzrxp.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydjk.org.cn/gtvrvpgdsx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtcdeuodbt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtxdaizjfr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yanxiufei.cn/gtehsbnhim.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xinyue.icu/gthhsgibqc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj202588.top/gtijpmkmsx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtmsfdpcmx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yanxiufei.cn/gtzfkgfyih.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtlgclwwlc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwwticflb.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtgqyziwrd.html

================================================================================
来源：http://hz.52xcode.cn/gtirgdozlv.html

[K01] 对象转 JSON 字符串
来源：http://hz.sweek.top/gtaqbaxgwo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gttaijphfl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtmmzkdtoz.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtrhmxitiy.html

TS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtkywgolqx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gtbuougjvn.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtzyohvewr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.quarkkingdee.top/gtwlacbcpn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtjzuneiwb.html

[K02] JSON 字符串转对象
来源：http://hz.hnqzz.top/gtwnhtgyui.html

Py:   json.loads(s)
来源：http://hz.yueranfly.top/gtzpqtdvfp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtnacqtipa.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtbydolawe.html


<!-- 参考信息 -->