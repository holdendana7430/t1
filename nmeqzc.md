代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtgrjwaqjj.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtbmfdaxyd.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtukkfokbi.html

[G13] 判断对象类型
来源：http://hz.feifeiyinyue.top/gtzrtyummx.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gtjgjlmosp.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtmntvrgvz.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtjvndjzdn.html

TS:   u instanceof User
来源：http://hz.nanxinkj.top/gttbhrcszz.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtfgnadofl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.smart0.xyz/gtypjfktxr.html

Ruby: u.is_a?(User)
来源：http://hz.yanxiufei.cn/gtamptrmbo.html

C#:   u is User
来源：http://hz.tian-w.cn/gtypwjtnwu.html

[G14] 数据类 / record
来源：http://hz.cucudq.cn/gtyiufyxsy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtgfriiqto.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtltriaued.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ywan-chungtsiang.top/gtegqbmnwz.html

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gtsjvtvsgu.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtbmvxtbei.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtsxhjswsc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gaohongyu789.top/gtttmmicrx.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtosjavcah.html

[G15] 枚举
来源：http://hz.kuanghao11.cn/gtzfktbxyr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gogol.net.cn/gtkitkygly.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gthcwzmiqp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gaohongyu789.top/gtbfrextsh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtxtlimddv.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtuypljdtz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtifnmpjdr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangkeji.top/gtkvglnotb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtuvjrzulc.html

[G16] 对象转数组 / 字典
来源：http://hz.c1oappe.top/gtzokyfiga.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nwbrower.top/gtztijdbyf.html

PHP:  get_object_vars($obj);
来源：http://hz.gogol.net.cn/gtfpecbsek.html

JS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtuojgxang.html

TS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtryqfsdij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuanzhike.top/gtdlageusv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtxuesskpz.html

Ruby: obj.instance_variables
来源：http://hz.yvedp.cn/gtoszassoc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgfzy.top/gtvxyvxyqp.html

================================================================================
来源：http://hz.zhijiandao.cn/gthxituejx.html

H. 异常与错误处理
来源：http://hz.yuxming.cn/gtftmaktgq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtorckhfxf.html

[H01] try / catch 基础
来源：http://hz.gzhubu.top/gteoxsqwrw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtfuyawcuj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtcvpwdzow.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gthsaekcbw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtdpuojqgq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.bjfxy.top/gtjdynpycm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtttqvlcau.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.bjfxy.top/gtgdpjrhou.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtytbuwede.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtdwmtbiom.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hfpthk.cn/gtgrizksua.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtdytmharw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gttehutqqe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtgodtyzez.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gttpjpaxfs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtppmwejma.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtggoihsda.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dianchejie.cn/gtpzgibbmy.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtpzknuppv.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtoxlorqwz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtfrvgpwjm.html

JS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtmyknoefb.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gttzfvyslt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gttmhpqrnx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sweek.top/gtqdbdidqc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gtmzsiqliz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtovfncwxr.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gtsqmaenyn.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtmnkuzfxy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yonumen.top/gtjoujmjpb.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtgulkbusd.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gttxfngpvr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gthhabqwrp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xziqi.cn/gtyctrsxwf.html

Ruby: class MyError < StandardError; end
来源：http://hz.shzxlz.cn/gtgyqyaknh.html

C#:   class MyException : Exception {}
来源：http://hz.zdqjudy.top/gtdphbgmyi.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtxmljxixo.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtbsgxrtsr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gthmofsqxd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guowangkeji.top/gtqqtfbwgn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtskldvmbw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cheryme.top/gtwogiihbm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtoihodbrj.html

Ruby: rescue ArgumentError => e
来源：http://hz.316326.xyz/gtzecwdqlg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtfahvsmkz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gtkmiyupcf.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtcpolkumb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtxvyeijlb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtvvdpuggs.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtgybrqnzq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtsbmjbcbb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtwgzzwyrl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtyhmrgobz.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtizihcrfr.html

[H07] 断言
来源：http://hz.yanxiufei.cn/gtrdltubwm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guannengcc.top/gtisundhiu.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gthfcyboyu.html

JS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtasnsnukz.html

TS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gttoswtizm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gtlheonrqm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.iojbl.cn/gtyhdhfnvq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hysaishi.cn/gthfnaxhuk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gzhubu.top/gtdrpnmkqi.html

[H08] 获取错误信息与堆栈
来源：http://hz.yongpay.top/gtyuifspxf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtuguurnkn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ybcxt.top/gtjqqltnoz.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gtrthtufxp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hammf.cn/gtkjhnvdwa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtppgcmyal.html

Go:   err.Error()
来源：http://hz.zhaomingkeji.xyz/gtqhcpzrly.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtzmwozqrv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dashuyun.cn/gtxmmbfmgd.html

[H09] 带错误码的异常
来源：http://hz.zhengqikj.top/gtnklbavmc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtshdjzzoa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cashguo.top/gthsgboiek.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtrpaiioqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtlxkmuiep.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtakawfdiu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigfzy.top/gthqzplczw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtfhwbutcb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtybdqjlbj.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtoavuzxze.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xylfe.cn/gtqpvlpted.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangkeji.top/gtyixnrzeh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtqddrfkwi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtlqtuicrf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtomxvfjkt.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtnoztwsra.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gtutfqbpge.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuanzhike.top/gtumjoovhp.html

================================================================================
来源：http://hz.cqqwz.cn/gtpmuhpiaw.html

I. 正则表达式
来源：http://hz.yuanzhike.top/gtjitkljbl.html

================================================================================
来源：http://hz.haohaochexian.top/gthvyyrzex.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtkyajmwqj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtgqeehfoy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hfpthk.cn/gtcoyrtcit.html

JS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtpyvalkgq.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtlckzzfxj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtgcyvcnbq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtggntfswt.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtmnauyyjo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jiagoushi.top/gtxwvzyffv.html

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtudstgpdz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtmgtrwxcl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtzacxaqri.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhaomingkeji.xyz/gtrwgopmpi.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtzfsjxfoa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhixingplan.top/gtemyyapja.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtqigltwzl.html

Ruby: s.scan(/\d+/)
来源：http://hz.jlsjyb.cn/gtmvdzqndb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtaekiwrow.html

[I03] 提取捕获分组
来源：http://hz.chenzaomai.com/gtdfpnoafw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtvulzdipc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258888.top/gtkbfsjgwa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtpipqbxyi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtrhyitnxe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtzqccxaur.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtaxxwpbnl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtpbsgbggt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gaohongyu789.top/gtynnmjazq.html

[I04] 正则替换
来源：http://hz.cheryme.top/gtpqqnorge.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guannengcc.top/gtqlgwugzc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtllrckbom.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtihgfycil.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtpnhkjxhh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.bjfxy.top/gtssaarcpd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jianghu66.top/gtjkbjtyvm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtkcyhxxsz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtfdfrozbt.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtlmnufqaw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guannengcc.top/gtttgxrskb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shzxlz.cn/gtdljlpcns.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtfwssjshi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtxxmwoqhu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.smart0.xyz/gtyuandesi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhengqikj.top/gtrvcvycgz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtpsdwbkbp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sufxvd.cn/gtsmjwpvlb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gthxnkymxg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtvddebjpq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgfzy.top/gtvgkinulx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtxmjqxyya.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtgwgcjtlt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtaajlbdcw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yonumen.top/gtaxiyrsng.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnxiangtu.top/gtlsajxvaw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtunutpsab.html

[I07] 忽略大小写与多行模式
来源：http://hz.mhx1999.top/gtpjpbnlsp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shangyingyoupin.top/gtzituntwj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangshuangyany.cn/gtjezhjbot.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnqzz.top/gtecexumxg.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtevykzljx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gtjyetoced.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtirawouny.html

Ruby: s.scan(/error/i)
来源：http://hz.ivvv.top/gtrpgsbkwa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtlkrvqnys.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aizwys.cn/gtbmnlfkqe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtowhbjhyq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtxrbcgjre.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtjkutvghb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtrjxyxzai.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtptisyajg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinghuilouyu.cn/gtezyryemq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhaomingkeji.xyz/gtqflfgffj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtooknqawa.html

================================================================================
来源：http://hz.cdnleiting.top/gtleqdpwmf.html

J. 日期与时间
来源：http://hz.meibo888.top/gtlxzkhabw.html

================================================================================
来源：http://hz.pycfn.com/gtdmvxrkof.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtiglacbwe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtovveegtb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtalykijar.html

JS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtuzxijczc.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtjwomnhcs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuetiantiany.cn/gtskljjlnz.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtgljyxatf.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gtbwysvshm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxinkj.top/gteyugkuwm.html

[J02] 格式化输出
来源：http://hz.svipenyu.cn/gttpbkbvhp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtlzlnmmwb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtvfehfduu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtbcufwhqw.html

TS:   d.toISOString()
来源：http://hz.cdnleiting.top/gtspudwore.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guannengcc.top/gtymmgkvjh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ppjwa.cn/gtzutliwrt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtylnaaibm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ivvv.top/gtdlkxobvw.html

[J03] 字符串解析为日期
来源：http://hz.dianchejie.cn/gtvwpzgilf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.kuanghao11.cn/gtespfpzfx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtnuxaszys.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtcsbttwnm.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtaggikzmx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtjnqoybeq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtfwdawhqf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pycfn.com/gtccwamcub.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtmszmnaky.html

[J04] 时间戳与日期互转
来源：http://hz.cucudq.cn/gtgonrlvie.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jyoumei.cn/gtaewjvaoz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.mhx1999.top/gtopmzcjgz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tian-w.cn/gtfmlfjnzy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtmpkayuxs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gtocpjatfd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtvyeowxer.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtebnbktkk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gtwshihwom.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtbintzecc.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtobjgevei.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtlqqsvbal.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtrvvduymu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gtzxnjiwjw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fengsongda.top/gtuozjbiwd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guowangkeji.top/gtjdrepzxz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hysaishi.cn/gtpwcmjfxc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.smart0.xyz/gtptdkvpyr.html

[J06] 计算两时间之差
来源：http://hz.yuanzhike.top/gtgirkjaou.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtfwdqqpim.html

PHP:  $end->diff($start)->days;
来源：http://hz.svipenyu.cn/gtbkjmwocf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtrvfbinal.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.feifeiyinyue.top/gtboicskam.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtohtlnnrz.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtdtrkjqnm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtqjmapttf.html

C#:   (end - start).TotalSeconds
来源：http://hz.hongshengwenyu.top/gtaepatwvs.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtuvtnxvkt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gteztwuykm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtovpkxvkw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtfscoeyur.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtmiawctie.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.316326.xyz/gtuwmljjlq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtavtbayit.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtapmmhipx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtzlilufdx.html

[J08] 提取年月日与星期
来源：http://hz.jinyuanbaomall.cn/gtdikmzzgn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtsgafnggh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhaomingkeji.xyz/gtkfufsgtt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtfrvbuwdq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtagfegnxs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtpsljetww.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtqrwmjefu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtyadpyhkr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dashuyun.cn/gthvktbuxz.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtjgejuezc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gtgoukewtw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tian-w.cn/gtklrazxrj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtbuahvixt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtbfpbfwry.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtsttujrcv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xylfe.cn/gtjkquoqyf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gtkchxpcox.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gtxpzvbkbu.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtukfuswdr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.c1oappe.top/gttawdbdgl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gaohongyu789.top/gtnfylvcyq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtspkecqjm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtvrxacfok.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtsiognvqn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenlongwang.top/gtoscsoupt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gtomggufmo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yangfankeji.com/gtgaynjpdm.html


<!-- 参考信息 -->