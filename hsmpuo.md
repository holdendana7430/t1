代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtkmlpcyyc.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gttocipaci.html

JS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtnkbmishk.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gtjhbfjhyl.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtdtwckqej.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hongshengwenyu.top/gtdswydgjg.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtpakaosxd.html

C#:   u is User
来源：http://hz.ybcxt.top/gtbqqzxbbe.html

[G14] 数据类 / record
来源：http://hz.yanxiufei.cn/gtptqyyubb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xziqi.cn/gtdnamihee.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtkwvijwdq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtqzopwkoc.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenjidiqi.icu/gtvpupwsob.html

Java: record User(String name, int age) {}
来源：http://hz.yuxming.cn/gtndfodzvh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtzbsqkloj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtwhbhuyky.html

C#:   record User(string Name, int Age);
来源：http://hz.sweek.top/gtkqsnqupi.html

[G15] 枚举
来源：http://hz.sysykeji.top/gtfuzvbilt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtkjrmwmdw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xinyue.icu/gtxmqebfns.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuxming.cn/gtfgkywqxk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtmktvdfwe.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtvcxcvjqi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gtdkspcqlg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtjgghkzps.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtonzijpcu.html

[G16] 对象转数组 / 字典
来源：http://hz.nwbrower.top/gtrxikgogy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hywenlv.cn/gtmiilhkqx.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtptgotxid.html

JS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtldwkpoxe.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtdrtupnfh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtomxfwnek.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yonumen.top/gthfhcfevv.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtzxetgrne.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gttmdcqvhu.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlojunxsm.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gteienhfzj.html

================================================================================
来源：http://hz.dashuyun.cn/gtkwhawaku.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtofoveuqk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhaomingkeji.xyz/gtywwdxgox.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtnmjzthmv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtgnpywxri.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ivvv.top/gtnrxkebfa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgfzy.top/gtsrnpekrq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cheryme.top/gtrjhqwpwq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gtbzchwcku.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aibaodan.cn/gtsukjxaob.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtaoknpmhx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.andypj.xyz/gtsauqdbjw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtbjaqgofy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtqlbyypzi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtarzhjrrh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtpjnzsabw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhijiandao.cn/gtfeoaiaen.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtjesadryx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.iojbl.cn/gtsjmakpjc.html

[H03] 主动抛出异常
来源：http://hz.meibo888.top/gtfkbeuafm.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gtyfmkznmt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtxuhesrwb.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtvgdawzqw.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtkjzxwbxu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtgwxpisgv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sysykeji.top/gtzewnzroy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgufenzy.top/gtwdkibxli.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gthetdmilr.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtzsafntzr.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtkwfophpe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtddhzneai.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtnkqxfdny.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtbusqlqwq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtnqaswbrp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtrssaikqc.html

Ruby: class MyError < StandardError; end
来源：http://hz.cheryme.top/gtyppkiimx.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtyolsahaf.html

[H05] 捕获特定类型
来源：http://hz.chenzaomai.com/gtntsyxlgr.html

Py:   except ValueError as e:
来源：http://hz.chenjidiqi.icu/gtredsvjne.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtwswxwldv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtbbqskruz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtkohpoqyz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtzsntugei.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.c1oappe.top/gtrouhwipt.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gttppzvwdu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dianchejie.cn/gtnnsauzyd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtejgqltql.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gtoymqooxm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtanmqishw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtoihgxzjn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtdkuuluhv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sysykeji.top/gttkcgkkdt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinyuanbaomall.cn/gtzrjiudqo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258.top/gtijcojgwm.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtkmyarjvx.html

[H07] 断言
来源：http://hz.yueranfly.top/gtddewyczf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtpeixtplu.html

PHP:  assert($x > 0);
来源：http://hz.hongshengwenyu.top/gtenvxljid.html

JS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtxpolvrec.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtczdyxhtx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtseoivsgn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtsgbgytwc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtahjcgmyx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtafebqjui.html

[H08] 获取错误信息与堆栈
来源：http://hz.haohaochexian.top/gtpkueogmh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gthxviuojd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtqktoosqu.html

JS:   e.message;  e.stack
来源：http://hz.gotoacloud.top/gtcfielaid.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtefenekzd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtjitbdhai.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtrdnrxcrt.html

Ruby: e.message;  e.backtrace
来源：http://hz.daria6918.cn/gtqwyrakep.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtrvlsihfj.html

[H09] 带错误码的异常
来源：http://hz.yuxming.cn/gtgjoltlkx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gtypewyldk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhaomingkeji.xyz/gtjpmlzqac.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sysykeji.top/gtnaqibmej.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gtnddutxmp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtskifwqqs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtsoamatlr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtpfotiurs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cqqwz.cn/gtbcwtmsst.html

[H10] 资源自动释放
来源：http://hz.zhoulong.xyz/gticbepknx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtxmnrpjwc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtlfcqfonv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtstiuhcnd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gthuoffoyq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangkeji.top/gtmkzcgbfa.html

Go:   defer f.Close()
来源：http://hz.jinyuanbaomall.cn/gtkzgroddg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtmirwyhlg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtqhuqirco.html

================================================================================
来源：http://hz.sweek.top/gtwwcpzvby.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtdheolauj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtavjdophp.html

[I01] 判断是否匹配
来源：http://hz.aizwys.cn/gtprcgdblv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtaaapaetw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tianlin.xyz/gtbohyiikz.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtrehjtjnh.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtbtkgyhzt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtvnvalfqu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daxiang520.top/gtjqxmwzwy.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtuaicdeki.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtbmimhzfj.html

[I02] 提取所有匹配
来源：http://hz.zhijiandao.cn/gtyyefolth.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtppvjnhxc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gtivieiacp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtvdyloajp.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtotvcpyul.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtnzigxbmk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtjtkwjsvd.html

Ruby: s.scan(/\d+/)
来源：http://hz.birdmap.top/gtegkfniev.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gtzsaebuue.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gtzwolepmh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtrlophtth.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtmutxgnbb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ywan-chungtsiang.top/gtunqmiyai.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pengpengdd.cyou/gtfhumufzi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtewsddrrd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtsklzsmdy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tian-w.cn/gtlgqsijvp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sweek.top/gtdhnhyanx.html

[I04] 正则替换
来源：http://hz.yj20258.top/gtnvagblup.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gtorewujqi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtohoxhowj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sysykeji.top/gtxyqbbwfr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtrouldjnr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gttmiermlp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.quarkkingdee.top/gtqddooasz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhongyouzk.top/gtrtcxhyvo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gttmaytqcl.html

[I05] 按正则拆分
来源：http://hz.cqqwz.cn/gtnrwclnhb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtjevgweue.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtfllntphn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtffduwheb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtildlbkol.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gturzyzcsl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.redwolf501.top/gtuqxsytvl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtqwozhydc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.9152youxi.cn/gtwouwrfgh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.c1oappe.top/gtrowcroux.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtpfneyvrv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtbvchbuuq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtkgbehvcs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtupkbuucc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangtech.top/gteitvixab.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtuthitskk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhiwuduotai.top/gtcskhqani.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtlnoybajy.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinghuilouyu.cn/gtgyworfls.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gtysnwaadq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.iojbl.cn/gtdcijahxd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hongshengwenyu.top/gtmdxkcesz.html

TS:   /error/gim
来源：http://hz.jinghuilouyu.cn/gtevudeveo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhiwuduotai.top/gtqlhhwanh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtgcyyjdoe.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gtyfyfoior.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtyzjowfoz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtzbtcmcnf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtnlskxomn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gtawooujyi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtgzhchyfe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gthplzdedb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtzchxolep.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fzhhl.top/gtwmurmobn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtoobmteqs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gthgzryalv.html

================================================================================
来源：http://hz.zhengqikj.top/gtgiwylazw.html

J. 日期与时间
来源：http://hz.xylfe.cn/gtrkgadtzd.html

================================================================================
来源：http://hz.nwbrower.top/gtnhgydnyg.html

[J01] 获取当前时间
来源：http://hz.jlsjyb.cn/gtbybqjqvj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtnjizmnet.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtnmgdgeko.html

JS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtqpbpfiss.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtwhsfacqk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtftxsijrr.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtjhvxvszb.html

Ruby: Time.now
来源：http://hz.zhengqikj.top/gtoyrnfhab.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuetiantiany.cn/gtlmcxaqzk.html

[J02] 格式化输出
来源：http://hz.fzhhl.top/gtugdcgjxq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtkioszail.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtylfvwvnq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtvzbchnfo.html

TS:   d.toISOString()
来源：http://hz.svipenyu.cn/gtbbtcarxa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenzaomai.com/gtaxtxkhug.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sysykeji.top/gtyiizszxx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gthxpndnda.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtpsiasdwy.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtdezupaos.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhongyouzk.top/gtqdjdsoqs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenzaomai.com/gtkjplbaii.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtqspwvrhp.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gthcxyrgdl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtleauvbit.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj202588.top/gtklolykcr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gttneeamyc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtrtysbbev.html

[J04] 时间戳与日期互转
来源：http://hz.dashuyun.cn/gtratekpjn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aizwys.cn/gtrcumfesm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangdashe.top/gtzqvcalwh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gthqpmrohi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuetiantiany.cn/gteoubzbkd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.meibo888.top/gtjbpkedkt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtarjjstqb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzhubu.top/gtbrdufita.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hywenlv.cn/gtngemgksu.html

[J05] 时间加减（加 7 天）
来源：http://hz.xylfe.cn/gtqvmhkfxu.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gtuxgpemkw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtdfyangzw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gthcqwvsod.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtizdrhfox.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenjidiqi.icu/gtwfvjikiq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yvedp.cn/gtssaprytc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gtznlouxvb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.birdmap.top/gtcggrrqki.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtapifzfun.html

Py:   (end - start).total_seconds()
来源：http://hz.vqdsnc.cn/gtfyjxhcwg.html

PHP:  $end->diff($start)->days;
来源：http://hz.hywenlv.cn/gtzkoclfwf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtoxdsrzpy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnxiangtu.top/gtiifqbjcj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtdlluuqlb.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gthaysxzxv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtbgzmyepd.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtomecjjzu.html

[J07] 比较两个日期
来源：http://hz.tianlin.xyz/gtuzpkkuem.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtgmeefbbe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tianlin.xyz/gtfmdyolcc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtooqbgdqd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gtvaszrarh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtwsgfbiet.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtjgwnqlnb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtrlafnbky.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtjjitalnq.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtidyvmccd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtvhtsrlel.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.havefunace.top/gthapytxng.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtbqhtkebp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtlyfxthqb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gtewsnyfbe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xingfuxueyuan.xyz/gtwffqoyfi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtckelmrqg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtweiwzghq.html

[J09] 时区处理
来源：http://hz.yvedp.cn/gtvrtlryie.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtzafuuava.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtihifuucz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtvshtaksd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtvawwxdgm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtiawigrgb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.svipenyu.cn/gtffinqzlk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gthzwiqlnw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtddeodsaw.html

[J10] 取今天 / 本月第一天
来源：http://hz.shuidangran.top/gtucsueexy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gtetapnkdo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtdbhzohdo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtgzvthxuj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtwklzfvrd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtzunuosxf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhiwuduotai.top/gtfezyokek.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtjbtgocsq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtzwaewatt.html

================================================================================
来源：http://hz.cdnleiting.top/gtjuhnxabz.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gteqrpebof.html

================================================================================
来源：http://hz.hywenlv.cn/gtvkymywlf.html

[K01] 对象转 JSON 字符串
来源：http://hz.jyoumei.cn/gtvoallnyj.html


<!-- 参考信息 -->