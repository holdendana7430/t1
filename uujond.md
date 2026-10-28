代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtgvcvohxa.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtmlpabvey.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtuvhkiyzb.html

[G13] 判断对象类型
来源：http://hz.jinghuilouyu.cn/gtyowzyznn.html

Py:   isinstance(u, User)
来源：http://hz.iojbl.cn/gtkzatzhns.html

PHP:  $u instanceof User
来源：http://hz.dashuyun.cn/gtxwdzmtmc.html

JS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtkzuyqsph.html

TS:   u instanceof User
来源：http://hz.guannengcc.top/gthdoazgix.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtrvgmiwie.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.quarkkingdee.top/gtecyqoton.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtgfxxvjex.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtqnbjvpzv.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtzwshfmol.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtdarqpujd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guannengcc.top/gtxngctdes.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtnunkujbh.html

TS:   type User = { name: string; age: number };
来源：http://hz.meibo888.top/gtqulqpeem.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gttndbdjba.html

Go:   type User struct { Name string; Age int }
来源：http://hz.vqdsnc.cn/gtjjefmeqo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gogol.net.cn/gtjfdporpi.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gttuhgouub.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtpajsildy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtgjhfpfrs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pycfn.com/gtpwdnpzxd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigufen.top/gtwfjazmva.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtpzkccyhs.html

Java: enum Color { RED, GREEN }
来源：http://hz.aibaodan.cn/gtaiivjnfo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daxiang520.top/gtlaedtgoi.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtaooleuwb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gthyxjtuho.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtykswliit.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ppjwa.cn/gtqnhzxgia.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gtxuyzezki.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtnzzlnkxz.html

TS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtrnlwyayg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shuidangran.top/gttxzlokbo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gtjwkevxwi.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtvokkkgyp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtbfjqsrle.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjcxgneim.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtufqywkoh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvrpcxmzq.html

[H01] try / catch 基础
来源：http://hz.guowangkeji.top/gtwyeoemft.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gteybndegn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtjinzewos.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtzgrvhopl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtfnodohme.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtkpowrtvq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgfzy.top/gtncwkqsfx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtmyemzeiq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guannengcc.top/gtavztftbs.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangkeji.top/gtxrzeqqcr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigufen.top/gttqqpfyod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtdusecgak.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtqtxulbdb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtbtctoqey.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtdehfqgis.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gtdcgvcpmc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtulfmrjoa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shangyingyoupin.top/gtuncqbzis.html

[H03] 主动抛出异常
来源：http://hz.gogol.net.cn/gttqdvpcqg.html

Py:   raise ValueError("错误信息")
来源：http://hz.vqdsnc.cn/gtncqumfks.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gttuhesxxy.html

JS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtclgyskxo.html

TS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtoepcmlaf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtkxgyjwjd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guowangkeji.top/gtmjvjopoa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fzhhl.top/gtupuaeday.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtttdgvgmb.html

[H04] 自定义异常类型
来源：http://hz.yuxming.cn/gtenuntvdv.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtocbzmljc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtgomvmlvk.html

JS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtvkkimkms.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtvryivhka.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtyfyhcaau.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtctfnszfz.html

Ruby: class MyError < StandardError; end
来源：http://hz.tian-w.cn/gtfdlbynms.html

C#:   class MyException : Exception {}
来源：http://hz.kuanghao11.cn/gtojkuudll.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtqtvmbzdg.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtanzjrnvt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.0kj1m.cn/gtxnvpvtnw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtbhxebdli.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtvbwnbwgq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zdqjudy.top/gttxondhra.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtbnmdikzb.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhoulong.xyz/gtojtdgqfe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gttylycglw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtuxcwbjzt.html

Py:   value = d.get("k") or default
来源：http://hz.pycfn.com/gtfkhlzvra.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtpodyhefx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtbhuydbfa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtiwfrdaqo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.0kj1m.cn/gtvjrkemdz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.vqdsnc.cn/gtwirwmaab.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yonumen.top/gtivzyeocm.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtnbtcvgyd.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtpfavinzp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtoqkeaqbn.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtyhfdxcgw.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtwqarajzm.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtaphcnjkg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gtbqhrcjth.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gtwmdgdmkr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhongyouzk.top/gthziswxpm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtzuszbgvx.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangdashe.top/gtjpfkasue.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.52xcode.cn/gteequavxm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtyxiusbvg.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtatemgofp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtyapgjlet.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtafvdsopf.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gtvyqfkoax.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigfzy.top/gtxjdkjtgz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cheryme.top/gtmhttpvhx.html

[H09] 带错误码的异常
来源：http://hz.bjfxy.top/gtoaogyiws.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jyoumei.cn/gtanlhleed.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.svipenyu.cn/gtnlrhejoy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtwbipnrwp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nwbrower.top/gtwtekzrhp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgufenzy.top/gtahtmuttc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zycfv.cn/gtqjxxitoa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.mhx1999.top/gtoiamqsff.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yvedp.cn/gtospocree.html

[H10] 资源自动释放
来源：http://hz.tanke756.top/gtvvnqhspy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.quarkkingdee.top/gtxyurvubc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hysaishi.cn/gtjkdcvnjs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gthwzbdndc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtpvlcvyqp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtezgvaltg.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtpvndaewj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.bjfxy.top/gtiyzonfym.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xziqi.cn/gtqkbnbmes.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbqprkygh.html

I. 正则表达式
来源：http://hz.shzxlz.cn/gtcohihrxa.html

================================================================================
来源：http://hz.jyoumei.cn/gtlbiipwsw.html

[I01] 判断是否匹配
来源：http://hz.hfpthk.cn/gtwiytxupt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daxiang520.top/gtxfxevnff.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtotavfwdv.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtnloodatf.html

TS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtifbditfb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtxdadltph.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtnsgkghzd.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtkjidcbip.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtplctdbjh.html

[I02] 提取所有匹配
来源：http://hz.hammf.cn/gtrrozwjeh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtswmczxxz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtsjhtjfcr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.smart0.xyz/gtsdkdazmg.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtjusglfzi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tianlin.xyz/gtqgczkzzj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.aibaodan.cn/gtlbcehruu.html

Ruby: s.scan(/\d+/)
来源：http://hz.birdmap.top/gtkzuezdyd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtlbiqfrmm.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtswtcovqs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fengsongda.top/gtvshnyodu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtjbaodwer.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hammf.cn/gtwhjxbhvh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xingfuxueyuan.xyz/gthsjembjd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtdblikbcr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gtuqlypdvv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtbalxtaay.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtzwsqfesy.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtgwizkepk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shuidangran.top/gtxwhykolk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xingfuxueyuan.xyz/gttcizwxbk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtuuepmsuz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtprzdngkx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aizwys.cn/gttskbsfkf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yangfankeji.com/gtrrigpgbh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.316326.xyz/gtkcjgambo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gtczecmmlb.html

[I05] 按正则拆分
来源：http://hz.gotoacloud.top/gtolibnmap.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dianchejie.cn/gtgiebicvp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtmivdevtk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gttulugxsi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtealemgnn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ivvv.top/gtoxaswhrh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtmkoxxacx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtnhhwzunj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gttuijgzmt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhixingplan.top/gtrsexfdgr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtgtcfjuiv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shangyingyoupin.top/gtdyfpfsob.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtalheoluy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtvhfhmzuo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtcnxdsevj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtiukjrewf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtnqqxmqlb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gttrjeylgd.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gttbyfglgg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gaohongyu789.top/gtsqgbnirw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.svipenyu.cn/gtolglkgup.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtsakaboci.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gttlnekomu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtctkbnjfy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.svipenyu.cn/gtmdktncty.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gtrgmqfttb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtlkbkbkje.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.iojbl.cn/gtldkaucfy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gtcibzuonm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtlifrshzc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtadcibdzu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtssulnuio.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtydjkhydq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtbmoijejg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtohzlmkia.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtfxoksqxf.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtclxitcsx.html

J. 日期与时间
来源：http://hz.pycfn.com/gtijhxmxxb.html

================================================================================
来源：http://hz.pycfn.com/gtibnzuebw.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtfdeniojc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtntjphsim.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtqtighuae.html

JS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtdwwoflsw.html

TS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtnfgmuuua.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtfludbyhj.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gtzefyqagt.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtcammbywy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuanzx.com/gtcqaldzry.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtjebyfpvl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtsytqkytp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gthkhtvucb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shuidangran.top/gtkghnknao.html

TS:   d.toISOString()
来源：http://hz.0kj1m.cn/gtrvgxeyjq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ppjwa.cn/gtxqzorjzo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtazivajsb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtlguvmbej.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtyafmvqsz.html

[J03] 字符串解析为日期
来源：http://hz.iojbl.cn/gtovoyijas.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangdashe.top/gtoemngjyg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtdvahljpo.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtyjslrtzw.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtladlptvd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtofeqedwy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtsawwdqgc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gthdqbslwl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigufen.top/gtziiekydb.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtotesqqwg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtpwqwphqn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gtcietkfcd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shzxlz.cn/gtoovizgww.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtiyimyniy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gtlssyejsx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ppjwa.cn/gtpkxzlmsp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jianghu66.top/gtzdnsndiw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtbfmosozp.html

[J05] 时间加减（加 7 天）
来源：http://hz.tanke756.top/gtnycamzpw.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtdrjijyoe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shzxlz.cn/gtlwfwiwre.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtdnkxssfc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtezcmcguc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtujdtbaql.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gtsfdqnhxp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtnekfpypm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sxryk.cn/gtoesabubi.html

[J06] 计算两时间之差
来源：http://hz.zycfv.cn/gtolsfgbdi.html

Py:   (end - start).total_seconds()
来源：http://hz.gaohongyu789.top/gtmodoxmag.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtbtsxwxnw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sufxvd.cn/gtxowdyfie.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gaohongyu789.top/gtsuyvhywa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgufenzy.top/gtfjvmkfwk.html

Go:   end.Sub(start).Hours()
来源：http://hz.316326.xyz/gtxsxnwxns.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gtinafyhfu.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtihyyzkfa.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtbwwwwjut.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtljgzbrzh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gtwrsavysn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gteuudwruu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtlsudxswg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtpalstchk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtzzoybssy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gthyzlgxwg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gthoywjklz.html

[J08] 提取年月日与星期
来源：http://hz.daxiang520.top/gtdknbwwcn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ppjwa.cn/gtbqjcemmx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gthboyvsnt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtmibiofku.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtgidfhcms.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtpmettaki.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gtritjyysz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtehcaqjxr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gtppbligtd.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtciotnonx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yonumen.top/gtnfnbsile.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuxming.cn/gtlaycnauw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtuasazuyt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gternhflki.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtpshnmhjj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.meibo888.top/gtuzickkrt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtdjqlsxkg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtszdgozyq.html

[J10] 取今天 / 本月第一天
来源：http://hz.iojbl.cn/gtqduphtiz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guannengcc.top/gtmtarijuj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gtquaksgcc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.mhx1999.top/gtnddmdeny.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydjk.org.cn/gtqvtegjlv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtjrixhcwh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtumpqzidn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtrljezrae.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxuanxn.top/gtzlmsjbgr.html


<!-- 参考信息 -->