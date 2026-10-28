代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.zhoulong.xyz/gteeksfokk.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtmbirjfsl.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtlaliczac.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guannengcc.top/gtrsexozcq.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtyeriuvvt.html

C#:   public string Name { get; set; }
来源：http://hz.cashguo.top/gtnatxridy.html

[G12] 对象转字符串
来源：http://hz.zhiwuduotai.top/gtiusklgrz.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtlfmnjnnd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtdjnqgjzq.html

JS:   toString() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtweffmiry.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtnvnjdjux.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtyeqdqxkg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtmzecvser.html

Ruby: def to_s; @name; end
来源：http://hz.xuetiantiany.cn/gtohqdwwyo.html

C#:   public override string ToString() => Name;
来源：http://hz.ybcxt.top/gtybexidjv.html

[G13] 判断对象类型
来源：http://hz.jianghu66.top/gttmqpnbwu.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtjnmpolbu.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtxfopqzno.html

JS:   u instanceof User
来源：http://hz.xinyue.icu/gtvachxxfr.html

TS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtmvqpxyal.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtayqbpvzv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cashguo.top/gtbmdtixkz.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtomtvfoxv.html

C#:   u is User
来源：http://hz.nanxuanxn.top/gtsajzuhfc.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtesqynbnq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtunjaznol.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gaohongyu789.top/gtrkjsoxvn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gtbvbwcfpm.html

TS:   type User = { name: string; age: number };
来源：http://hz.ybcxt.top/gtxikskdcx.html

Java: record User(String name, int age) {}
来源：http://hz.ehwqpu.com/gtukfaggkf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.smart0.xyz/gtmhnreqtt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtdqbqbpzk.html

C#:   record User(string Name, int Age);
来源：http://hz.jiagoushi.top/gtnprrslax.html

[G15] 枚举
来源：http://hz.ybcxt.top/gtzscdpvcw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtgpegqeae.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuxming.cn/gtjswrhrgi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cucudq.cn/gtffimnumf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtxiskwfyd.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtarakvhkt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtdyaucpbb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gaohongyu789.top/gteqsxacue.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtnqshyuhy.html

[G16] 对象转数组 / 字典
来源：http://hz.jiagoushi.top/gtuwcqtaus.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yanxiufei.cn/gtkndjycll.html

PHP:  get_object_vars($obj);
来源：http://hz.shangyingyoupin.top/gthjxuvasr.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtmenynpay.html

TS:   Object.entries(obj)
来源：http://hz.shuidangran.top/gthcopobma.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtqcaasiwd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jiagoushi.top/gtgtzofizn.html

Ruby: obj.instance_variables
来源：http://hz.pycfn.com/gtdhmkxjoj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtdigxmeyo.html

================================================================================
来源：http://hz.jinqigfzy.top/gtubalybsz.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtulrsrujx.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlwujbelu.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtqtcoddpi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gtjhokhtya.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shuidangran.top/gtnzkjcjta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtrthksnbc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtsrwnzcvj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenlongwang.top/gtpzwoiljc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gtvrlespwd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zycfv.cn/gtddgymcfv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dianchejie.cn/gtspmxmmuk.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtfmhbbsgx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtswwblbzy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtvocwevzz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtxqtvusdb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtdrmutdde.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtxlbwjnqv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shzxlz.cn/gtwgipecig.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gzhubu.top/gtzprglcfs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.havefunace.top/gteccfyrrx.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtzbisfrlx.html

Py:   raise ValueError("错误信息")
来源：http://hz.havefunace.top/gtydcdlrfj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtkenxfnbw.html

JS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtjtojupgk.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtjweodvvb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtbgruwfpl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gthbodvafw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.andypj.xyz/gtbtnkdnmx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtrdhfgnyu.html

[H04] 自定义异常类型
来源：http://hz.tian-w.cn/gtyguxnkpx.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtgujxgxdh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gttnxzvwft.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtxeawuqlu.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtrnzxlhez.html

Java: class MyException extends RuntimeException {}
来源：http://hz.iojbl.cn/gtvsogcjhc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gthzexoyhp.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gthlphfiwi.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtwxsrbbrw.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtajhwdlmm.html

Py:   except ValueError as e:
来源：http://hz.zhengqikj.top/gtkicsyqji.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gtmcerkkmq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtsqbzarxk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtitlqehdy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.haohaochexian.top/gtspmuyaic.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtchqycwfg.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhengqikj.top/gtgclhocdv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.0kj1m.cn/gtzzewmmzg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtzotdxvrk.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtbefcoqjt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtinjlgtry.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtidvstlsz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtwnvghegq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtpiwkljck.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gtfjrmkceo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ywan-chungtsiang.top/gtivvqgzcv.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtkvpqesrw.html

[H07] 断言
来源：http://hz.cashguo.top/gtxfckevyo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.mhx1999.top/gtwntahdlr.html

PHP:  assert($x > 0);
来源：http://hz.iojbl.cn/gtmetkghgz.html

JS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gthftuhgqr.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtiynntreg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtqhqeyusu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gtjttnapaz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shangyingyoupin.top/gtmwcmlrll.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xylfe.cn/gtmwfjbarv.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangdashe.top/gtygnbygxk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinghuilouyu.cn/gtljxpediv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtczwnsfup.html

JS:   e.message;  e.stack
来源：http://hz.hfpthk.cn/gtbejhznhy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yanxiufei.cn/gtwfknyuut.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtemcwnnyx.html

Go:   err.Error()
来源：http://hz.hnxiangtu.top/gtxrgsrgql.html

Ruby: e.message;  e.backtrace
来源：http://hz.meibo888.top/gtxbojdioz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtrqzvvbpu.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtikqaaope.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hongshengwenyu.top/gthtmvzkqi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtkxuduuby.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtueteyyxl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gtfvarcrzw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtpxrmxqth.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtlqxtgfzb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinyuanbaomall.cn/gtqxnaymde.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gtabtjgtdn.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gtihhfaszx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtxoriagcv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtgvmsjvku.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtoubvkcpj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtykxireov.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nwbrower.top/gtvsxvufir.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtpwxeuoyr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtlqgrmxlb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yongpay.top/gtmbqquabr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtyybykago.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtpbqjtkvt.html

================================================================================
来源：http://hz.cucudq.cn/gtpndluczt.html

[I01] 判断是否匹配
来源：http://hz.snrcjt.cn/gtubauoelw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.mhx1999.top/gtlxezrese.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.c1oappe.top/gtgzzumaiq.html

JS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtiuxgmgha.html

TS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtesdmcxry.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.kuanghao11.cn/gtskhplcoh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hywenlv.cn/gtniuyssak.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhengqikj.top/gtmirfaehg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hysaishi.cn/gtfekeztrf.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtlkxiwfzr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhengqikj.top/gtaclyikvw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangtech.top/gtaqtabntt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtiidhdwxp.html

TS:   s.match(/\d+/g)
来源：http://hz.gzhubu.top/gtggpgwbse.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gthracjehv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sxryk.cn/gtcjlncrix.html

Ruby: s.scan(/\d+/)
来源：http://hz.yongpay.top/gtssoczjyk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj202588.top/gtjjzoilkv.html

[I03] 提取捕获分组
来源：http://hz.xinyue.icu/gtqydnjjft.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtihhkmrea.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtsaowucbd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gteuwsakyj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pengpengdd.cyou/gtovjbpbjt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtfgpdxcbe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtcelrylvu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtduuksrfn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xingfuxueyuan.xyz/gtguhbgbkz.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtkundbnfo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fzhhl.top/gtljisdipn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtvfkkgyxk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtyeoaxvus.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtegxjogxa.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtermrhzgm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnxiangtu.top/gtfwdpoyke.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtzljploxd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtcamvlswu.html

[I05] 按正则拆分
来源：http://hz.daria6918.cn/gtdepaefrz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gtvwoaidar.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xylfe.cn/gtnyyqphbm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtugjpwsen.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtkonliyne.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtnpovbjgt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtvqzzhltv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtwxbuzjrc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtaqbnpzxv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangkeji.top/gtmagholom.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtimiqoijp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yueranfly.top/gtwtjkbatc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtzkdypugz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gthqlzkkix.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtiuxstalx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtypslnhwr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtqdhtxkez.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtmkoaeofh.html

[I07] 忽略大小写与多行模式
来源：http://hz.guowangkeji.top/gtvuocbnyx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hfpthk.cn/gtbumcmgsr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258888.top/gtlmocllaz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtzdsddgxu.html

TS:   /error/gim
来源：http://hz.sysykeji.top/gtxipbrowx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daria6918.cn/gtuxksgpda.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.quarkkingdee.top/gtnaczpajk.html

Ruby: s.scan(/error/i)
来源：http://hz.chenjidiqi.icu/gteocxcits.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jyoumei.cn/gtysrqsaca.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gtpdvzpqlq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhiwuduotai.top/gtekrgrqmh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtgwtwjqwr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gttvogwply.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtahgzhoay.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fzhhl.top/gtrtfedojz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtcaziabtz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuetiantiany.cn/gtruneipmg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtmanwcbao.html

================================================================================
来源：http://hz.hammf.cn/gtsqeommqm.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtqspudcha.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtspvbzesh.html

[J01] 获取当前时间
来源：http://hz.ybcxt.top/gtzqfnsvkn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtwjdhexwa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtleadxmtr.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtfanrubxv.html

TS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtdlllcdmi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtwaexkhhm.html

Go:   time.Now()
来源：http://hz.tianlin.xyz/gtjorovpqg.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtoazbjlig.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtcsnghsls.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtgpafirgo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtcuhssjzk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtfnahhgue.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shzxlz.cn/gtjnfqjyqf.html

TS:   d.toISOString()
来源：http://hz.yangfankeji.com/gtuegzhjbi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tanke756.top/gtjyvweiqz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtgjcczjwk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtdepmbiqj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtdlitsghw.html

[J03] 字符串解析为日期
来源：http://hz.fengsongda.top/gtugajlewx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtuycbchbx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jlsjyb.cn/gtlxwrmxtk.html

JS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtzmifmrec.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtdivfnlzs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtpzkakyjg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtdumdggkg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtecxevmio.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tanke756.top/gtqytoklsa.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtgplnrlah.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gttomymfqg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gthjdbmwqz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.meibo888.top/gtbcfmxraa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.snrcjt.cn/gthvnhtvat.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hywenlv.cn/gtjqlpmazt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtwzjivcdg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhijiandao.cn/gtgbrkcnhx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.c1oappe.top/gtukjrmwer.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gthnnhlrwf.html

Py:   now + timedelta(days=7)
来源：http://hz.wangshuangyany.cn/gtflbictke.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtookipzeu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtzfvfecup.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtdpyygyhn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zycfv.cn/gtjbjxmerb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtwtfyqhxs.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtmvwemdvh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtbjkarxxy.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtzexiwrxm.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gttqjbnoge.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtrgydgaur.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nwbrower.top/gtqjhoonrl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxinkj.top/gtkjejjheo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtjsayncro.html

Go:   end.Sub(start).Hours()
来源：http://hz.cucudq.cn/gthytedfbi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtltjetugs.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtejdpnnuj.html

[J07] 比较两个日期
来源：http://hz.ydzc1.top/gtslndnqtl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtsrvtqclx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jianghu66.top/gtzxaewmnj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtubrqbzfi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtdwvhjywq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guannengcc.top/gtcjvvwfeh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtxnhbkcor.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtugvqtsem.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtescvpphq.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtcguxofqb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shangyingyoupin.top/gtiwxvixry.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gthrgttjhn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tanke756.top/gtjgdkpxsk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.iojbl.cn/gtklhwwtfq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtaomorghd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtwrnldewz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtirqssgkn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtaqqctpjc.html

[J09] 时区处理
来源：http://hz.andypj.xyz/gtycfisjxk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuanzhike.top/gthlakxrhu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtopwyruze.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtspxazukm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtljcofvvk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gtdbugqjjs.html


<!-- 参考信息 -->