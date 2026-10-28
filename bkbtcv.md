代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.snrcjt.cn/gtfeuhwpxf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnxiangtu.top/gteiuaiqbb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tian-w.cn/gthsmfcxod.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtdwnauxnl.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtmqeqibdr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtihrlccjw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtamqetomw.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtvmhqzrfl.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gttqodvmnu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yuxming.cn/gtbaizzlhl.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtufswhfxk.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtonrknetn.html

TS:   public / protected / private
来源：http://hz.jyoumei.cn/gtltzrhptq.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gtfzxzmbnq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.svipenyu.cn/gtceguzlwj.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gtqjcmkoeo.html

C#:   public / protected / private / internal
来源：http://hz.hysaishi.cn/gtkuajduhs.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtmjttzbrv.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtdfqjcgub.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtwoayrgvo.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtjcxhsegu.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gtpvybwofz.html

Java: public String getName() { return name; }
来源：http://hz.jiagoushi.top/gtcaudytjn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guowangkeji.top/gtcdxrjvzc.html

Ruby: attr_accessor :name
来源：http://hz.yongpay.top/gtiacnblwx.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258.top/gtogrfiknr.html

[G12] 对象转字符串
来源：http://hz.wangshuangyany.cn/gtflsgszey.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtimqbhllx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtxhrlxcgn.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtvxwqxhyy.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtltpvumhc.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtgglnecyu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gttneuaftq.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtbjcwtppp.html

C#:   public override string ToString() => Name;
来源：http://hz.cucudq.cn/gtvsnvuhuz.html

[G13] 判断对象类型
来源：http://hz.andypj.xyz/gtmzxqmxtc.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gtpsiiupsx.html

PHP:  $u instanceof User
来源：http://hz.quarkkingdee.top/gtynzwdmdy.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtffdfebdv.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtxztlbtsu.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtcwinjrcu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtdxxgmduk.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtzokqjcpb.html

C#:   u is User
来源：http://hz.ivvv.top/gtatijmspy.html

[G14] 数据类 / record
来源：http://hz.dashuyun.cn/gtejcaiwiw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tian-w.cn/gtdwpihwyt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtgogapdno.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zdqjudy.top/gtybmlfwpv.html

TS:   type User = { name: string; age: number };
来源：http://hz.yonumen.top/gtrqkcazry.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtsqhzfwra.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gtrgndmdja.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtxzipkdht.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gthjajdled.html

[G15] 枚举
来源：http://hz.hfpthk.cn/gttbcywxrm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shuidangran.top/gtmxdnbhjc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hywenlv.cn/gtkyrbnfyx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtogaoiaxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtlgvcoeki.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gteicgzewi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.redwolf501.top/gtbfzagjxd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtualzvwuo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtkzvfuaog.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtmpzivypp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.svipenyu.cn/gtvefdccbk.html

PHP:  get_object_vars($obj);
来源：http://hz.cucudq.cn/gtnjswqyuk.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtlrpdyppf.html

TS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtrronoksf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jyoumei.cn/gtiacttjsa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tian-w.cn/gttyemyttr.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gtuzqiawnn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gtraliybdf.html

================================================================================
来源：http://hz.nanxinkj.top/gtogsqybaq.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtekrnbgkg.html

================================================================================
来源：http://hz.jiagoushi.top/gtgoapukvb.html

[H01] try / catch 基础
来源：http://hz.zhixingplan.top/gtccdpdmca.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenzaomai.com/gtdmlmnssy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shuidangran.top/gtnsqzenhb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtsgtnpdlj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtxotfuygo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtddwmcpii.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtwlevievq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cqqwz.cn/gtnlgswqzo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtcgstttsl.html

[H02] finally / ensure 收尾
来源：http://hz.xinyue.icu/gtmegaefqj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xziqi.cn/gtxkubtamm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtegqcfpyx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtyylsbtbu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gthugxvdra.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtkoygsipi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtgmezdikk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gtchpphsok.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtaicpryic.html

[H03] 主动抛出异常
来源：http://hz.0kj1m.cn/gtbznomoog.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydzc1.top/gtaasiieqb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtgthyvosd.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtatbseeyb.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtatddyjhj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtdtofbuym.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtpuxhfvvq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daria6918.cn/gthzimhydo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtgoiynvyj.html

[H04] 自定义异常类型
来源：http://hz.jianghu66.top/gtvnzidsul.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtuqktyfpj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zycfv.cn/gtjdcedkyu.html

JS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtzpwkktpa.html

TS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtgiwhllaz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gtmfoukfci.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.svipenyu.cn/gtfqefsxpr.html

Ruby: class MyError < StandardError; end
来源：http://hz.tian-w.cn/gtdhawfsnx.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtsodouglz.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gthwhqtonq.html

Py:   except ValueError as e:
来源：http://hz.sysykeji.top/gtpjqmtpbd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ybcxt.top/gtzmqecvgc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtjeastrbs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtyonlvnoh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtneifctus.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtartfypkm.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnxiangtu.top/gttmduojbv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.vqdsnc.cn/gtpvfinjvw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtqnifsbzh.html

Py:   value = d.get("k") or default
来源：http://hz.xylfe.cn/gtaadnnwsj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xinyue.icu/gtfgqrnkjt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtnndnezui.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtpcaljilh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.52xcode.cn/gteqglstds.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtytjwvluu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tanke756.top/gtobskzssz.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangtech.top/gtwzlebgqs.html

[H07] 断言
来源：http://hz.yuanzhike.top/gthhzzgbwy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shangyingyoupin.top/gtbfngophe.html

PHP:  assert($x > 0);
来源：http://hz.tian-w.cn/gtnnyawucp.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtqbayvnyr.html

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtewpsiquq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj202588.top/gtguifhvkc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.52xcode.cn/gtyrqvgehj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtsmxqxcpj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtuppzsdeq.html

[H08] 获取错误信息与堆栈
来源：http://hz.svipenyu.cn/gtlpxetuvv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.52xcode.cn/gtzyshezln.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangshuangyany.cn/gtktchqzaf.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtppltdjry.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtlawvagwq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daria6918.cn/gtfcayrqax.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtphztjitr.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtxnveehnl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.smart0.xyz/gtmgghkido.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtdktuzuqe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gtlpmrucdk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gtjwimxtsq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtwspkesjt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtdgxkqseg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtgxxtulxn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtneevqbxs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydzc1.top/gtijzazsgp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtokbuuorg.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtlyfrvxlv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tanke756.top/gtfsdhjxus.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuetiantiany.cn/gtsxckwwex.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtxzqibzgv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gttgyugvqy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.birdmap.top/gtcxucgvzj.html

Go:   defer f.Close()
来源：http://hz.tianlin.xyz/gteceuunqt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtcdaerczk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gttnqmhelc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmyyplnvh.html

I. 正则表达式
来源：http://hz.zhiwuduotai.top/gtoywoiioz.html

================================================================================
来源：http://hz.iojbl.cn/gtshbmtlap.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gtinfxyaaq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtgmqezmae.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhaomingkeji.xyz/gthyqqqceb.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtwhtthtao.html

TS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtobjlythd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtcjhnwgpo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtzxwndicu.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtofcsnsbu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gttvdsmyfh.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gtqvsjtlrd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258.top/gthhjuorab.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.meibo888.top/gtsqnvsqkc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtmjyzuwph.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gthxkvygir.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gtctbccfpb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gaohongyu789.top/gtzxfgfyke.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtlnyxbgsl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtovhhmnsx.html

[I03] 提取捕获分组
来源：http://hz.ydjk.org.cn/gtilsfgkis.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtuttppzqe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hywenlv.cn/gtitpepsft.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtnidzpyyu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtzwjhfybe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtxkbnrorp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangtech.top/gtzshotwzp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.bjfxy.top/gtgvgznhrs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hfpthk.cn/gtnxslzsmu.html

[I04] 正则替换
来源：http://hz.jinyuanbaomall.cn/gtvqlvwrlj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ehwqpu.com/gtpjhyopju.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhijiandao.cn/gtulryzqjg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.c1oappe.top/gtciupmnzb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtttqifusn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.quarkkingdee.top/gtfkdilchq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinqigufen.top/gtuveigymu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gteunbtwsf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dianchejie.cn/gtctvxibcf.html

[I05] 按正则拆分
来源：http://hz.ehwqpu.com/gtljwzjapq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhaomingkeji.xyz/gthepsqjbf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xziqi.cn/gtcbolauuu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtxyubpbxf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtvewolooy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cqqwz.cn/gtybywwysf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinghuilouyu.cn/gtqlinkdcq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtiuchxtrb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.c1oappe.top/gterzbkkon.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtupijvjjs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gttfgqaedz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinqigfzy.top/gtzqzjkndv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gthdgnkaek.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtllhfuuvc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xziqi.cn/gteztwqfly.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtafjqruru.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtrugeranb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtrrjgyyyp.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhengqikj.top/gtkcwvyavw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gthbxkgryz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtuarfubdu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtqexeuzzd.html

TS:   /error/gim
来源：http://hz.jinqigfzy.top/gtguafmglg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtfcnvcbxu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pengpengdd.cyou/gtwucddcfh.html

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gteierpnmh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gzhubu.top/gtfmmhpmgg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtsajorife.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtyretbifu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.meibo888.top/gtnumhzgpf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtujvcapho.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtvkbaqjjy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.havefunace.top/gtfousfgoa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtbuqzbqfa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gteulpaisk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.andypj.xyz/gtztabyanf.html

================================================================================
来源：http://hz.jianghu66.top/gtcxeffbnk.html

J. 日期与时间
来源：http://hz.ppjwa.cn/gtenmuivcl.html

================================================================================
来源：http://hz.iojbl.cn/gtoasezpre.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangkeji.top/gtypxmjnxm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtegqivaim.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtjvzinapg.html

JS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gthhkhuijt.html

TS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtofgmnmoc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtxedvpide.html

Go:   time.Now()
来源：http://hz.redwolf501.top/gtqzvvmauy.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtrjpgdpoy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guowangkeji.top/gtcszdsckl.html

[J02] 格式化输出
来源：http://hz.shangyingyoupin.top/gtxdwycfhc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtvapnbvfm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtkatnvzog.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtnupqryaq.html

TS:   d.toISOString()
来源：http://hz.andypj.xyz/gtgqflxdoq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtaibgcyau.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtxkwvjfbk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtopmnqdvf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gtrxequqiq.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtzhezmozl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtbyempwgp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtuspmszrk.html

JS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtbynijukg.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtuarosbkh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtjtorawpo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xziqi.cn/gtrjsostry.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtqrekuwvs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.iojbl.cn/gtosphkutt.html

[J04] 时间戳与日期互转
来源：http://hz.vqdsnc.cn/gtuzgtpbqp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gtbjocxxlr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tanke756.top/gttrmmhdkw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtteuzqudt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangkeji.top/gtrcbxgnrn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtirtqltck.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenzaomai.com/gtrvuhekbz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.bjfxy.top/gtrzeylxtt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtxbaahuyq.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtgqsimevo.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtypmgmmjx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtpcvtrewu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtytaetxig.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtsrmpmdht.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtzdofrwqg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pengpengdd.cyou/gtznlmkwfv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gtlqervuft.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nwbrower.top/gtgjysesgt.html

[J06] 计算两时间之差
来源：http://hz.birdmap.top/gtefnhtyhn.html

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gtfjljsnor.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuanzx.com/gtcqjeqxyl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gtpfqtebwh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtzknycokr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.feifeiyinyue.top/gtqhnzgrpp.html

Go:   end.Sub(start).Hours()
来源：http://hz.iojbl.cn/gtwthxmxwm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ivvv.top/gtadawivhe.html

C#:   (end - start).TotalSeconds
来源：http://hz.quarkkingdee.top/gtgcgffmgw.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gtwbpmewjz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtqndbsyxg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtekdnwxqy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtydmqjqvb.html


<!-- 参考信息 -->