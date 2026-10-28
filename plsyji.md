代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtyyhdueeb.html

Ruby: def to_s; @name; end
来源：http://hz.ppjwa.cn/gtqjvpqtnt.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gthmviaoxi.html

[G13] 判断对象类型
来源：http://hz.0kj1m.cn/gtmhqxjiwn.html

Py:   isinstance(u, User)
来源：http://hz.aibaodan.cn/gtyvdyiolx.html

PHP:  $u instanceof User
来源：http://hz.xylfe.cn/gtvpjumtwq.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtqfxexmdv.html

TS:   u instanceof User
来源：http://hz.yvedp.cn/gtfpishsnn.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtdhlwktrd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtejowjsbt.html

Ruby: u.is_a?(User)
来源：http://hz.yanxiufei.cn/gtumkasufz.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtrdbhveof.html

[G14] 数据类 / record
来源：http://hz.kuanghao11.cn/gtgchzhldx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gtnvpedpkh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtciqrbike.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gogol.net.cn/gtratuerpi.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxuanxn.top/gtmjcicgam.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtzkbbbcff.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtwyhfochh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtjlbaijds.html

C#:   record User(string Name, int Age);
来源：http://hz.xinyue.icu/gtdqwtssxt.html

[G15] 枚举
来源：http://hz.nanxuanxn.top/gthemgvxde.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtrkdfftta.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtpdrkgdrm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hfpthk.cn/gtjeszziwx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtcwodtzmj.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtwtdglhdu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gtyrjixsso.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gtdtcslowl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtrbgbgcxg.html

[G16] 对象转数组 / 字典
来源：http://hz.nwbrower.top/gtristtwsz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtyyarqdtv.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtoedhetar.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtzkncsvfc.html

TS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtqqfuhppe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtpgozawvw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtnhxlnspv.html

Ruby: obj.instance_variables
来源：http://hz.guowangkeji.top/gtyhcvoiga.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuetiantiany.cn/gtijmmpfzp.html

================================================================================
来源：http://hz.guowangkeji.top/gtlozwxxkv.html

H. 异常与错误处理
来源：http://hz.xuanzx.com/gtwlbmhiov.html

================================================================================
来源：http://hz.nanxinkj.top/gtmonobblw.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtlyvjwecm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtsvlfawxn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.haohaochexian.top/gtboyxqrmq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtraqcufsu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtbafthatq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daxiang520.top/gttyeytemj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtifkuwars.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhaomingkeji.xyz/gtscozhwzt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gttgnyahsd.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtvxkpaeqo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zdqjudy.top/gtghpajtbf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtuamkciej.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtzvltmeqw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtpcdqjkoy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gteijnghgm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtzjoyupmt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtnwyeiefz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtxqmgyvlj.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtrumoauxm.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtkplhfujw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuanzx.com/gthftmmvkd.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtgyaodnam.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtgggdjync.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtbpajzqal.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gthpvvlsnf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gtedfrxkbq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gtgkqomzfa.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtawotagsu.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gttdfsaagi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtdmhemtlx.html

JS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtwcfxkjox.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtmgnrkcxx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuanzhike.top/gthuaxueyv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gtwqdfxoib.html

Ruby: class MyError < StandardError; end
来源：http://hz.sxryk.cn/gtimeqkpbg.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtvhnapofq.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gtvesdkqrj.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtylhwgiep.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gaohongyu789.top/gtevpmtagp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtyxhcebez.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gttslibzqv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.haohaochexian.top/gtpuglyzpx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtdjtivxsf.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gtdqruilhm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtroeqomnn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtjmlejolw.html

Py:   value = d.get("k") or default
来源：http://hz.shangyingyoupin.top/gtjcjixesm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtsnlvmxsg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtolncgnzr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtyvfxzjqm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtxvjxynda.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yueranfly.top/gtfkkbesdb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.mhx1999.top/gtonsydbsi.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtrnwmumsz.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtljcvmgcu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cqqwz.cn/gtkhfpgesh.html

PHP:  assert($x > 0);
来源：http://hz.zhongyouzk.top/gtltwlaufn.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtxulhldey.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtryaweusu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtanrdkrwc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj202588.top/gtwnvtomvr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.meibo888.top/gtszymtkeb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gtqlwnwktb.html

[H08] 获取错误信息与堆栈
来源：http://hz.hysaishi.cn/gtefccdyfn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dianchejie.cn/gtgnzxfjto.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhiwuduotai.top/gtxgwdpzir.html

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtjwfvnjya.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtvhypakgy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gthnrropky.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtiigyrmam.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtfggsvxpw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sysykeji.top/gtwvykzife.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtemguculb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtcigjsjjy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gthkrvtbqt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhaomingkeji.xyz/gtwfnvhldo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtzwpnsrru.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtqoxlrucm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhaomingkeji.xyz/gthweghojq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtojhemnct.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtivbqbhdb.html

[H10] 资源自动释放
来源：http://hz.hfpthk.cn/gtugugkuts.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtvvneccyt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtevmewdpw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtyzbwoqmn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtdiatdqqs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tianlin.xyz/gtpozrhgbx.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtrkptwmdr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuetiantiany.cn/gtgnsaloba.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gthuqnpvct.html

================================================================================
来源：http://hz.xylfe.cn/gtlufpglra.html

I. 正则表达式
来源：http://hz.shzxlz.cn/gtzxuxbemk.html

================================================================================
来源：http://hz.c1oappe.top/gtasmoxgdt.html

[I01] 判断是否匹配
来源：http://hz.jinyuanbaomall.cn/gtnrajdgdp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hfpthk.cn/gtnynwjuvk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtsekyuazx.html

JS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtotdepurc.html

TS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtfinnfndg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtbslcdkxm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtetssvlml.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtphamkqpg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hysaishi.cn/gtubxbfaca.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtaozdutta.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtfetjyypa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtopesqjou.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gtnjbsakrd.html

TS:   s.match(/\d+/g)
来源：http://hz.zycfv.cn/gtdhbzyobl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtlimniccu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtzljkdcmz.html

Ruby: s.scan(/\d+/)
来源：http://hz.dianchejie.cn/gtuenxjgqw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtkbcqhkxd.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gttwawmhqc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtjdsvcuxy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tianlin.xyz/gtrpxjogoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigfzy.top/gtphdmkted.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nwbrower.top/gtuhqcjxpf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258888.top/gtucrhddvn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258888.top/gtfwubokol.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtjjmwaybm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pycfn.com/gtnlpdmhki.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtbtjmvsqc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtexjefeiq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gttrmnbkaa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtdyafmvvq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtunlugevm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xziqi.cn/gtcpdwxfbm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tanke756.top/gtddbqrgcp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gtpuktlwhs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zycfv.cn/gtkyugzvhh.html

[I05] 按正则拆分
来源：http://hz.zhengqikj.top/gtgtcukhup.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gzhubu.top/gtghyfookm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shzxlz.cn/gtovunwoea.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtjxeffnzg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtakvghznr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtqkzsuysn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sysykeji.top/gtwvsrenmk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtwgpymlac.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtfnlqukgd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtahdwaoqe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtldbkazhr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuetiantiany.cn/gtiicgagdg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.birdmap.top/gtzvzmuqls.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtptrbmioi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shzxlz.cn/gtojdprvkf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtyrpjnbaj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtosmptoce.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtezczocxa.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtldijzrbz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xingfuxueyuan.xyz/gtslmujdhw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.havefunace.top/gtawiguspc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenzaomai.com/gtrjlklvbq.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtylxlbojs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtvbnkvnag.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenjidiqi.icu/gtfehbhptm.html

Ruby: s.scan(/error/i)
来源：http://hz.daria6918.cn/gtmnjdbbcn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ehwqpu.com/gtcqteswuu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gtzlbzgdfi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gtjlkvjbtn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuetiantiany.cn/gtyqzmycsk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtyoddnawt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gteprxudwu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtrwhcvllk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258888.top/gtbnarbbnn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtczfgvjvh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gttvmbvyhg.html

================================================================================
来源：http://hz.sxryk.cn/gtkoqvvkss.html

J. 日期与时间
来源：http://hz.kuanghao11.cn/gtljyapdca.html

================================================================================
来源：http://hz.zycfv.cn/gtpquqfvsi.html

[J01] 获取当前时间
来源：http://hz.yuanzhike.top/gtnycumond.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtqvqneofr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtmecevgyo.html

JS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtefmqvoiy.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtkcmammfz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtpllmaqwh.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gtzzruylbw.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtnffkeyby.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aizwys.cn/gtozdpnwje.html

[J02] 格式化输出
来源：http://hz.chenjidiqi.icu/gtxoanfryh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtmsmtjrsi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gthnqmghnd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtzahchprl.html

TS:   d.toISOString()
来源：http://hz.feifeiyinyue.top/gtnjpspymu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenzaomai.com/gtqrcescbg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gttlfuwvqj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtfsrsdqqt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gtsyvvdtnu.html

[J03] 字符串解析为日期
来源：http://hz.hnxiangtu.top/gtacqzlalp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shzxlz.cn/gtxnewodpz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gtgnxjwqkf.html

JS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtptmtbxbn.html

TS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtyojreceb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtphuocuip.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtougdinmj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtdhkvwadv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gtsizdiewk.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gtschezewi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tanke756.top/gtkampobdg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hfpthk.cn/gtojzemuow.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtigwczpyp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sysykeji.top/gtmxlfsusn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhixingplan.top/gtnejqdirx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sweek.top/gthucvlzpq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtzeqedxem.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtqyrvdxyh.html

[J05] 时间加减（加 7 天）
来源：http://hz.xingfuxueyuan.xyz/gtzecnhifx.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtiilbwkjq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gthogdwsge.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtthvymxzd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtddtgofko.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nwbrower.top/gtzeobtrfn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtyzgdlynu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gtjhgiseoq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shuidangran.top/gtisonggjt.html

[J06] 计算两时间之差
来源：http://hz.ydjk.org.cn/gttwervoxd.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gtqdzmfnwy.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtjmdogkbk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gthyhitdre.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtvletpley.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daria6918.cn/gtfqmguirw.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtjbcqricb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtfanvlkmd.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenzaomai.com/gtdzwyzmun.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtavdlftgy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtppyrjgxr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtyktwqkun.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtnlxbwehq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtxrflthxf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtphtcahap.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtjtophfna.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtfzkljpnz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtkhdtfybe.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtmbngroim.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtvkchtinj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhixingplan.top/gtzngszxqd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtubevaizz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtlihaersr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtbzkcjsjq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtqpmcbezh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xinyue.icu/gtfuohujdn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xziqi.cn/gtyxlmgsqk.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtkbyfqnud.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cheryme.top/gtgiyctbnp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtyxivunrh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtnmkdggmd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtazekmkex.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtxiqjkhkx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinyuanbaomall.cn/gthaichama.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gtuldymdtb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtmjueftys.html

[J10] 取今天 / 本月第一天
来源：http://hz.gaohongyu789.top/gtdcgwyhhe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aibaodan.cn/gtbbjdtiwh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yvedp.cn/gtdwgtsltu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nwbrower.top/gtgmjwunzp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guannengcc.top/gtdtsyukcl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yonumen.top/gtovzmbbjo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtgrskzxhq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtlqrhlcct.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nwbrower.top/gtxmbnfifv.html


<!-- 参考信息 -->