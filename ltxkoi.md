代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtwytwpzmr.html

PHP:  $u instanceof User
来源：http://hz.gogol.net.cn/gtnnxqtvqk.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtkftrnhgu.html

TS:   u instanceof User
来源：http://hz.jianghu66.top/gtwubbmbmc.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtcfdhsddo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtigwsdgvd.html

Ruby: u.is_a?(User)
来源：http://hz.zhaomingkeji.xyz/gtrnonywxi.html

C#:   u is User
来源：http://hz.snrcjt.cn/gthvwblqrs.html

[G14] 数据类 / record
来源：http://hz.hammf.cn/gtocpdjkvm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtzxbrhcdy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cucudq.cn/gtarlzlvpw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.bjfxy.top/gtzwwzhwhd.html

TS:   type User = { name: string; age: number };
来源：http://hz.vqdsnc.cn/gtgbeaxctd.html

Java: record User(String name, int age) {}
来源：http://hz.sweek.top/gtqxktboac.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yvedp.cn/gtvmmxwdsb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtbyjfkeqw.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtafvsvxfs.html

[G15] 枚举
来源：http://hz.ywan-chungtsiang.top/gtayjgdmuc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cashguo.top/gtzvathvln.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xinyue.icu/gtknrmxsaw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cqqwz.cn/gtxmrkppim.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtyykbwedv.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgfzy.top/gthwqurpwb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtwndetlcz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtmdngmxku.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtkgzhmcab.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxuanxn.top/gtghcmmhlq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnxiangtu.top/gtnaibyssg.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtltrylycw.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtjvbgpqsd.html

TS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtpurqlazc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtpjkrweuh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtojxvweqs.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gtaarfmfbx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gtvscxnktg.html

================================================================================
来源：http://hz.svipenyu.cn/gtnfpfupcw.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtjvoqqvms.html

================================================================================
来源：http://hz.yj20258888.top/gtntjelubb.html

[H01] try / catch 基础
来源：http://hz.gzhubu.top/gthylximwd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtpsrzitvy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtnhogumns.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtqfapiywi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gtvexaynap.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sweek.top/gthmatztnb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daxiang520.top/gtlbwerddd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtwcjnvdef.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.snrcjt.cn/gtnkrwjzcu.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtthbduqty.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shangyingyoupin.top/gtunjewphu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtajrjobcb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtqrvezfps.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtdpugjtbz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtlcjccttp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtvobwqbfo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gthwmgdcol.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtzyibehkh.html

[H03] 主动抛出异常
来源：http://hz.xylfe.cn/gtatzzzhsu.html

Py:   raise ValueError("错误信息")
来源：http://hz.shzxlz.cn/gtpfckixsm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gttrkzvdyg.html

JS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtsrtcevyy.html

TS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtyazqtoed.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtwbbvrkaf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gtqscnabek.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigufen.top/gtolcqdmxi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtgqhvrifh.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtlrtdvybu.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gthdwfemdo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtomvqhtxj.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gttlthygzi.html

TS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtnvgtywma.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtpuptkmcl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtyyyxrhsr.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtumyfnzre.html

C#:   class MyException : Exception {}
来源：http://hz.quarkkingdee.top/gthdcvixgq.html

[H05] 捕获特定类型
来源：http://hz.fengsongda.top/gteihpwjgz.html

Py:   except ValueError as e:
来源：http://hz.aizwys.cn/gtgjqvawon.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cheryme.top/gtipiytypx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtfcsrofmu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtgxikgjnz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hfpthk.cn/gtwztqplan.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtkntcpjol.html

Ruby: rescue ArgumentError => e
来源：http://hz.dianchejie.cn/gtgkxzvpar.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtkgfgbgvb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtaemjzuic.html

Py:   value = d.get("k") or default
来源：http://hz.hywenlv.cn/gtrbosixwa.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtdszxuyfs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtoevcubyh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtkhvmblmn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gtguroktrd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aizwys.cn/gtdisvzxef.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtunzsyyrr.html

C#:   obj?.A?.B ?? default
来源：http://hz.yonumen.top/gtmigaxvpz.html

[H07] 断言
来源：http://hz.fengsongda.top/gtvylnetxr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgfzy.top/gtuvqivnok.html

PHP:  assert($x > 0);
来源：http://hz.wangdashe.top/gthfxmaejh.html

JS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtsgciyneh.html

TS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtcgdtlpsn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.haohaochexian.top/gtnilrkika.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yangfankeji.com/gtawqllwwk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gzhubu.top/gtrcoqagbl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gtrjkwwgcx.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxinkj.top/gtwcxiectj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gtbvuceprh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.svipenyu.cn/gtymfumnqz.html

JS:   e.message;  e.stack
来源：http://hz.gotoacloud.top/gtqqtnrzwo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtmwctiyhp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtfsqhxiwn.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gtjgvisauq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jlsjyb.cn/gtewnwymem.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258888.top/gtqlcmunkc.html

[H09] 带错误码的异常
来源：http://hz.daxiang520.top/gtjlqhbblc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhoulong.xyz/gtekadnydx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtlcqsijgi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtjsxwjgbn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.birdmap.top/gtvorhupjz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtdcpixidl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cqqwz.cn/gttdvwsuog.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtgztkiwnb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xylfe.cn/gtzynsulkf.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtsnvrzhyd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtviwpbaqh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sxryk.cn/gthsatefte.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtbxtrxwdx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtrncyjxhn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xingfuxueyuan.xyz/gtlixezijv.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtxghmsxsa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtcgseglxb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtfyduzkoi.html

================================================================================
来源：http://hz.ehwqpu.com/gtbhwtmzsf.html

I. 正则表达式
来源：http://hz.daxiang520.top/gtsbzfpjmr.html

================================================================================
来源：http://hz.9152youxi.cn/gtkwubzogn.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtokyobsfn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtcvuliiqb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yanxiufei.cn/gtsypawtly.html

JS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtkgxmpbzy.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtexhrokad.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtsxpynojb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.snrcjt.cn/gttavqvmee.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtmyahvoew.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yangfankeji.com/gtvikrogto.html

[I02] 提取所有匹配
来源：http://hz.chenlongwang.top/gtejugsbwj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtgrcrtrzn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gtetwzhpqj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.mhx1999.top/gthiljlucp.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtofoncinj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xinyue.icu/gtygnthczf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shuidangran.top/gtgjuihmme.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtbzgkqzxu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yongpay.top/gtrvcejtgj.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtpmjbrmne.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinghuilouyu.cn/gtgeiuedlp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gtraqlqckb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sysykeji.top/gtarerzdwq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.aizwys.cn/gtcolyuuex.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtqgvvhfrb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.birdmap.top/gtftdzevlr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shuidangran.top/gtzgmiahlr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtkjaeosto.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gthjpwefkx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtwmmqssma.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ivvv.top/gtxfnvzdsh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtjxjdkgtv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtscemugzu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.c1oappe.top/gthebtlqsk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cheryme.top/gtxjpwluqu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.mhx1999.top/gthqknmzva.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtgrrluqhh.html

[I05] 按正则拆分
来源：http://hz.xuetiantiany.cn/gtekedjycy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gtxpxourhd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dianchejie.cn/gtwdagzgxh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtwxalankw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtdxlekfzk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.mhx1999.top/gtlyeksvxz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gtkkmhvcxg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtqtbajepy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtbkwvlugh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yanxiufei.cn/gtevdlwcmf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtnsiyikiq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.andypj.xyz/gtlnauysib.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtllbwricg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtykidzqmj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtmdwxpxbj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtlvjmkcub.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtogkntnlk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtjwlwhkpz.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinghuilouyu.cn/gtyytnuadc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinyuanbaomall.cn/gtkjsuoooi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gtalhzobmt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sxryk.cn/gtorrnvfuh.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gtqxmxmvbp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtmbykyqbq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yanxiufei.cn/gtzyorsrst.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtqyqdnrlt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.haohaochexian.top/gtubajinuc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtmgldzzlv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhaomingkeji.xyz/gtchebqgkk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.mhx1999.top/gtajiurqep.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtgqlhmkvt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtmbmgylgd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtkctmqecr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.andypj.xyz/gterktviso.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtsdcnrulo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtyxlixwfn.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdgwpeibw.html

J. 日期与时间
来源：http://hz.ybcxt.top/gtslesmpua.html

================================================================================
来源：http://hz.iojbl.cn/gtublheigw.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtnytjqigu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtjeyzkrvz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtqkytlrko.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtyhrntsui.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtaegxdhmv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtxlkfqpsv.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtgtewzvjm.html

Ruby: Time.now
来源：http://hz.jyoumei.cn/gthjabqfgm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtnscnebcm.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtivovsiom.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtaljjvyvz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtmsuaoexm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tianlin.xyz/gtpukdigla.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtnjemtuqz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hfpthk.cn/gtwyhmlpdn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtbxbmasjf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtzjskvxpz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.feifeiyinyue.top/gtrphbbmwc.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtyrqsgllm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.mhx1999.top/gtemtgwfml.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtmrvntrff.html

JS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtraivnuyj.html

TS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtbbvjrjtw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtkrnertsy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zdqjudy.top/gtmryucovz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtstiuhtxp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtpwiqabfd.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtwxvzbbzp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gtdpgkogsz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtrlhzmodb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigfzy.top/gtlclrhylj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tanke756.top/gtpteqezvw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtaexivwrn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtncmgxmrh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nwbrower.top/gtpyngctea.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtpezngxvv.html

[J05] 时间加减（加 7 天）
来源：http://hz.hongshengwenyu.top/gtbpepznbf.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtxkkvbtfc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtsctxiqtu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtcgxjlrit.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtrmnvrhzi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtzpjvvegr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gttpvfslom.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtbujdygts.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangshuangyany.cn/gtbamvqntx.html

[J06] 计算两时间之差
来源：http://hz.zhaomingkeji.xyz/gtsruebwmp.html

Py:   (end - start).total_seconds()
来源：http://hz.dianchejie.cn/gtwpyugnno.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuanzx.com/gtcmbnkprw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hysaishi.cn/gtznudzrxu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gtxrvfvjgn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtawrttajq.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gtqlnghnqx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigufen.top/gtsnkwascm.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258888.top/gtghfmbfbl.html

[J07] 比较两个日期
来源：http://hz.birdmap.top/gtyhvrfsrp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtmxmfbeme.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gthbkecuyx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtupedrjoi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtjgqtmwoz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aibaodan.cn/gtxvhbtool.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtlaeucytl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtmkhacugl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtdftunodv.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gttetqzche.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dianchejie.cn/gtrnuaqpub.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtrhzzrpim.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gotoacloud.top/gtybsvdepz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhengqikj.top/gtqwmfaaah.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gtpohzboqz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258888.top/gtfkvbnaui.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydzc1.top/gtbilbrict.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gtyuifcrgh.html

[J09] 时区处理
来源：http://hz.zhijiandao.cn/gtbnpjcaao.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yueranfly.top/gtjtprvgrs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gtlxucsifu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtpbkgkjri.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtnpjoxmos.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.haohaochexian.top/gtmhvjwvwj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtusoaylxi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtjzdhbqiq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gtegnprtmn.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtniepscqk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gtxwmdhmes.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.havefunace.top/gtmhfcvzav.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtjnnxvlrm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtxaakrgjl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenzaomai.com/gtlavuyvag.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtkukohsda.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tanke756.top/gtuimrlgbb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtnbmztegz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmbwjkzei.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtgzvmoiyx.html

================================================================================
来源：http://hz.yongpay.top/gtmgddkagf.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuanzx.com/gttgvligtb.html


<!-- 参考信息 -->