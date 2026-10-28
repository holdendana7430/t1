代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.snrcjt.cn/gtdmtvdstj.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtcpafkkbx.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtjadufmys.html

TS:   u instanceof User
来源：http://hz.yonumen.top/gtoamgruzv.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtsxowwbzt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.mhx1999.top/gticefnwok.html

Ruby: u.is_a?(User)
来源：http://hz.feifeiyinyue.top/gtljebuzwc.html

C#:   u is User
来源：http://hz.shanyushiyangtech.top/gtopymgdjr.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtdgwgchzt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtujuqfkza.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gtuxcugzmc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jiagoushi.top/gtjizxzwtc.html

TS:   type User = { name: string; age: number };
来源：http://hz.nwbrower.top/gtoivtjrhg.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtwbumgkas.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258888.top/gtyjlikzhy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtolaqralt.html

C#:   record User(string Name, int Age);
来源：http://hz.xziqi.cn/gtoozbhhtu.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtlzpcyxtn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhiwuduotai.top/gtdfixfyvz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guannengcc.top/gtpqtojkmh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gtdfaxphgq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtutaaawoo.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtdrzziubm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fengsongda.top/gtmxwdoqzk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtadyscwnk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtyubcyovg.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gttkcrnqyb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dashuyun.cn/gtfapemjbn.html

PHP:  get_object_vars($obj);
来源：http://hz.yonumen.top/gtecaonuwb.html

JS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gthjqwdrzm.html

TS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtweoetfeo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtqjuhitbg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuxming.cn/gtmfgfwklc.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtqhepitcm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtrjqnduch.html

================================================================================
来源：http://hz.yuxming.cn/gtqnhtvcgq.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtniezmygv.html

================================================================================
来源：http://hz.fengsongda.top/gtqbrkmfiw.html

[H01] try / catch 基础
来源：http://hz.feifeiyinyue.top/gthtysdbtq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtixepbrpf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtxzlksqgb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yonumen.top/gttbqdcrme.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtlyagbybo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgfzy.top/gtuvqxsktt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.kuanghao11.cn/gtfatupvif.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tanke756.top/gtwbjpxhvx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gtesshtyja.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtlabpsory.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtxyosnxcz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtfzbxcady.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gttafopmvq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtdqjosxby.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtbdhizvfy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtnhcrbymk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtrhvummtu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuxming.cn/gtkgaipcxt.html

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtqmwkyfve.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxuanxn.top/gtfedtlaok.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtidkydsxu.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtmrmlkvsq.html

TS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtlqxneddc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtyipzodzn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenlongwang.top/gtkeyktefh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.0kj1m.cn/gtmyjcnilh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtsuwznmkb.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtflifwhvz.html

Py:   class MyError(Exception): pass
来源：http://hz.chenzaomai.com/gtuhmufhor.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtqzhhbfmu.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtvqjyelnn.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtmgctpkoz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtqxtfdpzh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtqjsyesoi.html

Ruby: class MyError < StandardError; end
来源：http://hz.havefunace.top/gthlvmfeog.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gttdvzltdi.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtsslvhrle.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtrpwjxdne.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtfcixuklm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtabllyxut.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtjsncsfsd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtdqymrtew.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtleyhqmmh.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtldynyuqm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnxiangtu.top/gtvxznxams.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtzxfzdijj.html

Py:   value = d.get("k") or default
来源：http://hz.chenjidiqi.icu/gttfrqeefd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cucudq.cn/gtgdbwbrwg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtpvizdyms.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtrqruxsib.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ivvv.top/gtchyfevga.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtkctuizyu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gthqiouwzy.html

C#:   obj?.A?.B ?? default
来源：http://hz.hongshengwenyu.top/gtcnhfyeiq.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtirdqrryj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydzc1.top/gtypaqozwf.html

PHP:  assert($x > 0);
来源：http://hz.gogol.net.cn/gtgcusylyn.html

JS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtihpbwqst.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtqdllbfbe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtgagxgihx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.vqdsnc.cn/gtcoelakiv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangshuangyany.cn/gtnoyvrgpp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daria6918.cn/gtalcawfbk.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhijiandao.cn/gtmrxtodci.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtwstoqtju.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj202588.top/gtshgopnjh.html

JS:   e.message;  e.stack
来源：http://hz.tianlin.xyz/gtoptybggn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258888.top/gtfsifqtzn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtqffrnarl.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtylchfjok.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtncgkeckk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtkqszbqbj.html

[H09] 带错误码的异常
来源：http://hz.cdnleiting.top/gtfuffaofp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gtvccgdowx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gthkgusfva.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtxomxcxub.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtfbzljmwd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jianghu66.top/gtgwkmpqbw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinyuanbaomall.cn/gtzhrtqawn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangdashe.top/gtounzedgl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtywmyfxvg.html

[H10] 资源自动释放
来源：http://hz.kuanghao11.cn/gtpvoiczht.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.svipenyu.cn/gtuzlvgjuz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aizwys.cn/gtyoyvtbbp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gtxozejkol.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtyeigvoxd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gttjhjlrib.html

Go:   defer f.Close()
来源：http://hz.iojbl.cn/gtyvgxvles.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtyvbuqgrf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gthgaduyst.html

================================================================================
来源：http://hz.xziqi.cn/gtpfsrrnyd.html

I. 正则表达式
来源：http://hz.wangdashe.top/gthbolfrqn.html

================================================================================
来源：http://hz.wangdashe.top/gtmdzmeqhd.html

[I01] 判断是否匹配
来源：http://hz.meibo888.top/gtwrtachpb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gzhubu.top/gtvouscxjj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtzalzmfrn.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gthacsgdfv.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtkseesfnt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtchaaeaie.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtrlrhptfq.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtiibbygty.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dianchejie.cn/gtmrrrzise.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gttgadpxul.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtuchlhjbe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gttryccllb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtaxeudshw.html

TS:   s.match(/\d+/g)
来源：http://hz.yangfankeji.com/gtkskaxawm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj202588.top/gthuzghcbx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtsyrdjejk.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtauxghklk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuetiantiany.cn/gtftqtxglm.html

[I03] 提取捕获分组
来源：http://hz.shzxlz.cn/gtcwxibwbb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtdxlzsojb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gtfsltwriv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.svipenyu.cn/gtnbkqiknx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangtech.top/gtyrpfjmej.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.smart0.xyz/gtwziyvcof.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtigimowqu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tanke756.top/gtospiicwp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shanyushiyangkeji.top/gtshfypsvy.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtxauqzuxp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtefetatei.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtmdaduljj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtuugojnei.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tianlin.xyz/gtqkpidbvh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gtyxmekuys.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtlpvhxdkm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigfzy.top/gtivbrpnpo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtcjqyhpyh.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gtpfwwchva.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtbeiizyrs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinghuilouyu.cn/gtiymmocss.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtxxulnmkq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtoqqlxcyo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtewbyxlwn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gthdjroqfd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtbbhpnsls.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sweek.top/gtfcxxdmcz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtdrloctpf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtegwyeixp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ehwqpu.com/gtkspptziu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtpstmcvmf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtoyycqszw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtvzmdagjk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhengqikj.top/gtaciorvrf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gttruqrtqn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gttwpqiqos.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtqbmnsjtj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigufen.top/gtyztuxqgo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtbcmbitrt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xingfuxueyuan.xyz/gtrfsmaoph.html

TS:   /error/gim
来源：http://hz.shzxlz.cn/gtmyvuksyc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gogol.net.cn/gtgbequgwg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtwroybeoa.html

Ruby: s.scan(/error/i)
来源：http://hz.zycfv.cn/gtlnixaenj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtcaqcfsha.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtlnyzplfa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhoulong.xyz/gtllzfnzew.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.quarkkingdee.top/gtumvigrcx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtcwbzgzfs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtkhjpbmlm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtetzyuolv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxinkj.top/gtshgphxcv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cucudq.cn/gttoweblkc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtuzkdyvnj.html

================================================================================
来源：http://hz.hfpthk.cn/gteqhovygf.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gtktgyyxsu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqyznjgrw.html

[J01] 获取当前时间
来源：http://hz.jianghu66.top/gtyzzkntfk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtushqvxud.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtlxncfcts.html

JS:   new Date();  Date.now()
来源：http://hz.jqgufenzy.top/gtrsleobfb.html

TS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtyuovwoay.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtwffbvddi.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gturxbydex.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtybpbvebs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtmfujobmh.html

[J02] 格式化输出
来源：http://hz.xuanzx.com/gtabkicamm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtksawinal.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtkninicqs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtqfecppfj.html

TS:   d.toISOString()
来源：http://hz.zhiwuduotai.top/gtrmchsyyh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtasrxwjxx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dianchejie.cn/gtmsinpcev.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtefdfoxft.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gtnirhrmpm.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtggolrtgo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.0kj1m.cn/gtygsoxfed.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.smart0.xyz/gtlrxhrvhr.html

JS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtkdhereld.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtnawpmtct.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtzpxnbtvo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xziqi.cn/gtktflxhof.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtjimuxsob.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtrljtpdgk.html

[J04] 时间戳与日期互转
来源：http://hz.birdmap.top/gtpraqovfk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.iojbl.cn/gtkkzjpnho.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gtgunsqvcy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtzadnkznn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gtcjxwujzm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtuujgnqrq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtlyhyvnmb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtgyfsnxmv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtnbexxime.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtfnpalnlk.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gtmfqtqnjp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yangfankeji.com/gtsdtjfiqp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtiteeofsp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtnvfncohw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtljfyepia.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtskhsnqto.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cheryme.top/gtrwsyvuif.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xylfe.cn/gtiaxkwaaq.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtrmlmkniy.html

Py:   (end - start).total_seconds()
来源：http://hz.hnxiangtu.top/gtxozoiykb.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258888.top/gtjgxgevlm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtztdeezif.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cucudq.cn/gtswrtlaxp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.svipenyu.cn/gttsniforh.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtuzagprsu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gtljmxmohn.html

C#:   (end - start).TotalSeconds
来源：http://hz.kuanghao11.cn/gtmzvoxtxz.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gtjgyhnvco.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtchktnsft.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gthpjitbzr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gttaodpgaz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtrrtelsrd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtyrxyweep.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gtvcvgozrd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtgcwudpuj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtnbdtaveq.html

[J08] 提取年月日与星期
来源：http://hz.c1oappe.top/gttkxukzso.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtzzvnrune.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj202588.top/gtbrintrkx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtpmhbaoux.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gtvmvodjsy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xingfuxueyuan.xyz/gtxnvkmuru.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtasjbkkta.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gotoacloud.top/gtwyzoeeim.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtmecwpvjq.html

[J09] 时区处理
来源：http://hz.zdqjudy.top/gtsjllgqfq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtpgzrdoqc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtcahrngex.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtjmhhroza.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtfubwepxz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.birdmap.top/gtfgvalrov.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hfpthk.cn/gtdbwyahqe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtypikrvjb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtqdpywkqg.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtezcubmat.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gtdmnjkrwz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtauyqjdsw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtwprrhbeb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuetiantiany.cn/gtghkobzby.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtamkgpnwg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yueranfly.top/gtabqpmbnl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtarzepwmo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gtcfquphco.html

================================================================================
来源：http://hz.0kj1m.cn/gtevrnyaof.html

K. JSON 与序列化
来源：http://hz.nwbrower.top/gtihndzhld.html

================================================================================
来源：http://hz.316326.xyz/gtasfrsyta.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangshuangyany.cn/gtyffmkfmq.html


<!-- 参考信息 -->