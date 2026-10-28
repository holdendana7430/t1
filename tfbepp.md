代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtaggdfrpa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtgmmnltqe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtrubjgavb.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtmihhhojv.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtbgbaxwyn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gtwwbwemfa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtgombxbqh.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhijiandao.cn/gtnaonovvk.html

[G10] 访问控制
来源：http://hz.yj20258.top/gtkkxmxrgz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cashguo.top/gtzdgbvyvg.html

PHP:  public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtdyotrubu.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtzxidvizl.html

TS:   public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtuucuuhpv.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gtksrhogsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cdnleiting.top/gterobbvcc.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtbrbsmkxx.html

C#:   public / protected / private / internal
来源：http://hz.aibaodan.cn/gtbapifuhn.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtogjazqfp.html

Py:   @property 与 @x.setter
来源：http://hz.yonumen.top/gtentomacs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtdxgdonua.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtfyjcowfs.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtqaqqthnq.html

Java: public String getName() { return name; }
来源：http://hz.ydzc1.top/gtouyheutj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtkcodgiaf.html

Ruby: attr_accessor :name
来源：http://hz.zhoulong.xyz/gthrnsvrdo.html

C#:   public string Name { get; set; }
来源：http://hz.fzhhl.top/gtgpqpulzc.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtejxjwlfk.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gthacjyhaw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtceeccyhx.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtjjlamjil.html

TS:   toString(): string { return this.name; }
来源：http://hz.fengsongda.top/gtkunzurnx.html

Java: @Override public String toString() { return name; }
来源：http://hz.xziqi.cn/gtldrmcxfk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gtxaphqyxs.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtjsgqaydz.html

C#:   public override string ToString() => Name;
来源：http://hz.pengpengdd.cyou/gttseqgnnv.html

[G13] 判断对象类型
来源：http://hz.shzxlz.cn/gtepihlxsq.html

Py:   isinstance(u, User)
来源：http://hz.c1oappe.top/gtlammgude.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtrvyoipgx.html

JS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtjgshozdv.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtifpttgtw.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtjkmlrhlm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pengpengdd.cyou/gtkecwkpsp.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtrrdxhyfi.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtzuirsers.html

[G14] 数据类 / record
来源：http://hz.9152youxi.cn/gtwssmtdhw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hammf.cn/gtehggvoox.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xziqi.cn/gtzxdufvrp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guannengcc.top/gtkkzjqkhd.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtybkcigli.html

Java: record User(String name, int age) {}
来源：http://hz.zhixingplan.top/gtgfdzyhyv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydzc1.top/gtsurcpwnp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gttpprcuel.html

C#:   record User(string Name, int Age);
来源：http://hz.xuetiantiany.cn/gtnlyqgfht.html

[G15] 枚举
来源：http://hz.ydjk.org.cn/gtrelpsihs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cucudq.cn/gtuyzusqxp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gtloxbmgra.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtwzunmmsr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtyhfcqggm.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinghuilouyu.cn/gtmztlxori.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jianghu66.top/gtltuagknc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dianchejie.cn/gtpvgrxcoi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtmqcjwilu.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtimyovnps.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gtzfetpgku.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtggjoyzme.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtbqtpnzkp.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtxvtoddrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hfpthk.cn/gtpqkkchqb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gttkpcjpwa.html

Ruby: obj.instance_variables
来源：http://hz.hysaishi.cn/gttdoimjwc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtwwkkbtbb.html

================================================================================
来源：http://hz.xziqi.cn/gtjzvkhfck.html

H. 异常与错误处理
来源：http://hz.zhixingplan.top/gthegdpgse.html

================================================================================
来源：http://hz.cucudq.cn/gthzvljlro.html

[H01] try / catch 基础
来源：http://hz.vqdsnc.cn/gtfvstwyey.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.c1oappe.top/gtdogclrhg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gotoacloud.top/gtmaebjtjo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgufenzy.top/gthquzoluo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtjugdharo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aizwys.cn/gtkotuuzbz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtmgwqxqsc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtnzexiaag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigfzy.top/gtqssijziw.html

[H02] finally / ensure 收尾
来源：http://hz.nwbrower.top/gtibwggmlj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtmghztlmw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtnzpsuuoh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtqvoyjtdt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtpdwjxyto.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtbasmbjjp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.316326.xyz/gtvwtoouec.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtpaxqotia.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtsjwgrtnv.html

[H03] 主动抛出异常
来源：http://hz.ywan-chungtsiang.top/gtptpbzkog.html

Py:   raise ValueError("错误信息")
来源：http://hz.redwolf501.top/gtqdlqtthj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtuhdbirmf.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gthvqjqrss.html

TS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtweabbghq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtauqmvmfy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtzqkwfsbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xziqi.cn/gthwagfuac.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtxirerhkl.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtsrzeyogi.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtalspvlci.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtxewvujtz.html

JS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtumwslzzi.html

TS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtqjhwkpbj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtpcjpdwin.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.mhx1999.top/gtsunpxwxc.html

Ruby: class MyError < StandardError; end
来源：http://hz.tianlin.xyz/gtbwkevuvb.html

C#:   class MyException : Exception {}
来源：http://hz.yuxming.cn/gtffmjmfow.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gtuvucfdkc.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gtltlbgfda.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtdbqurlqm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtaylldloc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtnhkqdkos.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gtbljrmhht.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.svipenyu.cn/gtjtluyeof.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtdhdwwdhn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ywan-chungtsiang.top/gtoxgswish.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gtooyqldhx.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtmloshiwm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gzhubu.top/gtsdsexzpj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtlcnmktjd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtdvwqaogd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sysykeji.top/gtyxwfgmha.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gthlhuqgry.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gttmwwchaa.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtoxdfciqv.html

[H07] 断言
来源：http://hz.ydzc1.top/gtrsucracw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtoqlajrbu.html

PHP:  assert($x > 0);
来源：http://hz.hongshengwenyu.top/gtojgkljid.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtnosytycs.html

TS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtvgsmkuow.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ywan-chungtsiang.top/gtabgqerkw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gtlexnhcoh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtxhdwrglq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tianlin.xyz/gtqqywcudt.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtfunwleux.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ehwqpu.com/gttwaluekj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtomytuubq.html

JS:   e.message;  e.stack
来源：http://hz.jqgfzy.top/gtainygudt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gttwwdnzmp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtxdfiitiz.html

Go:   err.Error()
来源：http://hz.pycfn.com/gthaatovox.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtitzpxbwo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinyuanbaomall.cn/gtzpvoydzk.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gtpyktznpk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gtuodomhvk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dashuyun.cn/gtbdzznwtl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtlchltlnj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhijiandao.cn/gtvbylzxck.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ybcxt.top/gterwhkhjw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtshyjjtqh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhongyouzk.top/gtfijxoljb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zdqjudy.top/gtaqdrvttz.html

[H10] 资源自动释放
来源：http://hz.yj20258.top/gtsivhagbp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtrgvciazk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cashguo.top/gtehxlqlcu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtfanmjkgo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtcucphtao.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnqzz.top/gtefsvvdyg.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtitxiasmz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhiwuduotai.top/gtylfisgaw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtjjortslp.html

================================================================================
来源：http://hz.nanxinkj.top/gtpnkgjxba.html

I. 正则表达式
来源：http://hz.meibo888.top/gtonrujqzs.html

================================================================================
来源：http://hz.hfpthk.cn/gtsfrgccpg.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtmqutyldj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtuxptdicj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtgyiuudmf.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtrysaenld.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtserifesq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtzokpebuh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aibaodan.cn/gtfkzrzmij.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtfbjhamke.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtpkxqtjjf.html

[I02] 提取所有匹配
来源：http://hz.snrcjt.cn/gtmpoxeivb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtiddnfoal.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shangyingyoupin.top/gtqwyptmha.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtxwhdnzen.html

TS:   s.match(/\d+/g)
来源：http://hz.chenjidiqi.icu/gtetnqankg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sysykeji.top/gtbckstztw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtxdzojjdp.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigufen.top/gtjxkwywau.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yueranfly.top/gtunlbdpma.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtittqacxf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gtufqdzfys.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtmossoojx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xinyue.icu/gtjlkyjhkr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtnjxprnmz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nwbrower.top/gtxwhqzhpb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.52xcode.cn/gtsguuwmps.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jiagoushi.top/gtmginivrb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daxiang520.top/gtszqgwuqa.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtygaozilj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtgkzvttda.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtvrxiiwxi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtobafhqvu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtlscovxnd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtqfrkdcch.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtnwezcsnf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtiuvjzasl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtuggtasfe.html

[I05] 按正则拆分
来源：http://hz.daxiang520.top/gtwcktnqcl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhiwuduotai.top/gtlbkgrpfx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtklcyuiyv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtjzcqlffk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtgwebzohv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.pycfn.com/gtiiudzfbz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gtezusgcoo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtwvtkkteo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gtogecylbt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtdohmxjcn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.haohaochexian.top/gtfekpanmk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258888.top/gtkpsynbls.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtjpkgfsdr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtmsxszjce.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhengqikj.top/gtifzwrkgy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ppjwa.cn/gtfidpwunj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gttnvjoudb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtpsasuzcu.html

[I07] 忽略大小写与多行模式
来源：http://hz.52xcode.cn/gtjnzaqqjq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtpftqbnil.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cqqwz.cn/gtyzhqftlv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigfzy.top/gtqiahtobx.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtnyfivsjv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tanke756.top/gtwccvyqvx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuetiantiany.cn/gtyusprppl.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gtjwynhklj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtdgkeperj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtqbsceuli.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtbodgrrxo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.mhx1999.top/gturhjilwe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtvbvcudsb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtvhzwphid.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtovpznlzs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtxofxsjip.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhongyouzk.top/gtzgemwsyw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtgtlvirev.html

================================================================================
来源：http://hz.tianlin.xyz/gtyyymvrpg.html

J. 日期与时间
来源：http://hz.wangdashe.top/gtlxxmzsqb.html

================================================================================
来源：http://hz.c1oappe.top/gtbhtbjbio.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtlmszjyxs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtdwtcolbn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtpchwypum.html

JS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gtjowscfkl.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtebgrlfel.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtwamolcoy.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtfomcfmpu.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtsgcxcmjm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtogjzjypr.html

[J02] 格式化输出
来源：http://hz.hammf.cn/gtscscdmlp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gthgdnfhrf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gthnbqqssa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtjihsqmhm.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gtsdetgndf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhengqikj.top/gtjgmrvfmw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj202588.top/gtafqjrklx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtbvmkyhqe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtzikwtruj.html

[J03] 字符串解析为日期
来源：http://hz.xuanzx.com/gtctwlyydf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuetiantiany.cn/gtggqfytmi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtqhxwevgt.html

JS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtcbjcyldj.html

TS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtojrlzwjl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtzhnbllmb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ivvv.top/gtawdkzffs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtfmcpqlxi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.haohaochexian.top/gtpgevmjch.html

[J04] 时间戳与日期互转
来源：http://hz.bjfxy.top/gtnsbmbpsr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtgnfwhmcz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shuidangran.top/gteysgesmd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtmmzklpxg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtxtblgqef.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gtxwlilmye.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtrjrxahof.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.c1oappe.top/gtbjvlfuai.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydjk.org.cn/gtthffmnhb.html

[J05] 时间加减（加 7 天）
来源：http://hz.jyoumei.cn/gtumrfjvrz.html

Py:   now + timedelta(days=7)
来源：http://hz.yangfankeji.com/gtmemwbwow.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangshuangyany.cn/gtmgyvlcup.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtbfbdfrcl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtrbbkfcif.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtfpezfzew.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtlxazawaj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hfpthk.cn/gtgmpsbguy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.smart0.xyz/gtwvabsvlw.html

[J06] 计算两时间之差
来源：http://hz.ppjwa.cn/gteiprmcra.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtdebfqzsh.html

PHP:  $end->diff($start)->days;
来源：http://hz.hywenlv.cn/gtkrwfivsz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtcqbpnkgn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daxiang520.top/gtroxngwmp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangtech.top/gtdcqpipma.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtvbcfgczs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtygrafxnl.html

C#:   (end - start).TotalSeconds
来源：http://hz.ppjwa.cn/gtanwzsafv.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gtoudwergi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtejfjsexn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gtbewnwbia.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtvrhafcwr.html


<!-- 参考信息 -->