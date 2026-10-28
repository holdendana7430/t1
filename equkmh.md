代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.jiagoushi.top/gtkyxgtlvd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydjk.org.cn/gtcusatgbl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cheryme.top/gtvqgeuife.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtdccifnvi.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtbczwxijt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtpaofpovt.html

PHP:  public / protected / private
来源：http://hz.birdmap.top/gtufzfbipn.html

JS:   #private 字段；其余公开
来源：http://hz.svipenyu.cn/gtefmcqltr.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtrtrllbbm.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gtovvjjgzv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuxming.cn/gtpwefhtug.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gtttypyeyw.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gttqzvdesj.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gtyyqeatuk.html

Py:   @property 与 @x.setter
来源：http://hz.yuanzhike.top/gtjzmhhnaa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtjcrgzrrd.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtpwslvwwn.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtxuqnsykq.html

Java: public String getName() { return name; }
来源：http://hz.xziqi.cn/gtyjeynjzo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cdnleiting.top/gtclfthzwa.html

Ruby: attr_accessor :name
来源：http://hz.meibo888.top/gtfrbmwhaa.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gttklafaqj.html

[G12] 对象转字符串
来源：http://hz.zhiwuduotai.top/gtpeyowwnd.html

Py:   def __str__(self): return self.name
来源：http://hz.ivvv.top/gtovcbgsdm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtjlihcvph.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gtptausrll.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtexcfnihc.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gtymxxiylw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtsirghdnl.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gteisppqzd.html

C#:   public override string ToString() => Name;
来源：http://hz.guannengcc.top/gtunkdcvwj.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gthlwulhtq.html

Py:   isinstance(u, User)
来源：http://hz.cdnleiting.top/gtwuqzcptj.html

PHP:  $u instanceof User
来源：http://hz.316326.xyz/gtgqasxmem.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtubdoybkb.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gturftigxo.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtkobvlbrm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxinkj.top/gtbftlnrlx.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gtjqnjiyli.html

C#:   u is User
来源：http://hz.feifeiyinyue.top/gtzmzqvkrr.html

[G14] 数据类 / record
来源：http://hz.ivvv.top/gtabkkfsjf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yvedp.cn/gtfecejaez.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gttuorhspn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sxryk.cn/gtbssobnbs.html

TS:   type User = { name: string; age: number };
来源：http://hz.shangyingyoupin.top/gteikfdrfm.html

Java: record User(String name, int age) {}
来源：http://hz.aibaodan.cn/gtkpdpofhy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtundpeays.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtvzvrtyna.html

C#:   record User(string Name, int Age);
来源：http://hz.zhongyouzk.top/gtwjfufwvm.html

[G15] 枚举
来源：http://hz.xziqi.cn/gtrjrpyqbt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shangyingyoupin.top/gtnwezkesq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtfnopmezh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtityxrsvd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtuiygixfr.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnqzz.top/gtawdyvgcx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gtgswwhpyr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuetiantiany.cn/gtywfzyhxw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtsqxcmrjn.html

[G16] 对象转数组 / 字典
来源：http://hz.zhijiandao.cn/gtpiiqxrnh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cucudq.cn/gtyunwctzu.html

PHP:  get_object_vars($obj);
来源：http://hz.fzhhl.top/gtifdytvny.html

JS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gthhsijglw.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtetrehxju.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtuxypijqq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhongyouzk.top/gtfcksfpwh.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtxqyretou.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jlsjyb.cn/gtvedqfoyq.html

================================================================================
来源：http://hz.zycfv.cn/gteaayvdyo.html

H. 异常与错误处理
来源：http://hz.jinyuanbaomall.cn/gtxplsnjae.html

================================================================================
来源：http://hz.aibaodan.cn/gtizydpljm.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtmfupdtbs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtkehighhb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenlongwang.top/gthjjvnutb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtywcfdihu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtkkvdvuil.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtjpjodjhj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtaltodunc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cdnleiting.top/gtkxmmxpck.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.feifeiyinyue.top/gtcrsllizt.html

[H02] finally / ensure 收尾
来源：http://hz.zhijiandao.cn/gttndmfibr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pengpengdd.cyou/gteaxfyawl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtqfpmjemu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtwmaxpvls.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtyoamcoub.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtjbnifkcx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.birdmap.top/gttlmrsgao.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhengqikj.top/gtvzvwnwpr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.smart0.xyz/gtazpxwlco.html

[H03] 主动抛出异常
来源：http://hz.yvedp.cn/gtsaaqjbny.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtvglhpzbz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtyrrqljpo.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gthkuqdaik.html

TS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtasvgqgff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtrmbklfqq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gtiwelnaaf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtraxrvypo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtapengqld.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtigzsfmoi.html

Py:   class MyError(Exception): pass
来源：http://hz.yj202588.top/gtvkvdtuim.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtqameexkc.html

JS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtndmcdton.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtiypdwbjc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtcvbqdwov.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gterkshiry.html

Ruby: class MyError < StandardError; end
来源：http://hz.yongpay.top/gtpicdsubb.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtkhfhmqpe.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtcarsjnbb.html

Py:   except ValueError as e:
来源：http://hz.daria6918.cn/gthrtcrhdt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ivvv.top/gtoabmukym.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtancbrahj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtyswntifz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtsqkkbjtl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gtbdsdaxoe.html

Ruby: rescue ArgumentError => e
来源：http://hz.redwolf501.top/gttvrwwnve.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ivvv.top/gtzszpezme.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtfegpqitd.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtaicqakcr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jianghu66.top/gtfeqyqxkd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cucudq.cn/gtdmoltmvf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtjscbtqke.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgfzy.top/gtpcxfblcy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtzvwpsnbe.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gtpshvmuhg.html

C#:   obj?.A?.B ?? default
来源：http://hz.xylfe.cn/gtksueajlt.html

[H07] 断言
来源：http://hz.ydzc1.top/gtksmbxhdj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gttfmmddyv.html

PHP:  assert($x > 0);
来源：http://hz.gzhubu.top/gtyqvrvxyl.html

JS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtysjlcqlg.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtkfrgyjbh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.quarkkingdee.top/gtqeikrikj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtcrjxenfs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydjk.org.cn/gtzkodtmnn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtyalmcwns.html

[H08] 获取错误信息与堆栈
来源：http://hz.gotoacloud.top/gtzlipprge.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtlanluqpu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.vqdsnc.cn/gtupwtvmho.html

JS:   e.message;  e.stack
来源：http://hz.aibaodan.cn/gtwctnofry.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gtkxerfyrm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtldrkgkke.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtvfittdsq.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtjgzlcbfu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtpootnhkj.html

[H09] 带错误码的异常
来源：http://hz.zhiwuduotai.top/gtegyfrltb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jyoumei.cn/gtxrfntnrw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtzurulqsa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gtqkstadip.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gogol.net.cn/gtrilauwdi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gttxgmsnns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cucudq.cn/gteawsmxuh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtxfcppzrh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ywan-chungtsiang.top/gtudtzmkdc.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtrultwdco.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.snrcjt.cn/gtrbnxikbb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenlongwang.top/gtokmuaazx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtlhgcwaoe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtkwvlpbfg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtsszylatq.html

Go:   defer f.Close()
来源：http://hz.iojbl.cn/gtdbgugljo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtalhntpct.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtvolrsowy.html

================================================================================
来源：http://hz.aibaodan.cn/gtwpponjbg.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gthffexgpy.html

================================================================================
来源：http://hz.nwbrower.top/gtpgrdtlma.html

[I01] 判断是否匹配
来源：http://hz.nwbrower.top/gtxuwfilwb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtpzyrwvtl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtyaiqzmcf.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtjodfnuio.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtwshgebxd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.316326.xyz/gtbnriulju.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtvxddjcfr.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtrbdmyyrw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sufxvd.cn/gtxlvevttt.html

[I02] 提取所有匹配
来源：http://hz.nanxuanxn.top/gtzruchutw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gturpwgsxs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gtgdnrvgsi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtewkmzmzj.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtfqadvfto.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtiomjknox.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhixingplan.top/gterwkdvud.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigufen.top/gtdacnkxlb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxinkj.top/gtiunulmfr.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtsvdwifqg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gtzwgmiyij.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtcntddift.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.meibo888.top/gtjxpjfreb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gtpumknwed.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.svipenyu.cn/gtbihvegld.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gteobskuxe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtbrfstcay.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtpnovpdej.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtpgeklkbj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhixingplan.top/gtmkirixae.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gttrenpvsd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtzeivzgmp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtexkadggc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.0kj1m.cn/gtlbogqgpd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtxgbxfjqo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtxymirbvv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gtblzayyvq.html

[I05] 按正则拆分
来源：http://hz.hnqzz.top/gtgrnhvolj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtcpzbpnii.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cdnleiting.top/gtgppnhezy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtfebibfec.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtqnzpbjox.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtdnbuzila.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gtotuuoswf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtkygsrqaq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtodwxzosl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtkaspzhhu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtgmzqxcak.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtnskeowei.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtzvvhgvdv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtajzwhdde.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ehwqpu.com/gtwokcsnpc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinghuilouyu.cn/gtrtaoirgx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtcirktprr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtcjttbkap.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtjkuxmctd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtxnirrllf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtwhfrvbez.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtppdtyney.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gtjflpdnxt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtcshirmgp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xingfuxueyuan.xyz/gtmrxxzqhm.html

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gtobtnirhn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jianghu66.top/gtbwdefore.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gogol.net.cn/gtnhppbduu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtoserjrot.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtjgcxhfga.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtfcmxgtza.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtnwoyosev.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtrelsgbqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.snrcjt.cn/gtaokxeqbq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtyjdqoqwn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtnqkfeovw.html

================================================================================
来源：http://hz.ehwqpu.com/gthzruqdsh.html

J. 日期与时间
来源：http://hz.zhongyouzk.top/gtdkdusnum.html

================================================================================
来源：http://hz.tian-w.cn/gtulueyave.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangtech.top/gtrqjxaztk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtcezawmcx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtmzikdvqo.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtwpzrsjmi.html

TS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtiecnnydz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tian-w.cn/gtknqyhgpw.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtbzuudxiw.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtansmpmhh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtkarvzqul.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtzzxizdwu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtjprjmjtq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtciismskl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtvlryqukx.html

TS:   d.toISOString()
来源：http://hz.316326.xyz/gtspsgndra.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daxiang520.top/gtesxmwnmv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenlongwang.top/gtqpjgpakt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gthzvdgrjk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtrhusvdqv.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtfrhsgsop.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtjgwwkuxb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gtppyimsoa.html

JS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtbaixsdda.html

TS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtypobrmsb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydjk.org.cn/gtedlhsyyq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtmjlcrizj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtpjxjtfqr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtoihqxhfe.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gtdosdqxrg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtycvhosxt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtyjnczfbs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.haohaochexian.top/gtooydhttm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtolkwdtem.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gtzykhgdah.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gtzqbcljkj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sufxvd.cn/gtkewlfvox.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtbpwlvxte.html

[J05] 时间加减（加 7 天）
来源：http://hz.redwolf501.top/gtifwuzebw.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtgeeswxwa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtguazbylv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtsjsqwpxu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtwumeqsum.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtorwwadvw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gthymycxxk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sxryk.cn/gtslnhtehu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtjwuvmupo.html

[J06] 计算两时间之差
来源：http://hz.havefunace.top/gtfdphqvsf.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigfzy.top/gtgimnapdw.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtzlfvxpdb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtqzqymhgm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtnymgnues.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gtcwcoprqs.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtvqkytpgv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xinyue.icu/gttyyrvlvu.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtzinjsgte.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtazcochje.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtzwfhxkwa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtjdposlag.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtsaaewazi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtynrkzjuz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gtmubogtch.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtkpwgchzs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtwvbfgpzb.html


<!-- 参考信息 -->