代发 wailian999

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gtowgunyuw.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gttrqztevw.html

TS:   static f(): void {}
来源：http://hz.gogol.net.cn/gtczstzupj.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtzwccdhvp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ehwqpu.com/gtfraxynfl.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtmlbodgcb.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtoyzlzyql.html

[G09] 接口 / 抽象类
来源：http://hz.daxiang520.top/gttnwvrveo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cucudq.cn/gtmroquerm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtrttyjpxz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtaosuurhw.html

TS:   interface Shape { area(): number; }
来源：http://hz.cashguo.top/gteykigifw.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gtevpvnohd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtovdvwitl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxinkj.top/gtyzzuvshs.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtrzdbzalo.html

[G10] 访问控制
来源：http://hz.yueranfly.top/gtnesmqruq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtatdrvukl.html

PHP:  public / protected / private
来源：http://hz.guannengcc.top/gtobpeidwh.html

JS:   #private 字段；其余公开
来源：http://hz.fzhhl.top/gtmjbhlgez.html

TS:   public / protected / private
来源：http://hz.gogol.net.cn/gtohcoaryi.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gtgviovxkd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtasstrqsk.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtjjvzjbji.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gtdblwhvvo.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtveulmekv.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtosclnfcv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtsvnpvvsp.html

JS:   get name() { return this._name; }
来源：http://hz.dashuyun.cn/gtstzpkycu.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gtwcplcayz.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtbxidodja.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtptbzlyfe.html

Ruby: attr_accessor :name
来源：http://hz.yj20258888.top/gtrijrlznn.html

C#:   public string Name { get; set; }
来源：http://hz.quarkkingdee.top/gtoytkjmlz.html

[G12] 对象转字符串
来源：http://hz.wangdashe.top/gtcwphuedq.html

Py:   def __str__(self): return self.name
来源：http://hz.hammf.cn/gtsstxlyxy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtyztrjlqr.html

JS:   toString() { return this.name; }
来源：http://hz.hnqzz.top/gtvihvobrs.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtjoavrwpr.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gthyljfceo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtvvmrfuzt.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gthzdhoopo.html

C#:   public override string ToString() => Name;
来源：http://hz.sysykeji.top/gttrazgsxq.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gthztlkcwo.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtptqayocn.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtotfvuscp.html

JS:   u instanceof User
来源：http://hz.sufxvd.cn/gtnqljonmv.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtglkerhvl.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtuqproatj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtgpwyfrlu.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtbbxaunji.html

C#:   u is User
来源：http://hz.aibaodan.cn/gtkfocaecz.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtorisuthk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigufen.top/gtzwhbxhje.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gtqjjcxmtz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtjtmhidaf.html

TS:   type User = { name: string; age: number };
来源：http://hz.svipenyu.cn/gtrbhdxuep.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtifptfhsi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuetiantiany.cn/gtqakhodov.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtjdsszwab.html

C#:   record User(string Name, int Age);
来源：http://hz.0kj1m.cn/gtjimyepyr.html

[G15] 枚举
来源：http://hz.yongpay.top/gtzhtmljmo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtguhwqvff.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinyuanbaomall.cn/gtakezlhir.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtuowaadiy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtxxxifkcc.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtizrcwldp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.snrcjt.cn/gtjmqnrjxf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gtqkujrppw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtfahwcvju.html

[G16] 对象转数组 / 字典
来源：http://hz.cheryme.top/gtssyncmdu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hysaishi.cn/gteeryrihm.html

PHP:  get_object_vars($obj);
来源：http://hz.hnxiangtu.top/gtxywkesdz.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gthvgkfcnm.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtfajofuwu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtnqhxblkd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zycfv.cn/gtqxmpqrrk.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtosxblgev.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtdddjvrvx.html

================================================================================
来源：http://hz.9152youxi.cn/gtskeugfvc.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtvwzaroho.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtujlmpbyk.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtflybtvug.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gtgtwvekub.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gotoacloud.top/gtqokiaukv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtwkcemjtk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gteenwlnwb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sufxvd.cn/gtbzoplesz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtnretzscq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtwppaoflq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ybcxt.top/gtycxcquyv.html

[H02] finally / ensure 收尾
来源：http://hz.jyoumei.cn/gtqdrtvkwl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shangyingyoupin.top/gtgkoqisch.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtitbphpfr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtnlidtlmp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtkhfnpiik.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtxqhwlrka.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtxoizvgpj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gteaiqmwue.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtngxdvxlk.html

[H03] 主动抛出异常
来源：http://hz.tianlin.xyz/gtnysbywnn.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtxflzooem.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gteougqkvc.html

JS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gteedhdfkw.html

TS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtqidkhqqw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtplbwectx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gthgfhwyjc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj202588.top/gtukxyplhk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtdjichiom.html

[H04] 自定义异常类型
来源：http://hz.jqgufenzy.top/gtvjxrztdm.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gtihxewqcd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtixilacqa.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtntaqraxs.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtppaelyso.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtbblmpxep.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtfjoyhryx.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtgblsnxzw.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtgfwpmkom.html

[H05] 捕获特定类型
来源：http://hz.xingfuxueyuan.xyz/gtmpaishkl.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtccrygocn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtifdyfgnr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtrkdoqind.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtcdhoclld.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.svipenyu.cn/gtylvkeeyw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gtlfmyaztr.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtnplcpzjn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhengqikj.top/gtzvfwhmuh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gtwcxbaocz.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258888.top/gtpvfyrspm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtwdrudcrb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtekdurlfx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gteultysjw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cheryme.top/gtknavjjfa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xingfuxueyuan.xyz/gtrbgnayhh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gtctpuvcfp.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtotugwigx.html

[H07] 断言
来源：http://hz.shuidangran.top/gteunydstc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtxpidgfwr.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtwoowjuso.html

JS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtkxexromn.html

TS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gtjfdrcyfe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gthwwllzmh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtyfmhmbwg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtetfgpork.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gtgjiedtzj.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtwbuxfpvw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gtfpagporv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gthqqskpmj.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtwocsfejq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sufxvd.cn/gtuoepqmzo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gttftsymmg.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtqtmodjdt.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtkzbagrml.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtobyzmukj.html

[H09] 带错误码的异常
来源：http://hz.jinyuanbaomall.cn/gtprxblbjq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigufen.top/gtkwdwktyo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtrruvxwdl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yueranfly.top/gtlwujzupt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtelgjnpsp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.smart0.xyz/gtqwognmei.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenlongwang.top/gtplvklunx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jiagoushi.top/gtbnoudgts.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtjscqyeye.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtkgzradcr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gtccmurgbw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gtxpnlyctn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtdkqmyaca.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtqmpyoxjl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtvoalhtkq.html

Go:   defer f.Close()
来源：http://hz.yuanzhike.top/gtgwonaqlo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigufen.top/gtcdxggghz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtfwmrbxcm.html

================================================================================
来源：http://hz.wangdashe.top/gtqjwmuxfn.html

I. 正则表达式
来源：http://hz.pengpengdd.cyou/gtlpynyenf.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmzbomyev.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gttdfcxzhv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtsvljmoua.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxuanxn.top/gthkzpkdoc.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtvolruimq.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtsbmwujrc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.316326.xyz/gtinzgzxxe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtjfkhcdwy.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtylzmcdgp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hywenlv.cn/gtcqqppjzi.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtegufuuvl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gttgrwzkux.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cdnleiting.top/gtxbzfminu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tian-w.cn/gtreujgrui.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtqonrfaok.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtqlkabyfa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dashuyun.cn/gtyytlonzn.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtiaubsfja.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtcgnuhddv.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gttxkyladh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zdqjudy.top/gtpluuqfqh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gticntxveq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yvedp.cn/gtvqidvxgf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuanzhike.top/gtipsruxgt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cashguo.top/gtojpwnzds.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtnhddhdxw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtmmbgxqou.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258.top/gtwfqokuwp.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gthceldxau.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhaomingkeji.xyz/gtedhgoddq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtnlfwsczv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtpbnhyhqe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtxhkkecvc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.bjfxy.top/gtwarwjisg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.vqdsnc.cn/gtbssewygp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gtqgjjcgff.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtxzwlmdhn.html

[I05] 按正则拆分
来源：http://hz.andypj.xyz/gtwmywtzzs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtxpbjzwpg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxuanxn.top/gtfhdndeml.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtmyynqote.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtassjjmqr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ehwqpu.com/gtebxdmsrj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gogol.net.cn/gtvcxpwhik.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtwjwblaqp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtijptqbhx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtfmcvdesi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtwneiktyo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cashguo.top/gtpxnsgwfx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.0kj1m.cn/gtkdeqftgy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtfoszmblo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gaohongyu789.top/gtukdzwckj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtopquylpq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydjk.org.cn/gtgeswmbca.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtfksijhvn.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgfzy.top/gtgmxtwkwt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sweek.top/gtdqycpcas.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxinkj.top/gtpwhirnjf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gtjhjilguu.html

TS:   /error/gim
来源：http://hz.cashguo.top/gtqxviokmz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtfooxwloe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gtzjjyiqwr.html

Ruby: s.scan(/error/i)
来源：http://hz.hfpthk.cn/gteglaiduf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtkcgyareg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.haohaochexian.top/gtnysmktsa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.316326.xyz/gtyovopnfn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dianchejie.cn/gtxzlihweo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtsjlyznww.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtfclvrayy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gtcoztqruv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pengpengdd.cyou/gtbwndingz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtahfkhpjf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gtzswrsoda.html

================================================================================
来源：http://hz.sweek.top/gtlfjtacbg.html

J. 日期与时间
来源：http://hz.hfpthk.cn/gtxyxntqxo.html

================================================================================
来源：http://hz.yj20258888.top/gtxkppcpml.html

[J01] 获取当前时间
来源：http://hz.zhijiandao.cn/gtcieypqdt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.9152youxi.cn/gthgxlvlrt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtpiqtxhdv.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtueenulqh.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtdmyzybgs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.havefunace.top/gtuhzjljgw.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtkyqjcdzm.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtvxjzhlga.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigfzy.top/gtjwnoxuti.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtnippyrls.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gttdmdurmm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtkviggnzc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtmziuyxkf.html

TS:   d.toISOString()
来源：http://hz.chenjidiqi.icu/gtkzjibeqg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtwubjcfjd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtaetflshw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtasmpyebf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gotoacloud.top/gtysafxgwi.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtqzoirvol.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yangfankeji.com/gtraohctec.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yonumen.top/gtkzojglaj.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtnqtxwqyz.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtcuzbqcda.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtiyfhziqj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yongpay.top/gthwktunhn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtqwzpeyfg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtkugjjvyf.html

[J04] 时间戳与日期互转
来源：http://hz.gotoacloud.top/gtjhxfjauk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daxiang520.top/gtvtnwhrnm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtjcgdxzxj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnxiangtu.top/gtoqoencpe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtqjoixvtf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuanzhike.top/gtyfsqzzwx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtnnnmdsdz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daria6918.cn/gtpeessdka.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtbecftcbz.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangdashe.top/gtmtplhzjs.html

Py:   now + timedelta(days=7)
来源：http://hz.nwbrower.top/gtwnrwtcny.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtcnepmnil.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtympmhqdv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtyzkpwsua.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yanxiufei.cn/gtqjacldlf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jlsjyb.cn/gtdvhiufva.html

Ruby: Time.now + 7 * 86400
来源：http://hz.316326.xyz/gttutisgnx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gtsnrvttuu.html

[J06] 计算两时间之差
来源：http://hz.gogol.net.cn/gtncshccgu.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gteipctcpe.html

PHP:  $end->diff($start)->days;
来源：http://hz.guannengcc.top/gtoselieiu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtkdyktilv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuanzx.com/gteonnlhmq.html


<!-- 参考信息 -->