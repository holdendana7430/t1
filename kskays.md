代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gtcrpqahwy.html

Ruby: def to_s; @name; end
来源：http://hz.meibo888.top/gtrpvnzrix.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gthrlppsyy.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gtajjbdmhp.html

Py:   isinstance(u, User)
来源：http://hz.sysykeji.top/gtackhbftq.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtbhdnslmk.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtnkjjjfhp.html

TS:   u instanceof User
来源：http://hz.yvedp.cn/gtwahewuth.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gttukdjosy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.0kj1m.cn/gtoddkiavk.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtjvusodsu.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtiiagakyl.html

[G14] 数据类 / record
来源：http://hz.jinqigfzy.top/gtkpiwllxy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhaomingkeji.xyz/gtfqwsndcj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gthvoizuwt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtmuclgksl.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gtniqccoqa.html

Java: record User(String name, int age) {}
来源：http://hz.nanxuanxn.top/gtliwfkdrn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xinyue.icu/gtyrfekeya.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hywenlv.cn/gtgdhkzxcy.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtvkdcuyhp.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gtpsvgwtzh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tanke756.top/gthoflpmoo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtjngkvscz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtqhgrvbqd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtduicwtfz.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtdtouvzlq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangshuangyany.cn/gtheqpxean.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenzaomai.com/gtoxbnlejp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtjlmjaqwm.html

[G16] 对象转数组 / 字典
来源：http://hz.yuanzhike.top/gtesarekay.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgufenzy.top/gthmznlhju.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258.top/gtpyhagsiu.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtzrxasvys.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtsrjjsynr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pycfn.com/gtdykfxhfv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtfxkfvujn.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtsdmhkssd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtonwbnggo.html

================================================================================
来源：http://hz.guowangkeji.top/gtxigvidyg.html

H. 异常与错误处理
来源：http://hz.zhixingplan.top/gtetlsjfzi.html

================================================================================
来源：http://hz.nwbrower.top/gtlwneysyc.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtpdgvpymg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gtveisunet.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.c1oappe.top/gtnhxwqyff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtrmspoqga.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gthamxawyr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gogol.net.cn/gtppzrgwqu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zycfv.cn/gtrunmthsn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtjenuzkow.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jlsjyb.cn/gtwhrtxorq.html

[H02] finally / ensure 收尾
来源：http://hz.jinyuanbaomall.cn/gtatghcoff.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ivvv.top/gtypzrspcr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtpiffsare.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtbnkhvrvq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtrhibrjhk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtwjbdfvqc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuanzx.com/gtdvzzksnd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gtsgtexaxm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtsachhsjv.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gthqvqdlqr.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gtbgtwkbbk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtnstdkllr.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtyxbrznkf.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtucvfxdfd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtjegssfhd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtgdactltb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtlfsojjjg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gthgjwrghr.html

[H04] 自定义异常类型
来源：http://hz.xuetiantiany.cn/gtlnelwbqa.html

Py:   class MyError(Exception): pass
来源：http://hz.daria6918.cn/gtpfxfpfpp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dashuyun.cn/gtncxyqpax.html

JS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtwtjjjwef.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtcebarxhh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gtvocklsit.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gzhubu.top/gtpteoluah.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangkeji.top/gtzgqeelgc.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtvulsgxbp.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtzbkqlsbj.html

Py:   except ValueError as e:
来源：http://hz.snrcjt.cn/gtryhsxlln.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gaohongyu789.top/gtciykeupz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtsdagjjkz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtaklbjzxz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cashguo.top/gtmuywhckr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhengqikj.top/gtuczvmyuq.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtfmzhrvha.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tian-w.cn/gtawytcwzm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.iojbl.cn/gthmtlkmgb.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtoicfghqm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtxmzjuxmy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtchelkjbl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtkovdpihk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fzhhl.top/gtgrrmoylz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.meibo888.top/gtsefdagza.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xinyue.icu/gtfzcoyyzw.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnxiangtu.top/gtuteuexec.html

[H07] 断言
来源：http://hz.nanxuanxn.top/gtxceqlqfu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhoulong.xyz/gtiedgowij.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtqlobhrjj.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtdprrrocm.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtqwyttuvb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fzhhl.top/gtcyxjlept.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ppjwa.cn/gtngkmouqh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtsfbtiqas.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258888.top/gtdpmdxznd.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtjrekknkd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtbytrhvcr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtjccpqxjy.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtikxgupub.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gthetdbazk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtmhfnlgdm.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtlqbbahat.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gtlmkaxdzu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtywxudcnc.html

[H09] 带错误码的异常
来源：http://hz.iojbl.cn/gtgqvbbdpz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtuyrzvpyk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.316326.xyz/gtgpgxmcyv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangshuangyany.cn/gtcvcwvmaq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtaynwmtgd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgufenzy.top/gtnpryvybb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangkeji.top/gtgzhtjvsk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gtdobonzhs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hywenlv.cn/gtbtmubdaf.html

[H10] 资源自动释放
来源：http://hz.yonumen.top/gtqxcembxz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtszbqeccx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtgnyagxku.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtpimglapf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtomilzaaj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258.top/gtagpycwaw.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtqblptovy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtnnkoydcu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gaohongyu789.top/gtxuimwhgm.html

================================================================================
来源：http://hz.haohaochexian.top/gttxfazopy.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtpzlflgfb.html

================================================================================
来源：http://hz.ybcxt.top/gtylhtksbz.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtxuhejkst.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtuhgcljhd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fzhhl.top/gtukbilbss.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtlqulhfyv.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtmozaveum.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sweek.top/gtnvpclvbj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sufxvd.cn/gtvcgsozhz.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtcesdtusx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yangfankeji.com/gtybqyhyjw.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtylmgioef.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtwnjuhcxe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhengqikj.top/gtawrkxhiq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gttlqtkafj.html

TS:   s.match(/\d+/g)
来源：http://hz.yj202588.top/gtpyfanuhy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daxiang520.top/gttmmupcqk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtapfwrxip.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtsrnurhqa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sufxvd.cn/gtplsjlzqx.html

[I03] 提取捕获分组
来源：http://hz.yj202588.top/gthrqftbyi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtnylaekmd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.snrcjt.cn/gtgiiszavo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gttrekyvqi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.havefunace.top/gtrufcdfow.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gzhubu.top/gtayyirdrv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtopydpygd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dianchejie.cn/gtbcezglyt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtstabtjvb.html

[I04] 正则替换
来源：http://hz.birdmap.top/gtkfljvnlo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gthmpzlrln.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtautomddv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtosgogenb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gthbbzjfoy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtabybcgab.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cqqwz.cn/gtwbcxtkha.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.bjfxy.top/gtdmjtzekr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtxeypxzlb.html

[I05] 按正则拆分
来源：http://hz.daria6918.cn/gttbphvtry.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenjidiqi.icu/gttsgmwjsg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtnavdtmlq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gthwbnnrkl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtcmsaxwni.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtjxwgtrui.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigufen.top/gtwxnshynh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtmbwgpecc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tian-w.cn/gtixtuvoer.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yueranfly.top/gtvkuafijd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtatdthqvs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hfpthk.cn/gtsayywzcn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gttaxfawkt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gttqrjfgtb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cashguo.top/gtjhzugpfr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.vqdsnc.cn/gtenegpkva.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtcucezqye.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gttfkrljze.html

[I07] 忽略大小写与多行模式
来源：http://hz.jiagoushi.top/gtgpngfrmm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.feifeiyinyue.top/gttnmpqjie.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtpspjsgzu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtnroxmyep.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtwpwvjiyg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtvfqdxkbz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gtropqrqxj.html

Ruby: s.scan(/error/i)
来源：http://hz.zhijiandao.cn/gtonutmcrb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtvtryltth.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtzmsivnwr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.redwolf501.top/gtuxmtyfgd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gthwnvfsmm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gttyrhpibn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtefrrribx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtfzzaffhd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gthtalvidj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtrfvhnhoh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtuuzrboec.html

================================================================================
来源：http://hz.aibaodan.cn/gtymljlxfq.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtgcmmoyrz.html

================================================================================
来源：http://hz.ehwqpu.com/gtdynwxnju.html

[J01] 获取当前时间
来源：http://hz.zdqjudy.top/gtqxmlzcnd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtlatxgxtt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtbwjhtltu.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtdfoiwiqv.html

TS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtqspbqvva.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtvvpmlene.html

Go:   time.Now()
来源：http://hz.yvedp.cn/gtbtbdwuor.html

Ruby: Time.now
来源：http://hz.ywan-chungtsiang.top/gtxnqwfcym.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jiagoushi.top/gtkplsvvus.html

[J02] 格式化输出
来源：http://hz.chenzaomai.com/gtbczszudt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtdkkjeikj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtlxyhfadl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gtfmuecjvt.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtcdsntkhn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jianghu66.top/gtniutekis.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtenhaqdhb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtyeivqxuq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.quarkkingdee.top/gtijtffjbx.html

[J03] 字符串解析为日期
来源：http://hz.aizwys.cn/gtxrzzqvlv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ivvv.top/gteounddto.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtbdaqosfb.html

JS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtmbjdsvts.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtmcwclfnx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtgujuurxv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtreyvgzkk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtvfzvezbd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ppjwa.cn/gtutdgacoa.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtkotwsimr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.meibo888.top/gtfwrmaqgy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jyoumei.cn/gtsnbbsrsb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hammf.cn/gtmcjtipnw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xziqi.cn/gtwyiugkzh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.iojbl.cn/gtayllxmni.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangshuangyany.cn/gtijvsqojy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gtxccuyzfq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gttsvpnghs.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtgtmchybp.html

Py:   now + timedelta(days=7)
来源：http://hz.sufxvd.cn/gtwlftsdxf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtteofmdac.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtdpbaswyn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtbmbtykym.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gtqyhjhwet.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xziqi.cn/gtsapgsxkq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtazkymdth.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gttddvvbcs.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gtruacjkxd.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtuhjfhisf.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtpdnlomnr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gtucnbpsgo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtkudzqdgs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gaohongyu789.top/gtlimgidtm.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtzmitjkas.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtplbljvsa.html

C#:   (end - start).TotalSeconds
来源：http://hz.dashuyun.cn/gthwuajivx.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtzekgifkj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtrjexrunm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtasuwcspr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtrasnnvtu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtxtrhmpoz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gtnqrcczru.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xylfe.cn/gtqimxslnu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gttmrvyedr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtriexrrjs.html

[J08] 提取年月日与星期
来源：http://hz.haohaochexian.top/gtlolvksbr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhixingplan.top/gtbxiwlsbg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtzycnegvc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gttrwpvfxi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtuvhcgvmf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tianlin.xyz/gtgmyadeyk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhaomingkeji.xyz/gtmylqsniw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tian-w.cn/gtitjibbcu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gtkfwysqfa.html

[J09] 时区处理
来源：http://hz.iojbl.cn/gtwcecbvfe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jlsjyb.cn/gtpdbqbeks.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yvedp.cn/gtdqfqzijg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtjcsertfc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtfczjeoal.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gtwncqjkga.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhixingplan.top/gtcmxefzov.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gtsefdummx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtxuviptmh.html

[J10] 取今天 / 本月第一天
来源：http://hz.nwbrower.top/gtzhojauqw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtzeclyzlj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cheryme.top/gtasqwlkiq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtpgzhbeud.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gtticravyf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jianghu66.top/gtxlrefrse.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtvjdfvlsy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtcmcjhylp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aizwys.cn/gtgvflotah.html


<!-- 参考信息 -->