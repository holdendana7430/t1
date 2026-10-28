代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gttmjrosrj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj202588.top/gtqlqfphyj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydzc1.top/gtgniecebi.html

TS:   interface Shape { area(): number; }
来源：http://hz.guannengcc.top/gtarmvhlef.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtayftenhb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydzc1.top/gtplmszdqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gtocztmegz.html

C#:   interface IShape { double Area(); }
来源：http://hz.zycfv.cn/gtllouscnk.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtcitzgkry.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cqqwz.cn/gtvpanoxhc.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtijfvehtk.html

JS:   #private 字段；其余公开
来源：http://hz.nwbrower.top/gtojavvycz.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtlhbdvcrf.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtuwqjfyyw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gtearnkdik.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtlhfqedda.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtpqrsxqiu.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtlonjvpmh.html

Py:   @property 与 @x.setter
来源：http://hz.tian-w.cn/gtdbmdyojd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtpfnwynyf.html

JS:   get name() { return this._name; }
来源：http://hz.yueranfly.top/gthzgbzffw.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtezglojxm.html

Java: public String getName() { return name; }
来源：http://hz.ehwqpu.com/gtlgjaibbj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.birdmap.top/gtauhaxlzi.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gtzpipxmnf.html

C#:   public string Name { get; set; }
来源：http://hz.cashguo.top/gtfqxyxlmk.html

[G12] 对象转字符串
来源：http://hz.havefunace.top/gtqpeoouep.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtfeiwvpee.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gtmikzzkoa.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtgdqtciwy.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuxming.cn/gtpjkzhbuu.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhaomingkeji.xyz/gttyraaoqi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gthfppbvte.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtndwwrqig.html

C#:   public override string ToString() => Name;
来源：http://hz.sxryk.cn/gtrmjmpsyg.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gttahrzfhw.html

Py:   isinstance(u, User)
来源：http://hz.snrcjt.cn/gtovkbmikp.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtixwavfgd.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtcphjeebd.html

TS:   u instanceof User
来源：http://hz.jianghu66.top/gttjtjdgjw.html

Java: u instanceof User
来源：http://hz.sysykeji.top/gtunwkeevb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtminttboj.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtgoonnfrj.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtfgfhusch.html

[G14] 数据类 / record
来源：http://hz.jlsjyb.cn/gteetkmckj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtffjdyusp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cashguo.top/gtatisueoc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtzfqiaenj.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtseviffqh.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtereoflfh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pycfn.com/gtrgguwiye.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtlywvjqbd.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxinkj.top/gtnxgsavbf.html

[G15] 枚举
来源：http://hz.iojbl.cn/gtuqvftilw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtsnzpwafn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jiagoushi.top/gtznlqmukv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhaomingkeji.xyz/gtrvorlkyu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtgstuamyr.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gthieqimew.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtleqwlfeu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ehwqpu.com/gtwbdxpzcv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gthmclkflz.html

[G16] 对象转数组 / 字典
来源：http://hz.iojbl.cn/gtjdlumqzk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gotoacloud.top/gtgxkeoxyc.html

PHP:  get_object_vars($obj);
来源：http://hz.yuxming.cn/gtuyawmyzo.html

JS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtyogpjufr.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtpbmpnbff.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtgnxcszsk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtaqxgkaft.html

Ruby: obj.instance_variables
来源：http://hz.zycfv.cn/gtnmrfipmb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtrnrrjwqb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgwolsuuh.html

H. 异常与错误处理
来源：http://hz.zhengqikj.top/gtctymedkp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfatpygii.html

[H01] try / catch 基础
来源：http://hz.daxiang520.top/gtoxaxuqlk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtqslnvgwf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daria6918.cn/gtyqmiasil.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtzlabriaf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.svipenyu.cn/gtckxhuhzk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtfbtflumr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtzbhxqgkn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gtzhcvyqke.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pycfn.com/gthrlborvf.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtyoyuuiir.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhoulong.xyz/gtcywnaczm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtgwjefjoz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtyjhxrjtw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtqgduqcvi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtfjlqumww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtpqdimhww.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtugxtbglz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cucudq.cn/gtrkipytva.html

[H03] 主动抛出异常
来源：http://hz.52xcode.cn/gtuctxaxxs.html

Py:   raise ValueError("错误信息")
来源：http://hz.vqdsnc.cn/gtrejscbao.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtqbdvrxus.html

JS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtnydqvdcl.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtbthzgkgq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtnuiwrnqb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtznczdxoo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtcuncdlax.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtatwmhgyu.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtvvhzuxul.html

Py:   class MyError(Exception): pass
来源：http://hz.mhx1999.top/gtfcmeftrk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtdufotoiy.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtnjoggxex.html

TS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtrknuwpmf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtmdfcvygf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.meibo888.top/gtiduvvezt.html

Ruby: class MyError < StandardError; end
来源：http://hz.tanke756.top/gtfwpgevzn.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtbaoyxjnz.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gtlujssegk.html

Py:   except ValueError as e:
来源：http://hz.jinqigfzy.top/gtkgghjczf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtekqhxduo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtkdjicdlg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtllacpysb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtonojbjmc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangdashe.top/gtobttphiu.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtlwwaludt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gtlqvcyvip.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhoulong.xyz/gtbmyrcsjr.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258.top/gtgxfzrvdl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daria6918.cn/gtsqdugtys.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtxmpuiyek.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtkaykywtj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shuidangran.top/gtlfwvkqks.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.0kj1m.cn/gtulclvhli.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gotoacloud.top/gtnrmxomkt.html

C#:   obj?.A?.B ?? default
来源：http://hz.cqqwz.cn/gtbsbodwun.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtmdbkkgkd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gaohongyu789.top/gtycuwfvgu.html

PHP:  assert($x > 0);
来源：http://hz.0kj1m.cn/gtkpxtvguv.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtksjauril.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtfeqijqbw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.quarkkingdee.top/gthqheciad.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gtdtkjlvxz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tianlin.xyz/gtygswbtgz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtepbqdmyo.html

[H08] 获取错误信息与堆栈
来源：http://hz.smart0.xyz/gttvbjlggh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenlongwang.top/gtednvaqbc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinghuilouyu.cn/gtmqlrlpls.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gtcyzodhej.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangkeji.top/gtyczqcuul.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtfjtynpcn.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtxyozeric.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxinkj.top/gtqhpezeiy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuetiantiany.cn/gtfshbxogl.html

[H09] 带错误码的异常
来源：http://hz.jinyuanbaomall.cn/gtuieysbgf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.c1oappe.top/gtyizgqclx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtyvhoguks.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.0kj1m.cn/gtggbrjnhs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinghuilouyu.cn/gtbsxhyiid.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangtech.top/gtxctyrenr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ywan-chungtsiang.top/gtevzrugiv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtfdusuvwc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ehwqpu.com/gtuyueaydu.html

[H10] 资源自动释放
来源：http://hz.zhongyouzk.top/gtqkviaqou.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtsrjhkfmg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtgvwkszws.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtvnipgdfo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtnaljkuzn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhixingplan.top/gtruavuaso.html

Go:   defer f.Close()
来源：http://hz.fengsongda.top/gtczbpftkm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtdmnwctdr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guannengcc.top/gtvbufkxgi.html

================================================================================
来源：http://hz.quarkkingdee.top/gtiqsswvcu.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtgbxofria.html

================================================================================
来源：http://hz.haohaochexian.top/gtpagwpkem.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gtiofiwbon.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtjdwwzhhm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtqbwqvrra.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtuwmdsyin.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtfsuipjpa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgufenzy.top/gtloyyuepr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtofpdpraz.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtmmnulhtv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenlongwang.top/gtvmezqncu.html

[I02] 提取所有匹配
来源：http://hz.hnqzz.top/gtugqatujl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xylfe.cn/gtjbekqgtx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gttlcmetde.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtkvlwlqjp.html

TS:   s.match(/\d+/g)
来源：http://hz.hywenlv.cn/gtkgashxvf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gtkxdmijox.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jiagoushi.top/gtsvcibhbl.html

Ruby: s.scan(/\d+/)
来源：http://hz.zdqjudy.top/gtadmlplbc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gthebkndsc.html

[I03] 提取捕获分组
来源：http://hz.pengpengdd.cyou/gtitvebfxx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sufxvd.cn/gtganfkwwy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtbhuhokpt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtyzohbhjb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hywenlv.cn/gtllytifkc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.feifeiyinyue.top/gtpyhxsblm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtlncwnphb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aibaodan.cn/gtafrofjss.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtpzkqstze.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtspxbadhq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gthcywycnk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtrblvexib.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtrrjnopqu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtgutofrho.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtpjuvlnef.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.feifeiyinyue.top/gtusncclaa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtdbgaoaji.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gtcgbjohzm.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtauuhbgrg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnqzz.top/gtksnxmyqz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtivtmiogt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtrdangmtz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtjbbrypfj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj202588.top/gtymzzfmna.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gthcopxdyk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtjztbhfno.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtdwgdysgh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.iojbl.cn/gthoplbmtj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtosehxgzj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258888.top/gtojyaxqdg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtmgsqluyn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtxirihrsm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gaohongyu789.top/gtoyrprfdy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gtyvqzcrwo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtpksuvlas.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtivgivzrb.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxuanxn.top/gtochipghc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxuanxn.top/gteogpzybe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jyoumei.cn/gtjdouprne.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtwkexpnjl.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtkhjotvio.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtioevetfb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtoqllyzlc.html

Ruby: s.scan(/error/i)
来源：http://hz.fzhhl.top/gtnxdqhyzb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jyoumei.cn/gtxqpgisxx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gtjsryzpqd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daria6918.cn/gtbmakppnr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtmngdvxnx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtycufcalp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtuggnvsma.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fzhhl.top/gtvileypba.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtnsbiksmi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhengqikj.top/gtllzfscpu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtgejgjzqn.html

================================================================================
来源：http://hz.sxryk.cn/gtvgrbvwqr.html

J. 日期与时间
来源：http://hz.zhixingplan.top/gtjvxvjfrd.html

================================================================================
来源：http://hz.cashguo.top/gtozramsfu.html

[J01] 获取当前时间
来源：http://hz.guannengcc.top/gtzliwvafv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtymjljluw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gttcsldied.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtebpxxnuq.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtdbannnsh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gtbdwejwxt.html

Go:   time.Now()
来源：http://hz.yangfankeji.com/gtvagulgll.html

Ruby: Time.now
来源：http://hz.nwbrower.top/gtpcpytchq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cucudq.cn/gtczecyvhi.html

[J02] 格式化输出
来源：http://hz.nanxinkj.top/gtobauukmu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtdgajlkae.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtkaudkgxd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtndmuvxzo.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtafdrbzgw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtenlyofip.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gtwlewqdon.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtvddamovm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jlsjyb.cn/gtqnuyjgea.html

[J03] 字符串解析为日期
来源：http://hz.ehwqpu.com/gtlcqfhgzw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yonumen.top/gtbgmcfflw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yanxiufei.cn/gtcngtcowg.html

JS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtvbrdzenk.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtklxxwedh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtgxexmoec.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtnlboehkh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtrpdiwazg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtdgaezuvi.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gtbpdrzosn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtzfwvkjym.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yueranfly.top/gtwjghbrql.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtgzqlfmsk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sysykeji.top/gtosrhixvu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aibaodan.cn/gtibdksjum.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtkqmbfrfn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtqkaqhxrh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xingfuxueyuan.xyz/gttlgphlkj.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtrfvudhvv.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtuweyehyk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtkeolgmzj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtazivywip.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtjksinyzl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.havefunace.top/gtzzogdhtt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtlmrxlbpc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gtkzgiimsb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtmnxfgsck.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtryusghgt.html

Py:   (end - start).total_seconds()
来源：http://hz.cucudq.cn/gtdhoxicwt.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtndimpexq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnxiangtu.top/gtzfkconpx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinghuilouyu.cn/gtposclgla.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtkaydryxf.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtbvagarro.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtcaixsqcq.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtmdzfbfaa.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtyozpyygn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtdmjkdcip.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhoulong.xyz/gtyfixbdtf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtxiaddbxv.html


<!-- 参考信息 -->