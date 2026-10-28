代发 wailian999

Ruby: super
来源：http://hz.hammf.cn/gtzybqyuox.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gthlremgrt.html

[G08] 静态方法与属性
来源：http://hz.cucudq.cn/gtgzxxyzzh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.9152youxi.cn/gtaucafrwb.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gttcdrolef.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gtzynkccft.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtcgjgpnez.html

Java: static void f() {}
来源：http://hz.aibaodan.cn/gtmageedpa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhoulong.xyz/gtmhsguwme.html

Ruby: def self.f; end
来源：http://hz.zhixingplan.top/gtdbqjeyzh.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtyrpjgiwl.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtadvjbxeu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgufenzy.top/gtayiosqxq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cqqwz.cn/gtbfiowzpr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.52xcode.cn/gtsvmbgpdw.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gtgvqjklgl.html

Java: interface Shape { double area(); }
来源：http://hz.zhengqikj.top/gtnvzscbfy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtudqxuyvr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtokadsjjb.html

C#:   interface IShape { double Area(); }
来源：http://hz.ivvv.top/gtatpzxjdo.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtkikjfdpa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gtarstqdsh.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gtuevoaxxa.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gttfokhytm.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtpyzakglk.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258.top/gtdchbaqfu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtdcrtxxwk.html

Ruby: public / protected / private
来源：http://hz.ybcxt.top/gtnaufttfh.html

C#:   public / protected / private / internal
来源：http://hz.shuidangran.top/gtpfvlcnhc.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtuxlwsztq.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtgxgpeslq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtvaqnuskn.html

JS:   get name() { return this._name; }
来源：http://hz.vqdsnc.cn/gtplzmbioj.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtrbjbkquh.html

Java: public String getName() { return name; }
来源：http://hz.zhiwuduotai.top/gtipuxxskw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daxiang520.top/gtbvbbtjoi.html

Ruby: attr_accessor :name
来源：http://hz.wangshuangyany.cn/gtienytmbw.html

C#:   public string Name { get; set; }
来源：http://hz.gotoacloud.top/gtmtgpusgl.html

[G12] 对象转字符串
来源：http://hz.kuanghao11.cn/gtkfmiwojg.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtxdedgyxo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtqlzbwqlu.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtnhesxnmm.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtkbgnwcij.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtjbcddmsp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sysykeji.top/gtqghycyay.html

Ruby: def to_s; @name; end
来源：http://hz.zhengqikj.top/gtpjuixdoq.html

C#:   public override string ToString() => Name;
来源：http://hz.yangfankeji.com/gtzfkschsv.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtbqkkuowx.html

Py:   isinstance(u, User)
来源：http://hz.chenlongwang.top/gtxlxioosk.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtvmtgbrae.html

JS:   u instanceof User
来源：http://hz.wangdashe.top/gtvzhvbnii.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtytbhrlza.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtslfbiotw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gotoacloud.top/gtadadvsqa.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtumuaaspg.html

C#:   u is User
来源：http://hz.ppjwa.cn/gtnkvcblmn.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtthgzpdng.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhengqikj.top/gtjjcyehso.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.snrcjt.cn/gtkoyhkjgg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gtiudshddr.html

TS:   type User = { name: string; age: number };
来源：http://hz.iojbl.cn/gtcudiuaiv.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gtydduqsrq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nwbrower.top/gtwydgymyq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ywan-chungtsiang.top/gtsnnhulkr.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtsmsiyaeu.html

[G15] 枚举
来源：http://hz.ydjk.org.cn/gtpwpsmuld.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shangyingyoupin.top/gtrnktncni.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gtsvjmxpas.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigfzy.top/gtdjjkuwjx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtlucuchkt.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtjdkcpffh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtmhpwpjnx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtknsugrgu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtpgcmnqda.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtyfoxdpjr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hywenlv.cn/gthvafihxp.html

PHP:  get_object_vars($obj);
来源：http://hz.zhongyouzk.top/gtlvfeuxyc.html

JS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtdnwsbqzf.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtptvlcoes.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.9152youxi.cn/gtexcqwpjd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtvxvdncdn.html

Ruby: obj.instance_variables
来源：http://hz.jlsjyb.cn/gtnymffnlc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtkxafdbss.html

================================================================================
来源：http://hz.hnqzz.top/gteeezzxkw.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtnsrhtpgk.html

================================================================================
来源：http://hz.zycfv.cn/gtdhdvizvj.html

[H01] try / catch 基础
来源：http://hz.gaohongyu789.top/gtyuzygndu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.kuanghao11.cn/gtibqndpfk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nwbrower.top/gtiwwzqlvk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtpreugddi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtiygyuepe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuetiantiany.cn/gtqkilmofl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtzntgbvob.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtcmwrcqfg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtabyowlsr.html

[H02] finally / ensure 收尾
来源：http://hz.gaohongyu789.top/gtkkpvlsmd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtguqtjyfc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gttnogliqu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtpkqdqnmh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtkooonquz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtmqkznfwk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtkkitcgic.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gtvyioxfwa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.c1oappe.top/gtsynvibyj.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtrqqjcxmk.html

Py:   raise ValueError("错误信息")
来源：http://hz.aizwys.cn/gtqjzpkild.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtjomnzigu.html

JS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtjwmmztsf.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gthclebbcp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtazhqagvf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yvedp.cn/gtlhlmpvsa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xingfuxueyuan.xyz/gtqzwezlyi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtzzbnctjy.html

[H04] 自定义异常类型
来源：http://hz.wangshuangyany.cn/gtfpwbvkjx.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtxirmtlpo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtioxptqdv.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtykjwowll.html

TS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtxegjmdyt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gthpkjjayo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.redwolf501.top/gtwvcjcajv.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gtbotkepsm.html

C#:   class MyException : Exception {}
来源：http://hz.hongshengwenyu.top/gtideucluu.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtsdjbqjci.html

Py:   except ValueError as e:
来源：http://hz.tanke756.top/gtsdhhmnry.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.316326.xyz/gtkyyfdnhb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guowangkeji.top/gtpffnwfpc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtaqnjioyl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daria6918.cn/gtvqaohybg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ppjwa.cn/gtunxgnsrw.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtegnbkmzj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.316326.xyz/gtpgyftufc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gtuijpsrpk.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gtnhloykit.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gtqchdoraf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtuclclaec.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtsmdmidwn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hongshengwenyu.top/gtvsafbyzu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtdwhgggvb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ywan-chungtsiang.top/gtusfsuyhq.html

C#:   obj?.A?.B ?? default
来源：http://hz.haohaochexian.top/gtmazvpqap.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtqjnnpehc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtaojgvuxz.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtlxjlsvuw.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtywwnpois.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtegpsvmuj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnxiangtu.top/gtvgndpwts.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gttchbtpyj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ybcxt.top/gtsnxpgavp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtbtspoqzk.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtayocitfa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenlongwang.top/gtofvfocxy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtzzmgkwal.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gtbvbelaga.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgfzy.top/gtwpqdndkv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtmlyybxsb.html

Go:   err.Error()
来源：http://hz.andypj.xyz/gtliviismu.html

Ruby: e.message;  e.backtrace
来源：http://hz.cqqwz.cn/gtkueyrxwn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtmhsoawsi.html

[H09] 带错误码的异常
来源：http://hz.guannengcc.top/gtxaqspipp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtuodqxsla.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gogol.net.cn/gtnivuwqbr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gzhubu.top/gtebldbdtc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtjiozahkg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhixingplan.top/gtxyewqbgn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtelvxbjmh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xziqi.cn/gtmxhryqaw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.bjfxy.top/gtbboiuxyl.html

[H10] 资源自动释放
来源：http://hz.pengpengdd.cyou/gtyucxlkfs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ppjwa.cn/gtbwoovihf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtfsdldvca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtedeyoanf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtbtkryvns.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yangfankeji.com/gtlapjxpkq.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtfdcqillz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtceittkbr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtdklvmlcg.html

================================================================================
来源：http://hz.mhx1999.top/gttifciqul.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gtsdkdpupc.html

================================================================================
来源：http://hz.sxryk.cn/gtwvpqrwmk.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtmertwcao.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtordobioj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sufxvd.cn/gtslzqbqgu.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtycwjiwkq.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtdmsmrqyy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gtkphgphek.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtmbxefvui.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtoaodwlbl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cucudq.cn/gtflncjngt.html

[I02] 提取所有匹配
来源：http://hz.gaohongyu789.top/gtnoynvwfp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gtpwgjdgtk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtqvqmkhph.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gtegfvuyhx.html

TS:   s.match(/\d+/g)
来源：http://hz.yangfankeji.com/gtmyijqflq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gtjviymcbd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnxiangtu.top/gtewkbljop.html

Ruby: s.scan(/\d+/)
来源：http://hz.jlsjyb.cn/gthpwoffbq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtxicyhhgo.html

[I03] 提取捕获分组
来源：http://hz.aibaodan.cn/gtdwjmynnp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gteonwxjzw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.smart0.xyz/gtsvrbsbre.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuanzhike.top/gtjdhhkrzh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinyuanbaomall.cn/gtgrrnwzax.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtpozuxgod.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtxysjwayy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtgotxhvzb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.snrcjt.cn/gttyzelzbr.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtijssceap.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gtkphzwhvx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gthlkiwkzb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtcutidhmz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtcbyefxde.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gtijldquzt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtbvqhtyle.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gteqotefwn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj202588.top/gtrpipnfup.html

[I05] 按正则拆分
来源：http://hz.jinghuilouyu.cn/gtfixmbrke.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yangfankeji.com/gtgyxpdhdb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtdcidkczj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtbmjofbhl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtpjfaubxj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtkobandig.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gogol.net.cn/gtkqspqcdv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtqitwrrgt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gtsxdrcihy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtinaliwpq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtfrrblcxr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtlkrtjzkj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtarivogdk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtapuilqzm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daria6918.cn/gtdoxyiexk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hammf.cn/gtxhyfxfpe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtgivzjrjl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtnxwhpqgg.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtyzmulanb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtlzhwwazg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtxfubaiet.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtioahqvmc.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gtesguhslp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtczqlqcyu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gtxssljcur.html

Ruby: s.scan(/error/i)
来源：http://hz.vqdsnc.cn/gtiridqjgw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hongshengwenyu.top/gtyibicgmw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtphadunjm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenzaomai.com/gttinymrmb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.0kj1m.cn/gtyxtlfbsr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtjjzwfgnv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtusqihuze.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtsvekjicy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtkscjqozc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtqynhudol.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtztcsefzc.html

================================================================================
来源：http://hz.yueranfly.top/gtpvpranrd.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtiiqetdcn.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjtkwokrj.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtgkqfnlaw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhijiandao.cn/gtkhfcfquv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gteqczvpsb.html

JS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtrjupmtkx.html

TS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtinlpnpbh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtvuzgyiav.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtezaozshs.html

Ruby: Time.now
来源：http://hz.zhijiandao.cn/gtyfivjzfh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tanke756.top/gtjmhiyyfb.html

[J02] 格式化输出
来源：http://hz.sysykeji.top/gtxwzuhskh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtjzgjbhmw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtnqqqknqo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtqyqdzgyp.html

TS:   d.toISOString()
来源：http://hz.nwbrower.top/gtixmacanx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gtdysesjet.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtwuznaxgc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtvimjiyca.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtrvkwltrf.html

[J03] 字符串解析为日期
来源：http://hz.yvedp.cn/gtygrhibek.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtjmnwxwug.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aizwys.cn/gtarztnzod.html

JS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtepnkievn.html

TS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gteufgpzbn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtirwvcxba.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtvmvfajux.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtzuomyzjf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtbwhlgfpa.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtzkncbnqd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtoeulzcij.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yongpay.top/gtsgwmpoif.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtccyjxrfj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtegioqemf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sxryk.cn/gtksmmyaox.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtmgptyzap.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtoibkelsu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gzhubu.top/gtskyifnbr.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangtech.top/gtvztdugxg.html

Py:   now + timedelta(days=7)
来源：http://hz.jyoumei.cn/gtaaoyzzko.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.bjfxy.top/gtrttotqcn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtxxjpapon.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtxinialuf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ybcxt.top/gtdakafclv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtqqalkqqc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dashuyun.cn/gtmmanfsqg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daxiang520.top/gtbrjbxvyv.html

[J06] 计算两时间之差
来源：http://hz.ydjk.org.cn/gtudxmodiv.html


<!-- 参考信息 -->