代发 wailian999

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gtkpgwfcaf.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gttpmekppq.html

TS:   static f(): void {}
来源：http://hz.52xcode.cn/gtwtpmteua.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtliplvbsk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtpvpjgqyy.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtmqgovxmm.html

C#:   public static void F() {}
来源：http://hz.ydjk.org.cn/gtbcmmhjng.html

[G09] 接口 / 抽象类
来源：http://hz.shangyingyoupin.top/gtvhekvthj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daxiang520.top/gtrbsewpfi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gtgrliwprl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtrweqkhod.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtaprrzwdt.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtxqkdyvmx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yanxiufei.cn/gtfhinwpmj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gttvetckvc.html

C#:   interface IShape { double Area(); }
来源：http://hz.dianchejie.cn/gtylghttbd.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtfnhwdmcl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigfzy.top/gtcmhdigou.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtafevblhy.html

JS:   #private 字段；其余公开
来源：http://hz.hnqzz.top/gtjjtbxxyq.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtrvlsomht.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gtgszogtqg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtirfuauaq.html

Ruby: public / protected / private
来源：http://hz.daria6918.cn/gtoqosbuno.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gtcmhpjdwc.html

[G11] getter / setter
来源：http://hz.ehwqpu.com/gtfumtmsjw.html

Py:   @property 与 @x.setter
来源：http://hz.redwolf501.top/gtpqzvzkoy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yongpay.top/gtjifzvowz.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtwotyksxl.html

TS:   get name(): string { return this._name; }
来源：http://hz.cqqwz.cn/gtaliqfbtx.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtmsumdryx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtmrjawlis.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtqniqltbx.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtfnosjmmx.html

[G12] 对象转字符串
来源：http://hz.316326.xyz/gtiifqcaqy.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gtcqsmnztz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gthpujbsek.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gtltbboqph.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gteddnlkxa.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtdqtmspdq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtgthpdbgh.html

Ruby: def to_s; @name; end
来源：http://hz.andypj.xyz/gtwsfywgmq.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtmtkqfpnb.html

[G13] 判断对象类型
来源：http://hz.pengpengdd.cyou/gtvqzcegrw.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gtkpirbukx.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtpzinqmzk.html

JS:   u instanceof User
来源：http://hz.jyoumei.cn/gtwloxvnxj.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtrnqmhtrj.html

Java: u instanceof User
来源：http://hz.shangyingyoupin.top/gtwbikbjxb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gttioaoxjo.html

Ruby: u.is_a?(User)
来源：http://hz.zhiwuduotai.top/gtbvrjnesc.html

C#:   u is User
来源：http://hz.zhixingplan.top/gttsnxjabe.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtphqqmser.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangdashe.top/gtllwouvsj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.mhx1999.top/gtdosgfmxi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtzxjbuomr.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtpiiyzilk.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtwtkubnzm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtkclghdrb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gthvughmnk.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtgeoysxfl.html

[G15] 枚举
来源：http://hz.0kj1m.cn/gtlndfhmjd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtytmzjzsm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yvedp.cn/gtocnxcqfr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtjjonivxm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtcqcmuexn.html

Java: enum Color { RED, GREEN }
来源：http://hz.cucudq.cn/gtbmpifnbq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jyoumei.cn/gthjdsfdwp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gaohongyu789.top/gtctuzwlug.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtiupbbyao.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtjliwnige.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenzaomai.com/gtevzapxqk.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtxvjzsrkh.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtfjcolbzm.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtnrowuyug.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtbdqjwnrw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtzmxpnhho.html

Ruby: obj.instance_variables
来源：http://hz.0kj1m.cn/gtbvryeqkl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aizwys.cn/gtholyhbfl.html

================================================================================
来源：http://hz.hnqzz.top/gteywpdugh.html

H. 异常与错误处理
来源：http://hz.chenzaomai.com/gtaaenkusj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpncvyiiw.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtnjibdogl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhiwuduotai.top/gtdojevomz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtcofirytl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtqtaxlcnu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.bjfxy.top/gtfswfbojd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtjaardxns.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtyuecjukk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtfhivhgxk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258888.top/gtpxszfypl.html

[H02] finally / ensure 收尾
来源：http://hz.hammf.cn/gtdmfwerqd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258888.top/gtcprwsjwj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtcziagfku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gteixnlqvn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtibnashqc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gttungfnra.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.redwolf501.top/gtagvcsbuh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gttbdndtba.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtiiltmupc.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtyjpjpkuz.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gthtfzzaxm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtmabrkjdo.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtpdabarxg.html

TS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtdmstswla.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtmhlcccek.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgufenzy.top/gtihjnjnhz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtqmowvkrs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtiqkmpoti.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtwhzalrby.html

Py:   class MyError(Exception): pass
来源：http://hz.hywenlv.cn/gtpsibfwog.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtuccdelek.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gttvukueam.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtjxxfecin.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtmmrended.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuetiantiany.cn/gtpeycwjok.html

Ruby: class MyError < StandardError; end
来源：http://hz.sxryk.cn/gtdyfqjocy.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtadxbevow.html

[H05] 捕获特定类型
来源：http://hz.svipenyu.cn/gtaqntutfh.html

Py:   except ValueError as e:
来源：http://hz.316326.xyz/gtgqhoimlf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtjmndnizk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtjownhmvn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtitlxdcne.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.svipenyu.cn/gtdttnjcgz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aibaodan.cn/gtuvrmjqon.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtfzwjihjq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtalfgzgbn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtsucpkozn.html

Py:   value = d.get("k") or default
来源：http://hz.zycfv.cn/gtsrqqdwfx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yanxiufei.cn/gtpfoaglkj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtswejowdp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtzcbajtdt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtjgllmqni.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hysaishi.cn/gtjxobhywu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gtmesjtqen.html

C#:   obj?.A?.B ?? default
来源：http://hz.sxryk.cn/gtpglswiif.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtwygtdybi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.bjfxy.top/gtwlvwykxe.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangtech.top/gtbseyslep.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtvonysjuj.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtlwxupkss.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtsgezwgra.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258.top/gtbrlhqdho.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtyuxpifmw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhixingplan.top/gtuvdzerzn.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtxjpzqhjm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtrnyqqvyo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dashuyun.cn/gtkxivwnal.html

JS:   e.message;  e.stack
来源：http://hz.quarkkingdee.top/gtaikuazft.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtbzbxblhi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tanke756.top/gtieblkisc.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtvviliadl.html

Ruby: e.message;  e.backtrace
来源：http://hz.gotoacloud.top/gteitmqpjp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtwvnnukgn.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtvrcsmvka.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sufxvd.cn/gtiwsknlfg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtqfbeodiy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenlongwang.top/gthkowagmz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuanzhike.top/gtpfrbgxqc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtrofgzosy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinghuilouyu.cn/gtxueyetby.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.vqdsnc.cn/gttqmsscto.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shzxlz.cn/gtpnyfsmft.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtapkgamrh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtnmoctxfd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxinkj.top/gtywxprhrn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtiuyeowtu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtqktqwjmc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.havefunace.top/gtobxombho.html

Go:   defer f.Close()
来源：http://hz.nwbrower.top/gtllnyhdax.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtkoolhpss.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yonumen.top/gtubmzzhnx.html

================================================================================
来源：http://hz.yuanzhike.top/gtcrlbzixb.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtrtxhqnsc.html

================================================================================
来源：http://hz.zhengqikj.top/gtvknwkqiq.html

[I01] 判断是否匹配
来源：http://hz.nwbrower.top/gtjpizoirf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtjalznfgw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtcmxjgyqd.html

JS:   /\d+/.test(s)
来源：http://hz.316326.xyz/gtutpbwrco.html

TS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtetyordvv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhiwuduotai.top/gtxbcdkgsk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xylfe.cn/gtdhykeuol.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gteqhlbkvb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtsroovcrk.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtnbwxmoja.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gthcpianiv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gttbniqazi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtilftebzn.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gtlbfhacjw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gtgrcwwnkd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gaohongyu789.top/gtnbbtueay.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtujtzxuqj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtacamfdpx.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtdidpyamf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangkeji.top/gtnyowrntd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtqcpoikyh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ehwqpu.com/gtscguorqp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gteuiufdkr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gtjuzehpib.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtvlupestj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtxzogaodx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gtiyhxibqd.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtcdxtnlum.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gtrufumdvv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtdohngxmj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtbgestfgv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtrogpegnb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gthqlsxlzl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gtcnpkqnyn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hfpthk.cn/gtnnqtaezz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gtrltcsfad.html

[I05] 按正则拆分
来源：http://hz.gaohongyu789.top/gtspoyyopx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangtech.top/gthgsqbyop.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yongpay.top/gtxfuycwcl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtgixyzktk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtrczuqpgu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.vqdsnc.cn/gtkmyatkxr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daria6918.cn/gtrgtamnmu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gttruosnie.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jyoumei.cn/gtfbftdptq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hfpthk.cn/gtnmgjktux.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtlpusswpt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gtfciaqbbm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtmlvavivl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtdifugead.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtvppanirm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtcwxceomw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtuxcrtscj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtpupzvdlk.html

[I07] 忽略大小写与多行模式
来源：http://hz.gogol.net.cn/gtmjiltyjj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnqzz.top/gtjvuguvjy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtjoprsoij.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtixshlkgb.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtjbwnpcum.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ivvv.top/gtqktmbjsp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtxtcuegyz.html

Ruby: s.scan(/error/i)
来源：http://hz.aibaodan.cn/gtfqzffmwl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtmkloqegw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yueranfly.top/gttbmmwfeu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtclclqnyt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.smart0.xyz/gtxssyocda.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtnlzuyibw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtalssgosd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.iojbl.cn/gtywosnuhe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtimefzeev.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtxhoqcibr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtgsdthvlm.html

================================================================================
来源：http://hz.shuidangran.top/gtkgcyixmp.html

J. 日期与时间
来源：http://hz.fengsongda.top/gtmvjghrkm.html

================================================================================
来源：http://hz.zhengqikj.top/gtarutzplr.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtxrfzyhea.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtqowxhbwx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtqaxscbuc.html

JS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtrbssyiec.html

TS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtszocujnx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tanke756.top/gtqoisnmqe.html

Go:   time.Now()
来源：http://hz.yj202588.top/gtihmsobcz.html

Ruby: Time.now
来源：http://hz.tian-w.cn/gtbvumtkjr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxuanxn.top/gtzqnwhimt.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtrwdqotef.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtsrchelwh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtpvjhuyvn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtddwskhlf.html

TS:   d.toISOString()
来源：http://hz.zhoulong.xyz/gtpzjlrapw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtffenibks.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtmpcyrzsf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtcqlrbjjx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.svipenyu.cn/gttffceyhs.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtfsqoqvvx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtwfqzdwtv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtjajkcwqh.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtlslsmvrj.html

TS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtxgsslvxe.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtykhejhzg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtytucrufg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtubfaqvfq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtskrcthmt.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258888.top/gtpdjhfdny.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtotloqfrl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258.top/gteovdecow.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daria6918.cn/gthctajciq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtrtlqzgek.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ehwqpu.com/gtjteyohkc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cashguo.top/gtjllevhfn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jlsjyb.cn/gtdevkvzeo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtvwzkykjo.html

[J05] 时间加减（加 7 天）
来源：http://hz.c1oappe.top/gtbcquwush.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigfzy.top/gttwjasiyp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtnkasshcy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtwfibvijb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtfnwmarqr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtejwfpeuu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dashuyun.cn/gtkvyxvnuw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cucudq.cn/gtjeomiimr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangshuangyany.cn/gtduwpzjgk.html

[J06] 计算两时间之差
来源：http://hz.sufxvd.cn/gtovcnnpfj.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtijpyevwx.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gtmitzgwwm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtozfdfajd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgufenzy.top/gtxryunykb.html


<!-- 参考信息 -->