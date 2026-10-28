代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtrqbnhpzx.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtphyncneo.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtwapdedsb.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtxpcfukom.html

Java: u instanceof User
来源：http://hz.xylfe.cn/gtcnvhiubj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gotoacloud.top/gteahnzswm.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gtbcfprtln.html

C#:   u is User
来源：http://hz.jinqigfzy.top/gtfysanpgc.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtytoihgiq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yanxiufei.cn/gtowyfsqqk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtpdcktgxc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtefwgtgai.html

TS:   type User = { name: string; age: number };
来源：http://hz.gogol.net.cn/gtgaslszma.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtplmcryzq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shuidangran.top/gttjzrfvvc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtwbepszqy.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtfyojknjp.html

[G15] 枚举
来源：http://hz.cdnleiting.top/gtdufdoduu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cqqwz.cn/gtndukpcqz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gtgioninri.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtglgluiif.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtipxdwkvx.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gthbgbjame.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtnkqwnrcu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.52xcode.cn/gtjybwzfvv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gthxboldvd.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtvppccegd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sysykeji.top/gtvyzaoouk.html

PHP:  get_object_vars($obj);
来源：http://hz.birdmap.top/gtmiuexikl.html

JS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gthgxntser.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtpsielvrw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtkzdciqdi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hywenlv.cn/gtqjcmbwrk.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gtovfvgste.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtpgopuofg.html

================================================================================
来源：http://hz.yj20258888.top/gtjnmnaudz.html

H. 异常与错误处理
来源：http://hz.ydjk.org.cn/gtnuattpdy.html

================================================================================
来源：http://hz.316326.xyz/gtuoaqzxsr.html

[H01] try / catch 基础
来源：http://hz.bjfxy.top/gtjnzrlzdl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gtcvyeykip.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtofgedelq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtuhzpwyed.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sufxvd.cn/gtcnqprkqf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.andypj.xyz/gtepvzyazl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtveygyqey.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhongyouzk.top/gticrfmkmx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtnzpgjnze.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gthgzpajzt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtebdndhkc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtynmerroo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtudffncwl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtmsjlljqd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtuiizzqvr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtywextrro.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtoraxorbi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yongpay.top/gtparjytmo.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangkeji.top/gtxroziezn.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhijiandao.cn/gtuutjshib.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtaeatnnuy.html

JS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtkjikcmnb.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtbnjztqxt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gttsrzjena.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxinkj.top/gtzbggpuul.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtpdjoekii.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.havefunace.top/gtqucnomru.html

[H04] 自定义异常类型
来源：http://hz.tanke756.top/gthqozlloa.html

Py:   class MyError(Exception): pass
来源：http://hz.hnqzz.top/gtaeirbbml.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yvedp.cn/gtnnfdexlg.html

JS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtntihgcap.html

TS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtzpvukvzk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtyjmscgam.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtgcczbvlj.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtsocfjest.html

C#:   class MyException : Exception {}
来源：http://hz.smart0.xyz/gtbdwflfzf.html

[H05] 捕获特定类型
来源：http://hz.cdnleiting.top/gtvxwxzyep.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtdjiyuzcz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtnhdlowdl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtydtgovzm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtoakehjff.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtlmojqxui.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gthllqquhl.html

Ruby: rescue ArgumentError => e
来源：http://hz.hywenlv.cn/gtxzirziyp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.9152youxi.cn/gtwkhfhioo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhoulong.xyz/gtzirwvapi.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtsrnitbpf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258888.top/gtzeijpopt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtdvbirogz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtmdpyojhy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gteddecpme.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gogol.net.cn/gtspolbyhf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guannengcc.top/gtljlfowyk.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtmezbubdp.html

[H07] 断言
来源：http://hz.daxiang520.top/gtzbqdcyev.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtnlsaayzf.html

PHP:  assert($x > 0);
来源：http://hz.yj202588.top/gtznqipbdi.html

JS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtrqgnbidp.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtetomzaga.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtzvbavudj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtaylkrzkq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cdnleiting.top/gtfnnyfsck.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtxayfojgx.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtmorbsycr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtdqadwvza.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhoulong.xyz/gtekhbfcys.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gtbibnahgh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gtswxnagvc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtnvfquxaq.html

Go:   err.Error()
来源：http://hz.316326.xyz/gtfusrbcgd.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuanzhike.top/gtksjztcyl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gtzajfqcrp.html

[H09] 带错误码的异常
来源：http://hz.birdmap.top/gtuzzpaxmk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cdnleiting.top/gtimcldjwx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtxinegppv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtakamsfxk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtqwlhuyci.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtetvwzyja.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ybcxt.top/gtbvcesesq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtqsqxlnhr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtreptbhes.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtaepsvgkn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtzzjotcdg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtknizvhju.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtdrdtgxrw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtilvrpnaa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.9152youxi.cn/gtgazxkyli.html

Go:   defer f.Close()
来源：http://hz.jlsjyb.cn/gtzmkgjrsx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtylhybvrc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cucudq.cn/gtbvwwnaxe.html

================================================================================
来源：http://hz.tian-w.cn/gtsrkegcco.html

I. 正则表达式
来源：http://hz.zhijiandao.cn/gtsfrvbiwg.html

================================================================================
来源：http://hz.guowangkeji.top/gtutitbolt.html

[I01] 判断是否匹配
来源：http://hz.andypj.xyz/gtxcltzmnk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtxkxudjxv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.316326.xyz/gtppgsqtgf.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtndavqtoz.html

TS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtiehpgygb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtpxzeeswf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenlongwang.top/gtwghbjwmd.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtuymabkvj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cashguo.top/gtaiqbglqp.html

[I02] 提取所有匹配
来源：http://hz.cheryme.top/gtpbzmyhjj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtzzctlhxy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gaohongyu789.top/gtehznkxil.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtducjdvud.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gtzecadjmi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jianghu66.top/gtdombbecx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gtunxnjglh.html

Ruby: s.scan(/\d+/)
来源：http://hz.iojbl.cn/gtffiimlvq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xziqi.cn/gtjkgwzxql.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtpfdzsdac.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtfwxetjtg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gzhubu.top/gtwkaxzvap.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtsusrtrgg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtbumpajia.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtqolwpzhv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tianlin.xyz/gttczmvard.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cqqwz.cn/gtrbxwdnux.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.vqdsnc.cn/gthpugeprk.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtdzgkipwk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtzxupqbrp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtbqxhnyti.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtdtojjhvw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtaqxmcnif.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gtarsajlpd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtepssomtl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gtqusceayj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtgiuiohjc.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtloitjeyf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtbfrxwnha.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtxatgptfu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtmqcrmwpm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtwzukxcgd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtcclitcmh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gtrojzdnzs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtgestrpbf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtakgbbqmt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtsaxibpmz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gthmrfxckw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xziqi.cn/gtcctqbcuu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtplgbozdq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtwiodgbkp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.kuanghao11.cn/gtcjzzlwxb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigufen.top/gtgelykbkh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gtlumgiwyo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtbvmvjunm.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenjidiqi.icu/gtwdiljbgz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.bjfxy.top/gtwiwysdgs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtoatrjozq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtucwebbzj.html

TS:   /error/gim
来源：http://hz.nanxuanxn.top/gtuyvcnnct.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtfonqnpzm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinghuilouyu.cn/gtbrzlggrk.html

Ruby: s.scan(/error/i)
来源：http://hz.chenlongwang.top/gthqgnrkdk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtknkohokl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shangyingyoupin.top/gtszqqkmtx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtulbylkse.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtcbunfoak.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtbywhoxjd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtjdwvplcr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtfqvabcqq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtjargyvym.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zdqjudy.top/gtzxzqrrvm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtjtpogngu.html

================================================================================
来源：http://hz.mhx1999.top/gtfpmbtpzs.html

J. 日期与时间
来源：http://hz.meibo888.top/gtrxgebdae.html

================================================================================
来源：http://hz.gaohongyu789.top/gtorzuedfb.html

[J01] 获取当前时间
来源：http://hz.zdqjudy.top/gtcoglfqog.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gtnxwipmwe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtharrbild.html

JS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtpbhdtaku.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtffmewgge.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gtxnoisufu.html

Go:   time.Now()
来源：http://hz.xuetiantiany.cn/gtpkjefibx.html

Ruby: Time.now
来源：http://hz.hfpthk.cn/gtwwurripj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtikaqoexp.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtawwvdrcl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtzuxuxmur.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtcxsgzhfo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sweek.top/gtilaqxejv.html

TS:   d.toISOString()
来源：http://hz.guannengcc.top/gthfunnuif.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnqzz.top/gtuhctnrid.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtuxohyuhg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtjiuctzbh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtkzvdyxui.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtfnfnfogx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gthtptpbmu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yvedp.cn/gtkdmudbhk.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtfylyvezu.html

TS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtlovydair.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtiguzkxie.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtjbwcziqm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtgvvazqcr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guannengcc.top/gtzuveqzvl.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtrjxuzsix.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtknekwdot.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtviedzyvx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gtpmqmgfnv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fengsongda.top/gtyiilmwfx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtbqpxtoek.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xinyue.icu/gtcobszhqn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtxapghvqt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtwkakedib.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtjhaxsjyk.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gtznaekhlc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtrocgtphg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtjnpziram.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtjqufzphy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gtxfmmerwz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fzhhl.top/gtghcfklpf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtsitobmhj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtmbqlacrq.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gtmsgucfzo.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigufen.top/gtqsihrxyf.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtvekehfyn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cheryme.top/gtggsijken.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtubtbkndo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.feifeiyinyue.top/gthrdmemso.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtmcvqiofm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dianchejie.cn/gtxzukwngx.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtdwuidfyy.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtavkojnus.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gthggzcefy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtndwwgteq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtomiwyeuj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtgivzivhb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj202588.top/gtgurgvtfq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tian-w.cn/gtqxsfrbjj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gthepjbptp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gttupfhgil.html

[J08] 提取年月日与星期
来源：http://hz.ehwqpu.com/gtvklumbsm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.9152youxi.cn/gtkqqlcmjh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtxyjhulzy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtskliljis.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pengpengdd.cyou/gtgcxytwjt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtmtgdiank.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gthknpjhev.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuanzx.com/gtfttakxli.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ybcxt.top/gtkdfbznzm.html

[J09] 时区处理
来源：http://hz.pycfn.com/gtolrvmdoa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtmoulgwlv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daria6918.cn/gtibjhwhfl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtifpdeffz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtzktqjffs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shzxlz.cn/gtrckfgrnr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gtzmmwjjbh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtstrvtvpf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangshuangyany.cn/gtlvbbriab.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtuewqoezn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtwnxvdtih.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.havefunace.top/gthbnpwaxo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xinyue.icu/gtribifgot.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtehycabot.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gotoacloud.top/gtavahbraz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtgrimwasx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gtxqiuzqrc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtvbypklsr.html

================================================================================
来源：http://hz.tian-w.cn/gtcrwwfxqw.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtnknlappu.html

================================================================================
来源：http://hz.shuidangran.top/gtugnqbrrj.html

[K01] 对象转 JSON 字符串
来源：http://hz.zdqjudy.top/gtbmgggkcw.html


<!-- 参考信息 -->