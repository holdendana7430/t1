代发 wailian999

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtporagdps.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtvkxgytzw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtjlajlbzy.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtbktalzkw.html

C#:   public / protected / private / internal
来源：http://hz.xingfuxueyuan.xyz/gtpbrfxdvo.html

[G11] getter / setter
来源：http://hz.chenzaomai.com/gtkunodpar.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtprzygpfw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtsgtmuhxa.html

JS:   get name() { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtkrmgzonk.html

TS:   get name(): string { return this._name; }
来源：http://hz.cheryme.top/gtnyrdozkv.html

Java: public String getName() { return name; }
来源：http://hz.zhongyouzk.top/gteadthrkd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtaiwxbsby.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtrfmmjghg.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gtbhbpfvvl.html

[G12] 对象转字符串
来源：http://hz.jiagoushi.top/gtwrqnkkdn.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gtelhqxasr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gthbvojxdt.html

JS:   toString() { return this.name; }
来源：http://hz.guowangkeji.top/gteqxthbjk.html

TS:   toString(): string { return this.name; }
来源：http://hz.xziqi.cn/gtjyonrmic.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgufenzy.top/gtkaoovedm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtvjbclxzj.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtgsjyrxwt.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtonwlnham.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangtech.top/gtpgtnlmap.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtmllcvoxb.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtmktobgdn.html

JS:   u instanceof User
来源：http://hz.shuidangran.top/gtfskcbskb.html

TS:   u instanceof User
来源：http://hz.yueranfly.top/gtskzgmhno.html

Java: u instanceof User
来源：http://hz.zhixingplan.top/gtaqbkedjj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gtfsaqcyuw.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gtmfihlmxu.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtawtheudw.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtwyxiikdc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gthqngvruj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jlsjyb.cn/gtjegmnxgb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenlongwang.top/gtpiqunzlq.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gtxhgpzwvc.html

Java: record User(String name, int age) {}
来源：http://hz.jinyuanbaomall.cn/gtwytrssxk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuanzhike.top/gtocoapsti.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtyqznbyml.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtleqjnzie.html

[G15] 枚举
来源：http://hz.cashguo.top/gtwetanyrl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ywan-chungtsiang.top/gtgichkfhe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gthgmhssui.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gtftmytztr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gthtrczmxs.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtjdxyreks.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtuixjvksa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258.top/gtkwrxvbwk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtirteqzwn.html

[G16] 对象转数组 / 字典
来源：http://hz.c1oappe.top/gtxxuasijy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtaucsdusg.html

PHP:  get_object_vars($obj);
来源：http://hz.fengsongda.top/gtacyyzcwd.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtdkbpdsdb.html

TS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtamqqxdqm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gtjtoduzms.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xziqi.cn/gtbdffucxq.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtvdcwmwut.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.vqdsnc.cn/gtycuqfoqx.html

================================================================================
来源：http://hz.gogol.net.cn/gtuejbqtcw.html

H. 异常与错误处理
来源：http://hz.sufxvd.cn/gtlvbrkwds.html

================================================================================
来源：http://hz.jyoumei.cn/gtktqbxrxj.html

[H01] try / catch 基础
来源：http://hz.daria6918.cn/gtlsgcgnxv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenlongwang.top/gtfmagjvmo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fzhhl.top/gtcmrllsye.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtpvdvxcbd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtvwkdxdij.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtfkgxidax.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtpvidxeuf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zdqjudy.top/gtfdcbxhhv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sweek.top/gtexhvcgal.html

[H02] finally / ensure 收尾
来源：http://hz.hfpthk.cn/gtdknmpycg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gtsdaadlos.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtmblccewm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtszoqupbm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtyfwyfdck.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtalmflsml.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gttvmxilum.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtjawaincb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.quarkkingdee.top/gtnclsvroc.html

[H03] 主动抛出异常
来源：http://hz.chenjidiqi.icu/gtsqqipohv.html

Py:   raise ValueError("错误信息")
来源：http://hz.kuanghao11.cn/gtgjfruzzg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtaxzbgisw.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtdkgswhve.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtrxkyvpof.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258.top/gtykmurdvi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtionxcfes.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtkhmupekh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gttkjjnptu.html

[H04] 自定义异常类型
来源：http://hz.yj20258.top/gtoxlnwtcj.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtikiskqsf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtdiqgbsxu.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtnjphlqpa.html

TS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtuvleuhap.html

Java: class MyException extends RuntimeException {}
来源：http://hz.meibo888.top/gteeulowjn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shuidangran.top/gtuupzrbej.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtpkurhrmk.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtkeljgkqh.html

[H05] 捕获特定类型
来源：http://hz.sufxvd.cn/gtagfftxqm.html

Py:   except ValueError as e:
来源：http://hz.bjfxy.top/gtnjguxeam.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtehcijgwf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtbsvvvibo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtdrcozlnf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gtizqsievb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yangfankeji.com/gthadzfjsf.html

Ruby: rescue ArgumentError => e
来源：http://hz.c1oappe.top/gtmzwvrqnv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.redwolf501.top/gtswrikgdb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sysykeji.top/gtnoriyglv.html

Py:   value = d.get("k") or default
来源：http://hz.yueranfly.top/gtwlbvkrjt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.smart0.xyz/gtxfcwqjcm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtvsgaxost.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtngnxpnfo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gttpweuics.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gtuhuxefvk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtphwhggml.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtydcfmypx.html

[H07] 断言
来源：http://hz.jlsjyb.cn/gtsbynitkx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cdnleiting.top/gtdhblmhxy.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtmlmrpyti.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtbyyblbid.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtctrvotpk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gotoacloud.top/gtdfdcjfsx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dianchejie.cn/gtrbyhkfvy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangtech.top/gtpflfkcyq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtpwykmqla.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtgaqwrzqd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtzouylovx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.iojbl.cn/gtztblfhbs.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtclwguzvf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtnvazregh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtnjzbeqjs.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtzmncvsgn.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258.top/gthwhexvjw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtsyclvxen.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtwdsmvmbr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtdpohdipo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtqzdmfuea.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtncswpkgk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtcqnnwjpq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtjpdiqoxz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yueranfly.top/gtmoyxsuxa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.52xcode.cn/gtighzgqlm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yueranfly.top/gtsewjlsgi.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtukwamysf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtevwjoaaq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ywan-chungtsiang.top/gttmkevwbp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtaezfbkve.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gttqcvancv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pycfn.com/gtdihddbdd.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtyplgbqgq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtcsxccvkq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtjivohyeg.html

================================================================================
来源：http://hz.redwolf501.top/gtcurvjfqc.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtudfaybmw.html

================================================================================
来源：http://hz.zhixingplan.top/gttmlfbmwv.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtesggdkpj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtcwotakkj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sxryk.cn/gtrgxnwvzc.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtcdqzlnbq.html

TS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtqkpkylon.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yangfankeji.com/gtxydnbuia.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtyaijabqm.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangshuangyany.cn/gtnavcietu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtdgdhvcyh.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtepqbizvq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.9152youxi.cn/gtdqqedmfn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtmvozqrew.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtxwuxwpnt.html

TS:   s.match(/\d+/g)
来源：http://hz.shangyingyoupin.top/gtfujwdxvc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtltcjxoxq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gtxepafugg.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gthdhzmayc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtfdjigjck.html

[I03] 提取捕获分组
来源：http://hz.zhixingplan.top/gtkxhzzyzh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gtqviqnnev.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtogfjgatw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sysykeji.top/gtcyxeuczy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yongpay.top/gtlbcvygcx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jiagoushi.top/gttgvrsfsj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtdosnuuay.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhaomingkeji.xyz/gteainknqy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gtvmorcztp.html

[I04] 正则替换
来源：http://hz.jianghu66.top/gtgdvmixpl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tianlin.xyz/gtprvwcckv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtknghgltr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtigfqmfks.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtyvlshxoe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhixingplan.top/gtxhqclepy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gtczytsdae.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtzxowyvjd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gttxpigovk.html

[I05] 按正则拆分
来源：http://hz.xuetiantiany.cn/gtbctwgdeb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtaghwznqa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtejplwdvr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtklafhacg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtuwidhioz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.0kj1m.cn/gtioslatzm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sufxvd.cn/gtluvoxfaj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtpzjyinpy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jyoumei.cn/gtxdzhwyjw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ywan-chungtsiang.top/gtvsajgqye.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtsjjgojsi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtdbmrwjpg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtaxutjtfc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gttwcebizl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gtwrjxawnr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtnxrktwzm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gtsoahacuv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtyyfmtfgs.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtczbxqjmo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guannengcc.top/gtflwkbymd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuanzx.com/gtbgbdpjpx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.havefunace.top/gtjokhefst.html

TS:   /error/gim
来源：http://hz.jqgfzy.top/gtlrytfuza.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtdyapapgg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtypnqlpba.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtnjnifruh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtaelwcimu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtsmotuqmo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtqfqqbfxl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtrajdncjr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtnsltyvdh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gteclncitw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtwywtqfay.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jlsjyb.cn/gtrggsmrtd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xingfuxueyuan.xyz/gtxofhfyyi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gzhubu.top/gtspzzaoed.html

================================================================================
来源：http://hz.gotoacloud.top/gtjjnkysww.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtajasrybb.html

================================================================================
来源：http://hz.bjfxy.top/gttewlbfsu.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtsyedxhsp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuanzhike.top/gtehykwygu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtpjygnoks.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtvqtgpfzk.html

TS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtbymcewzj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtnkqbfysm.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtgcvtyrfj.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtfwuyffkc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tanke756.top/gthabfxdsn.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtgpxzktqo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtjkohndfw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtsapygvoc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.smart0.xyz/gtvesoibiu.html

TS:   d.toISOString()
来源：http://hz.yonumen.top/gtmzmlqqgy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtsjhzqocq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gtuokpboea.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtxmnjeolb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtqhfhgejl.html

[J03] 字符串解析为日期
来源：http://hz.316326.xyz/gtdewqdsoo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuxming.cn/gtnxuckmhq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gtncmkuobz.html

JS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gtgocgyeal.html

TS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtvirpeagv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtqtbmfcdq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gtjiyckirv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtaghqgnen.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtqhgtufbt.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtlskgtbih.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.redwolf501.top/gtnjjnuapd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yongpay.top/gtqlpplwdk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtddvvpaaw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtumfraufr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj202588.top/gtziioccke.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtzlmfzrcz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgfzy.top/gtvscrkazn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gtyygjretz.html

[J05] 时间加减（加 7 天）
来源：http://hz.mhx1999.top/gtuvmijlmd.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtzyvzutcn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtynfqsmlc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtbapphgzv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gthatiaivd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhixingplan.top/gtobbzighq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtqascqxkg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtgecfsori.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtpsfeluso.html

[J06] 计算两时间之差
来源：http://hz.chenlongwang.top/gtoqscsohz.html

Py:   (end - start).total_seconds()
来源：http://hz.zhengqikj.top/gtbxudkbgw.html

PHP:  $end->diff($start)->days;
来源：http://hz.sweek.top/gtawmhnpsi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.vqdsnc.cn/gtdirujxyq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtbmglbihb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ybcxt.top/gtcmnyqwgi.html

Go:   end.Sub(start).Hours()
来源：http://hz.jyoumei.cn/gtqxuagtfy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtczvbrnzq.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtaioiovhr.html

[J07] 比较两个日期
来源：http://hz.xingfuxueyuan.xyz/gtfhpkkgzd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtrhubvbee.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtvpspuzcx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtctvrdfbh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gtnfokoxmo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtjlyjsxli.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtgeqrcxtv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtisztehgj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtgjwwzlbv.html

[J08] 提取年月日与星期
来源：http://hz.hywenlv.cn/gttnmppdxk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aibaodan.cn/gtwrazeaci.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yanxiufei.cn/gtaznzdmpz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtzlrzacbw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gtlntlkujf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtblgsudja.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtzopabbgy.html


<!-- 参考信息 -->