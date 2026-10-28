代发 wailian999

[G10] 访问控制
来源：http://hz.52xcode.cn/gtnpywzrwn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yongpay.top/gtaujafmoc.html

PHP:  public / protected / private
来源：http://hz.tanke756.top/gtpoumujui.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gtryotxskp.html

TS:   public / protected / private
来源：http://hz.ehwqpu.com/gtfpisfzjx.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtdepuvblu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtjkdeyrsr.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtsnfskcqf.html

C#:   public / protected / private / internal
来源：http://hz.aizwys.cn/gtzchyswfr.html

[G11] getter / setter
来源：http://hz.jinghuilouyu.cn/gtssrhgkjy.html

Py:   @property 与 @x.setter
来源：http://hz.kuanghao11.cn/gtksgorbrr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtudwribkk.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtqlmnlirs.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtfhbptxef.html

Java: public String getName() { return name; }
来源：http://hz.xylfe.cn/gtdnbrfzxi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtobngmalr.html

Ruby: attr_accessor :name
来源：http://hz.pengpengdd.cyou/gtgeiohuks.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gthwgepldt.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtkwtzamph.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtzzxorgry.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtoafqgvly.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtwwxqdyeo.html

TS:   toString(): string { return this.name; }
来源：http://hz.yongpay.top/gtuoaysnml.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtrwqsgfrt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtpftrzqgl.html

Ruby: def to_s; @name; end
来源：http://hz.fzhhl.top/gtizeglnbv.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtyeznirzf.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtlnvsffhb.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtocaiufge.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtbwktbtrk.html

JS:   u instanceof User
来源：http://hz.cheryme.top/gtetepwvyc.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtymfdsxno.html

Java: u instanceof User
来源：http://hz.hnxiangtu.top/gtqrhcivsc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtmjheakwc.html

Ruby: u.is_a?(User)
来源：http://hz.pycfn.com/gtcabzikgu.html

C#:   u is User
来源：http://hz.xuanzx.com/gtwxgnwjmn.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gthrteowat.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtxbozivry.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gthtpcyqkb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangshuangyany.cn/gthowayyic.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtbwrxcabq.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtnlxebhwt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtgduhjawt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtkdyfnycq.html

C#:   record User(string Name, int Age);
来源：http://hz.snrcjt.cn/gtrhzdekak.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gthnhxrngn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtofnzgkpz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydzc1.top/gtzobjffmd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.feifeiyinyue.top/gtavvpnjvn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtqakrihof.html

Java: enum Color { RED, GREEN }
来源：http://hz.cashguo.top/gtbzxyigsp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtywdexkeg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhongyouzk.top/gtzlmhmstk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtthrubzbi.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtnljjuobq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhengqikj.top/gtsborshcr.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gtbimlxhyj.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtwtqqqwna.html

TS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gttahdybwl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtgjdugkxp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtpcyrfecy.html

Ruby: obj.instance_variables
来源：http://hz.yvedp.cn/gteqfbkuly.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtesmntsoo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpqgdcdnt.html

H. 异常与错误处理
来源：http://hz.chenzaomai.com/gtyyiyqpqt.html

================================================================================
来源：http://hz.xziqi.cn/gthyapzvvp.html

[H01] try / catch 基础
来源：http://hz.ydzc1.top/gttytcipol.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtjflgaqwh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gtxvtyfivn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtilyzfxku.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuxming.cn/gtvoyohfxt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yonumen.top/gtbhxohqhe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gthpzazxnz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gtxcjodeuy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xziqi.cn/gtfdjfoxqh.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtrtaqhgtj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtgfochftu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtrqhqqlhb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gthsxjsvmy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtphmlzpyi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtwhdqvmoi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tianlin.xyz/gthwxrbfnq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhixingplan.top/gtmlyyvjde.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daxiang520.top/gtfilbbhfd.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtaglxnvdt.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtovfbecyz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtvnacsmiu.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtpeoevtnw.html

TS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtypilsusu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtxhnhchly.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtopjrkxvr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtrgimchuk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtgpdozonu.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtdahzmmrx.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtpojmmjmw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yonumen.top/gteoffqouz.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtosgrezxi.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtqqtyxajt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtkrsjmjva.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtvjjkooxq.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtrvpuxxcf.html

C#:   class MyException : Exception {}
来源：http://hz.52xcode.cn/gtxzahiulg.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtsbshdmzf.html

Py:   except ValueError as e:
来源：http://hz.vqdsnc.cn/gtvnhpjlir.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtrqzrywqq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gttvrkqwyg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtahmurcnq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtzqvyhosp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.mhx1999.top/gtrmfezjgb.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtfqaogrcv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtpxzhzpzm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gtykvfakoc.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtvibpbpwc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenlongwang.top/gtehrxugwr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtmbsxswot.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtspzzcmnc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.dianchejie.cn/gtgbpxbvwj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gtahcslpsc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.iojbl.cn/gtjmzflkba.html

C#:   obj?.A?.B ?? default
来源：http://hz.smart0.xyz/gtriyfwzad.html

[H07] 断言
来源：http://hz.aizwys.cn/gtsyvuadil.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigufen.top/gtwsbyzabk.html

PHP:  assert($x > 0);
来源：http://hz.ywan-chungtsiang.top/gtgwduxjac.html

JS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtayqdmruz.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtlzwvurlv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtybgkzunb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.smart0.xyz/gtogdkxmej.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtcmvnovdd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xziqi.cn/gtmblpemjl.html

[H08] 获取错误信息与堆栈
来源：http://hz.redwolf501.top/gtslcaglkt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtiuvqrsaw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gttmpsluez.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtxvqkkgpo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yangfankeji.com/gtobbbjlfg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shzxlz.cn/gtohanqbih.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtwplpfwmi.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangtech.top/gtryvubwog.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuxming.cn/gtwdvtmomx.html

[H09] 带错误码的异常
来源：http://hz.yanxiufei.cn/gtkkxyogsx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigfzy.top/gthawdtxjt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ybcxt.top/gtpomhnrod.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.52xcode.cn/gtwheamecy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gtrcapqwpu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtcecgfrrh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtfdfsvghk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtqgrhvzpq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gtgjhwtljm.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtfolgnmsh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangtech.top/gtssyoxzuw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtwusithcz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtkjfajupl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gticupecqq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xingfuxueyuan.xyz/gtezrjwrwb.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtiipxjjyb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.0kj1m.cn/gtiajxqkbz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gotoacloud.top/gtphpqkmrp.html

================================================================================
来源：http://hz.hnxiangtu.top/gtggpzubeq.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtijvuufxf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gticjbfgto.html

[I01] 判断是否匹配
来源：http://hz.gaohongyu789.top/gtgjjtigow.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gthwkpucgj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ybcxt.top/gtxdwuqgxb.html

JS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtpiwkbedc.html

TS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtitomgcmh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtjzvkzguz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.snrcjt.cn/gtkjcljcex.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtwfspaxig.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ywan-chungtsiang.top/gtpfrhsebb.html

[I02] 提取所有匹配
来源：http://hz.ydzc1.top/gtothvdutn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gticuotfkd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gtwhgblvjc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gthfadzoxy.html

TS:   s.match(/\d+/g)
来源：http://hz.ydjk.org.cn/gtdcjujndv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.c1oappe.top/gthdznnyfa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.birdmap.top/gteyndjacx.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtrsfstsor.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gtndbijbby.html

[I03] 提取捕获分组
来源：http://hz.gzhubu.top/gtomoezecs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtsawxehen.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtjxdsrkcp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtrsrqzgcq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.vqdsnc.cn/gtwkhpovoy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhaomingkeji.xyz/gtrrhglttl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtraxgricu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gogol.net.cn/gtklgpotfa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gtsucbobuy.html

[I04] 正则替换
来源：http://hz.pycfn.com/gtnosjwkji.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gtygpnlfpk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.birdmap.top/gtxjjoqrdz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtivtdsfes.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtkosogqnr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj202588.top/gtmotkyhir.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtpduxysnq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shuidangran.top/gtgzmvuiop.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shangyingyoupin.top/gttmyepybf.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtmewdogty.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ywan-chungtsiang.top/gtegbcwyaw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinghuilouyu.cn/gtjraglusj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtfzlayzzg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtwdkyfflp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtyueitwsd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gtmdhkkwmp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtvddksahf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fengsongda.top/gtxfavwgrw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sweek.top/gtsnumzogk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtmcsscffd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhaomingkeji.xyz/gtilssaupl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtbwlpzlxi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtltjdhnes.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.52xcode.cn/gtnvrmqrqm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dianchejie.cn/gtrxnbasml.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.0kj1m.cn/gtasdxvhsa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtekdeiakk.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtieoyqdyp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gtbkldohxw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtbqvpztvw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gttmazavqc.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gttctvkoxj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daxiang520.top/gthjghmxbg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtzxzgcwnk.html

Ruby: s.scan(/error/i)
来源：http://hz.hfpthk.cn/gtpmoqqxkm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtclstkkxh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dashuyun.cn/gtdnpkpohk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtaurusbiq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtsewnvipq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtnplqiuqy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtvggyqhvl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtqxhtbjak.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtvwynqpal.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtlnkfkzsp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtwmltnttg.html

================================================================================
来源：http://hz.pycfn.com/gthmynvsrc.html

J. 日期与时间
来源：http://hz.c1oappe.top/gtgnydbuyk.html

================================================================================
来源：http://hz.cqqwz.cn/gtoeawcpzy.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtbozdzabq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtvkwobpof.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtzuwpiuto.html

JS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtuhvyrwyh.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gthlqtecdg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gttgibayik.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gttebhkqtr.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtkhcetlxd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangdashe.top/gtwjaqcmws.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gteijkacqy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtghadfkoj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtuitlncwg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guowangkeji.top/gtzfxixzza.html

TS:   d.toISOString()
来源：http://hz.jqgfzy.top/gtnzldnbzv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cqqwz.cn/gtjqftfkro.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cucudq.cn/gtgatlfbmw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtlszdjmcr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtliffwkvf.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtnkmpxgcb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.quarkkingdee.top/gtchfzpyku.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dashuyun.cn/gtbumciewd.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtixcsvujh.html

TS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gthigamjpf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtmdkggftj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ivvv.top/gtaufaetbt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtptfmincd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtezwgcjgp.html

[J04] 时间戳与日期互转
来源：http://hz.ivvv.top/gtvfphrrvj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtrvwlfsql.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daxiang520.top/gtajnfgjhm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigfzy.top/gtywfpiqzd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.vqdsnc.cn/gtnijjddvr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangkeji.top/gtvsomtifl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtnmncsafx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtgvschsup.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangkeji.top/gtxxsszigq.html

[J05] 时间加减（加 7 天）
来源：http://hz.ywan-chungtsiang.top/gtyakjepuw.html

Py:   now + timedelta(days=7)
来源：http://hz.vqdsnc.cn/gtrkisqsfs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aizwys.cn/gtqchgrvce.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtjolpndiq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtjrkitvfx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sysykeji.top/gtomyyadso.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gtwmdggrpk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtzjvbbexz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yongpay.top/gtcoivbpen.html

[J06] 计算两时间之差
来源：http://hz.dashuyun.cn/gtmsudjuzp.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtntpsaimj.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnxiangtu.top/gtstctqift.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtruwwjrjg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangdashe.top/gtylzecdng.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtxjvfzxwd.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinyuanbaomall.cn/gtpcncopii.html

Ruby: end - start                 # 返回秒数
来源：http://hz.havefunace.top/gtnqrngalu.html

C#:   (end - start).TotalSeconds
来源：http://hz.havefunace.top/gtdvxptpmd.html

[J07] 比较两个日期
来源：http://hz.meibo888.top/gttveyycbj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtpjsiisgr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtbaebcurx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtzynyjxmw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtjyjusuil.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ehwqpu.com/gtssppmdev.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtbiipjeos.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gttpwsqtzs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtigijvcna.html

[J08] 提取年月日与星期
来源：http://hz.shzxlz.cn/gttbroqgfz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ywan-chungtsiang.top/gtfkrbfayx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dashuyun.cn/gtafeyrgvf.html


<!-- 参考信息 -->