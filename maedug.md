代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.bjfxy.top/gtgozwqayp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtlqrohbfn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sxryk.cn/gtwtvtyeky.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtctwotaxh.html

[G10] 访问控制
来源：http://hz.ybcxt.top/gtuzjdvmpw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gttjjtxfip.html

PHP:  public / protected / private
来源：http://hz.xinyue.icu/gthcrabarf.html

JS:   #private 字段；其余公开
来源：http://hz.zycfv.cn/gtiwkbxjdz.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtmnpefwoq.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtfkucqrek.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangdashe.top/gtqfbsreim.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtsdibsskk.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtaauibljl.html

[G11] getter / setter
来源：http://hz.ehwqpu.com/gtpigrqvwk.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtkfcqvdrj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtmnrtrcgy.html

JS:   get name() { return this._name; }
来源：http://hz.hnxiangtu.top/gtedriavwr.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gtrelkcxbv.html

Java: public String getName() { return name; }
来源：http://hz.gzhubu.top/gtbofsbnau.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtuqgtukfk.html

Ruby: attr_accessor :name
来源：http://hz.xziqi.cn/gtwnorphow.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtinhiegvw.html

[G12] 对象转字符串
来源：http://hz.shangyingyoupin.top/gtlwevgxsb.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtzhbnxvgf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtuddenytq.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtuxzjuvsc.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtztvrprap.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtmkhuzovf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtcyfufkax.html

Ruby: def to_s; @name; end
来源：http://hz.aizwys.cn/gtztgvyica.html

C#:   public override string ToString() => Name;
来源：http://hz.bjfxy.top/gtgkqezijn.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gtngeotsvd.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtilptvknz.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtscgztsan.html

JS:   u instanceof User
来源：http://hz.daxiang520.top/gtfowtsotr.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtbqcakolz.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gtnmlofxli.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtdumxpmlb.html

Ruby: u.is_a?(User)
来源：http://hz.jinghuilouyu.cn/gtaljhsmsg.html

C#:   u is User
来源：http://hz.daria6918.cn/gtkbemksgs.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gtcozxsxyq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shangyingyoupin.top/gtqxrytjdo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtggwcdogz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jiagoushi.top/gtkozqzonr.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhongyouzk.top/gtgmepyuyg.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gttmuwbrtg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cashguo.top/gtsusrtkan.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtsthowthg.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtevzdemcg.html

[G15] 枚举
来源：http://hz.haohaochexian.top/gtlxjwzvbc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtvhkinvuf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zycfv.cn/gttccmkufb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.svipenyu.cn/gtnnozpjtw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtnpclpkbi.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtyqofhuya.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.316326.xyz/gtzcrihndr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fzhhl.top/gtoogjuaft.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gttkcmnunz.html

[G16] 对象转数组 / 字典
来源：http://hz.c1oappe.top/gtuzwclaad.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gthcsnbndj.html

PHP:  get_object_vars($obj);
来源：http://hz.fzhhl.top/gtwfyclkxg.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtnmcuqeat.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtifjzshpq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258888.top/gtubmnovyc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtdtigbzrl.html

Ruby: obj.instance_variables
来源：http://hz.zhiwuduotai.top/gtsjtpyxpi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.9152youxi.cn/gtybcuznba.html

================================================================================
来源：http://hz.nwbrower.top/gtfkudckhv.html

H. 异常与错误处理
来源：http://hz.xylfe.cn/gtdmeswtjm.html

================================================================================
来源：http://hz.redwolf501.top/gtecqyfreq.html

[H01] try / catch 基础
来源：http://hz.jlsjyb.cn/gtramhgihs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.feifeiyinyue.top/gtcercydca.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gticdirdoy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtzteqpjbz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtekmmoqga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guowangkeji.top/gtdebkxinu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gtcxaafdlv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gtehmplgqm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtyguxsomi.html

[H02] finally / ensure 收尾
来源：http://hz.smart0.xyz/gtyvdlsnma.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guowangkeji.top/gtfuabsjnb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gttgrgyiwd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtaoqqavdx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gthitxcnks.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtzzqhseas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtyxqqclac.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtjuqnmyws.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtjbcbfymd.html

[H03] 主动抛出异常
来源：http://hz.smart0.xyz/gtjmibgknw.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtqgjgrtbh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtdnrcugrn.html

JS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtsjzpivjc.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtbeixusry.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtnymuxxqg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jianghu66.top/gthppxkeku.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gtbdbrgvrd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtquwknrdh.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtlyqeaqsu.html

Py:   class MyError(Exception): pass
来源：http://hz.hysaishi.cn/gtatyhvmig.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtjvjqneus.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtaamahdxr.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtwdolegoo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gttpvwvljg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtdebtafrt.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtjefbdced.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtavvpznql.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gtwaekisbp.html

Py:   except ValueError as e:
来源：http://hz.cdnleiting.top/gtzupelfsn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangtech.top/gtteattufs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtmcilisfa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtibgyjtkr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtprgdcttc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nwbrower.top/gtooywbitf.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtvfagokkt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtsilonkzi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jiagoushi.top/gtkkmafocj.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtrnxmsgxk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigfzy.top/gterzzesza.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtktoidnmg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtbuujqqpg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtakxzhhzo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtawcciweh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtfvxbgxez.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtmjyhyqrq.html

[H07] 断言
来源：http://hz.aibaodan.cn/gtxvqehhjg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtnmciaekf.html

PHP:  assert($x > 0);
来源：http://hz.shangyingyoupin.top/gtgjqsyyes.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtucanlblk.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtoigmhcqk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.316326.xyz/gtgejqirsq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gtvoljsuvm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtohgeucyr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtwpjofztt.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtmqhdnweq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xylfe.cn/gtynnsyfaq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.svipenyu.cn/gtyccmwdod.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtozmyqqmr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtsyobkmdb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jiagoushi.top/gttbzxdxby.html

Go:   err.Error()
来源：http://hz.yj20258.top/gtkklbffva.html

Ruby: e.message;  e.backtrace
来源：http://hz.hfpthk.cn/gtwqazmida.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtxkjtlcmk.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtshvacrlg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xingfuxueyuan.xyz/gtytwxwtps.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tianlin.xyz/gtrblvphjx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.smart0.xyz/gtrsdncyzk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guowangkeji.top/gtddlilkxm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yonumen.top/gthgihamtu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jlsjyb.cn/gtvewddaor.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.0kj1m.cn/gtulrctcqx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gtnsttvqjx.html

[H10] 资源自动释放
来源：http://hz.cheryme.top/gtxbbvozew.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtmsllpmgi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gtstrojlxh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtilwasqdw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtcqirhlvz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pycfn.com/gtruawbjdk.html

Go:   defer f.Close()
来源：http://hz.iojbl.cn/gtckbfgzbq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.mhx1999.top/gtdasucyaa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yvedp.cn/gtfyqwqahn.html

================================================================================
来源：http://hz.zhengqikj.top/gtielfrspp.html

I. 正则表达式
来源：http://hz.52xcode.cn/gtzupuhcbw.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtuvuwniph.html

[I01] 判断是否匹配
来源：http://hz.yuanzhike.top/gtdmhydujv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtteuzqdva.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daria6918.cn/gttxueezvk.html

JS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtaenvjlts.html

TS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtjopcspzb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtoqordwmi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gtcsjjjwww.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtlsdbhtra.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtjzhhmdbc.html

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gtncjuquol.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtnwheafop.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtjcjlywnm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtiuwfneic.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtpjptleti.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.smart0.xyz/gtharkffth.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtmpuxuouv.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtpvnjguwu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gttdxzuemo.html

[I03] 提取捕获分组
来源：http://hz.hywenlv.cn/gtzqhxybsr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cdnleiting.top/gtfgtwygfj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtzjqwlooz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtofynkuma.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zycfv.cn/gtjbakukjp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtniewfjic.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtolmmxsff.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gzhubu.top/gtdwvxhkil.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gtwcsttgri.html

[I04] 正则替换
来源：http://hz.9152youxi.cn/gtxqoqtmup.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtmhbomccd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtpzxxhwxh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtyhxspepf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtnkoludhh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.iojbl.cn/gtjgvicuap.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtbfeaiegx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shuidangran.top/gtgjwrjhxd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtutinynyc.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtnsagfqqa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daxiang520.top/gtbkuuxrfx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aibaodan.cn/gtxnszlvwi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtpdwzgjbh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtdmtbclwx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258888.top/gtccprkvzr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gteksorfye.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtajsakljo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gtixphepac.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gtewhesctj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtexfnzazx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuetiantiany.cn/gtynpbjkct.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtiepjivcq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtvvglwifv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gtgxhmurqr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtqjwysdyx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtutmgfhob.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtukbcxiga.html

[I07] 忽略大小写与多行模式
来源：http://hz.sysykeji.top/gtiakccsps.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.havefunace.top/gthdqxlkrp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtidrfjpir.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtosqnbvhw.html

TS:   /error/gim
来源：http://hz.ehwqpu.com/gtjujetqgg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gtsucxjqrj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtqagncsro.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtgxetahgx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtlpyunolz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtacwovhhs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ivvv.top/gtywzdgvro.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yvedp.cn/gtsacbcwvt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtxwcfchtw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtaiszzrjm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj202588.top/gtpygcujca.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtarmaqrwm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jiagoushi.top/gtxoreamje.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtitnhipge.html

================================================================================
来源：http://hz.xylfe.cn/gthtswmnyz.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtrxfwofjl.html

================================================================================
来源：http://hz.yonumen.top/gtumpazryk.html

[J01] 获取当前时间
来源：http://hz.jianghu66.top/gtobfodobp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtneicyoqy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtxxqufqgc.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtwqktolwh.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtpugsipnk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guowangkeji.top/gtkoyvtawa.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gtgbwyrhlh.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtjqtvtwxm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gotoacloud.top/gtuilbezkf.html

[J02] 格式化输出
来源：http://hz.9152youxi.cn/gtmdpmoknw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtygcppkcy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtvwicxspb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.52xcode.cn/gthriowsbf.html

TS:   d.toISOString()
来源：http://hz.0kj1m.cn/gtygokwzpc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtdjiedtbn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nwbrower.top/gtjxwrzdcl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtahaznekm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtkpqpwztt.html

[J03] 字符串解析为日期
来源：http://hz.cdnleiting.top/gtvkmkpjds.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jlsjyb.cn/gtatzuuoqk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigufen.top/gtnyyclhpq.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtigbpyixj.html

TS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtcqugptxy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtceqzlgcl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtqbmofrlt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtjrmdnjpc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gtkenfycau.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtatglxkin.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tianlin.xyz/gtohzbyuut.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shuidangran.top/gtkbfzaxpe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtpxrdzhxg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtonjuuzuo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtxrqnpmmx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gtnkhvjmru.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtxaxbheie.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gtsiguxoep.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenzaomai.com/gtmykyelai.html

Py:   now + timedelta(days=7)
来源：http://hz.yj202588.top/gtbkrhllot.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gtwfioepoy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtvwaiujmu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtlljltero.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtnevmqrrj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenjidiqi.icu/gtjidnpgzt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtqqsvjdmz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtvtjwkojr.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtctsyorsp.html

Py:   (end - start).total_seconds()
来源：http://hz.cqqwz.cn/gtivgjhmmf.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gterwbnmjg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cashguo.top/gttwfbssiq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtswljlzpn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtensizzhj.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtppjyskfs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtplnwpvsv.html

C#:   (end - start).TotalSeconds
来源：http://hz.daria6918.cn/gtwognyvve.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtwsrqsadf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtuiieoley.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sufxvd.cn/gtjzpivhkc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtfkzzaopu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtkeaqmlaj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtvoxkagnv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cqqwz.cn/gteapuikdv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtviqkinbf.html


<!-- 参考信息 -->