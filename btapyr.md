代发 wailian999

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gtabywphcr.html

JS:   static f() {}
来源：http://hz.yj202588.top/gthzjrliev.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gtzgkehagt.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtkcobmmsv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtumjezbwy.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gthpcifhmy.html

C#:   public static void F() {}
来源：http://hz.gogol.net.cn/gtuqyeuxhr.html

[G09] 接口 / 抽象类
来源：http://hz.snrcjt.cn/gtstpzrodf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtjfbkmiuk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtoydpnrhw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtxdrcvayu.html

TS:   interface Shape { area(): number; }
来源：http://hz.jiagoushi.top/gtghwzdtec.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtamhhoddt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xylfe.cn/gtvytsgtvr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.feifeiyinyue.top/gtbylnnmyp.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgufenzy.top/gtuxmmojod.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtxfoniaof.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgufenzy.top/gtdrgzjegx.html

PHP:  public / protected / private
来源：http://hz.zycfv.cn/gtzoxbyopl.html

JS:   #private 字段；其余公开
来源：http://hz.shzxlz.cn/gtqmeqotky.html

TS:   public / protected / private
来源：http://hz.zhixingplan.top/gtzafxyxxd.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gtneoikqhj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgfzy.top/gtdvplhahp.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gtiyjwbsvk.html

C#:   public / protected / private / internal
来源：http://hz.andypj.xyz/gtoedaracv.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtdweoeyxs.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtnfjnobtk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtwwgkexyt.html

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gtuieoomtk.html

TS:   get name(): string { return this._name; }
来源：http://hz.andypj.xyz/gtjwfevkjb.html

Java: public String getName() { return name; }
来源：http://hz.xziqi.cn/gtldmlwcms.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtxgdsucfm.html

Ruby: attr_accessor :name
来源：http://hz.feifeiyinyue.top/gtkzxijqqx.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtansksqyq.html

[G12] 对象转字符串
来源：http://hz.nanxuanxn.top/gtbkrapstt.html

Py:   def __str__(self): return self.name
来源：http://hz.xinyue.icu/gtyvgjmwzv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtxyooeqmh.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtzubskert.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtavciikom.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxinkj.top/gtttxsypju.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gtedxnidei.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtuqosjfgs.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gtvaonnqjx.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtkekclrhi.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtmnpabwwy.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtiiuqfhqg.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtaijxvrmj.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gtjkiuxrnf.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtttglyvag.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sufxvd.cn/gtmckysvty.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gthwgxofwt.html

C#:   u is User
来源：http://hz.jinghuilouyu.cn/gtagbuemhe.html

[G14] 数据类 / record
来源：http://hz.gaohongyu789.top/gtufmdjjtz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenjidiqi.icu/gtdjcnsyvz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtpqiwhrsl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gteorjqpiw.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gtfuteliaz.html

Java: record User(String name, int age) {}
来源：http://hz.hnxiangtu.top/gtxloetwya.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtlndwedxs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtmxmzbycz.html

C#:   record User(string Name, int Age);
来源：http://hz.yangfankeji.com/gtlqhrnrmf.html

[G15] 枚举
来源：http://hz.xziqi.cn/gtetqlztjj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtdcshxyqn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.52xcode.cn/gtobohdday.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtiduvwjvm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtcoavsxig.html

Java: enum Color { RED, GREEN }
来源：http://hz.sweek.top/gtcgkvrcbg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenzaomai.com/gtaojtptlu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gtwdfmznjq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtruqhaecm.html

[G16] 对象转数组 / 字典
来源：http://hz.pengpengdd.cyou/gtxnbpubsv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gttfkgkgbq.html

PHP:  get_object_vars($obj);
来源：http://hz.yonumen.top/gteueowsyy.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtuhbtclir.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtnkaaewbv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtnbyftvrh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtqdxdekyf.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtsjdoofih.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydzc1.top/gtgstxjezb.html

================================================================================
来源：http://hz.ydzc1.top/gtxouiykif.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtjrfxtllz.html

================================================================================
来源：http://hz.pycfn.com/gtmkkojert.html

[H01] try / catch 基础
来源：http://hz.cdnleiting.top/gtelnstxcm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhixingplan.top/gtuingimih.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtoilzyxqs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gttpqdhogh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gtouxhbswz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtvjzkcvgv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtkfjajvgf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hysaishi.cn/gtrqgntnmi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtljluxthd.html

[H02] finally / ensure 收尾
来源：http://hz.dashuyun.cn/gtefqlazzw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zdqjudy.top/gtlcygsred.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtsjrkeeba.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtyonyxwzg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gthlpoxbjn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtemlknbfs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtoworbrwu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtnvosxruc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtehybjevw.html

[H03] 主动抛出异常
来源：http://hz.nanxuanxn.top/gtlgzlibwj.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtkhpfnujx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gttvdmiugc.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtqzdemjmr.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtjkdvlymj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtewojvnxw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yonumen.top/gtbfbpbcmw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fzhhl.top/gtmtflgohy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtxnnnbtff.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtisumhopd.html

Py:   class MyError(Exception): pass
来源：http://hz.daxiang520.top/gtrnqwxazp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jianghu66.top/gttjmaprjy.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtnznqclvc.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gttfsyyzww.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shuidangran.top/gtxlzvgbhi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yongpay.top/gtlavbdpue.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gtmxdfrqzg.html

C#:   class MyException : Exception {}
来源：http://hz.andypj.xyz/gtorkwbwjt.html

[H05] 捕获特定类型
来源：http://hz.ppjwa.cn/gtyxfmaroj.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtoeetplzx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hysaishi.cn/gtgtgkvlwc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtjvbguryy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtnnudyrex.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtaixuncze.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydjk.org.cn/gtqocsweun.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtrcngwlnk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nanxinkj.top/gtogbekecm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aizwys.cn/gtqjdottjk.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtwtlhlyrs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnqzz.top/gtvtordizk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gthvileuad.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtashyyfgp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangtech.top/gtkbvklfbg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtsuswnwcd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtzcbvdzqd.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenzaomai.com/gtdwusphpg.html

[H07] 断言
来源：http://hz.316326.xyz/gteewwgdhy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gtqdqhkchs.html

PHP:  assert($x > 0);
来源：http://hz.hywenlv.cn/gtlvmgewbu.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gthqpbxxay.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtbgvlacka.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtikqkhpvr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shzxlz.cn/gtnemksynl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtztuhjdjk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtegtsmupm.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtmtqptvya.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258.top/gtpomrawuw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtnyundnnf.html

JS:   e.message;  e.stack
来源：http://hz.ybcxt.top/gtwxehjybx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ivvv.top/gtlutbrpjk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gtdvvmuqoq.html

Go:   err.Error()
来源：http://hz.52xcode.cn/gtmwoflpwx.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtwlrazpiu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtygtmwkqm.html

[H09] 带错误码的异常
来源：http://hz.tianlin.xyz/gtbwalxjze.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gtzaysjcxm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tianlin.xyz/gturlbiwqm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangtech.top/gtzckqxcdo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtvrmovdsc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xinyue.icu/gtdjmgriuo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guowangkeji.top/gtuostwzzb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtqlhbkuel.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtmdzgndsh.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtcpahlcii.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gtmkprthuy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shangyingyoupin.top/gtinmsuslc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtgaoshzff.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtetacdpod.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhixingplan.top/gtkvzibjtr.html

Go:   defer f.Close()
来源：http://hz.jiagoushi.top/gtrljbgxdp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tianlin.xyz/gtcjudpbxn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtzfyzfrpu.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjetrkpyw.html

I. 正则表达式
来源：http://hz.ivvv.top/gtiwjokodj.html

================================================================================
来源：http://hz.tianlin.xyz/gtbthkbqed.html

[I01] 判断是否匹配
来源：http://hz.cdnleiting.top/gtkyymuhzc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtjktrjtrg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hfpthk.cn/gteawrwgwt.html

JS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtxvizbbtx.html

TS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gttutwvhar.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtiavfhmwy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shuidangran.top/gtypzbldze.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhongyouzk.top/gtghvfvsee.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.haohaochexian.top/gtlnawopxu.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gtgajwnlez.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gttyjpciaa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtfpdlkeji.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shuidangran.top/gtsckvldhx.html

TS:   s.match(/\d+/g)
来源：http://hz.jyoumei.cn/gtscestkie.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhiwuduotai.top/gtphakbvhv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yanxiufei.cn/gtqzrwgioz.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigufen.top/gtpwiryavm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtgkbkbfam.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtzrkvcqjb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtpuluashf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gttmurzqwj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sysykeji.top/gtbzlzxkca.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtxmgtpjgk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zycfv.cn/gtqbimsygu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtlhhgawud.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nwbrower.top/gtgsekujiu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yangfankeji.com/gtehyjnbna.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtosjfqbeq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daria6918.cn/gthjauenbv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtnpqddshh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtieeuiuut.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtuolufywm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydzc1.top/gtrfmbivbd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtfirksvsl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenzaomai.com/gtlvzvexhh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shangyingyoupin.top/gttuffmnnv.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gtceylyphy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gttdrsiehn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gtihogvhhs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtpltlpeqn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtkmymzvxf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxinkj.top/gtytuhniac.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zycfv.cn/gtzlacfufi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtgbnxvwya.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtzxpwjoct.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ywan-chungtsiang.top/gtezujafal.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtzzbimfzf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtxlphvdjs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtlvdxvhaj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtyzvetlxo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gtxgwommpi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtxvbqpikj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtabeffnez.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtelraoxiu.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtgzhffnjo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yueranfly.top/gtbhoodzfd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtpshsrptx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sysykeji.top/gtewnvwncx.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtfhafrrno.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtjumtuqvs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtqivkegrq.html

Ruby: s.scan(/error/i)
来源：http://hz.fzhhl.top/gtcctzjtbv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtwpeoodrc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gttiaefhqa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258.top/gtcbeafvjw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtctgofyxt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtynvhcdhd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtfshvzpnv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtvxvulskn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtnliyzfxj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ywan-chungtsiang.top/gtsmtxxesp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtwnhgepmb.html

================================================================================
来源：http://hz.gzhubu.top/gteeadjpia.html

J. 日期与时间
来源：http://hz.tian-w.cn/gtssdpmqxh.html

================================================================================
来源：http://hz.yangfankeji.com/gtlxuirfeb.html

[J01] 获取当前时间
来源：http://hz.iojbl.cn/gtmeiegwit.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtiozysusf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtznzpsade.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtceoyrhmg.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtcdyueado.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuetiantiany.cn/gtyaxpjknj.html

Go:   time.Now()
来源：http://hz.ywan-chungtsiang.top/gtyxbtvjer.html

Ruby: Time.now
来源：http://hz.zycfv.cn/gthuezgqde.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.c1oappe.top/gtgokzjktr.html

[J02] 格式化输出
来源：http://hz.nanxinkj.top/gtteawmdbn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtylbseiaz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtilppffmk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tianlin.xyz/gtfxisvesm.html

TS:   d.toISOString()
来源：http://hz.yvedp.cn/gtitmharhw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shzxlz.cn/gtbikylzcd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtxrmeqcfd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtqucuqoip.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gthoevigwm.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtyzbqwjxn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ehwqpu.com/gtatbhmdqy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtyffacakr.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtoellnhjd.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtgaawoobn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtftqeasvv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtqjcwtdsa.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtsliqxaus.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fzhhl.top/gtkcjoradz.html

[J04] 时间戳与日期互转
来源：http://hz.feifeiyinyue.top/gtsbuyenav.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtuccdjwjz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258888.top/gteqfpblsm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtyxjvsamo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtyxrycdim.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gteffeqoap.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gthmygevpq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtbiesdaqo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtfiranprr.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtbdjvcvmb.html

Py:   now + timedelta(days=7)
来源：http://hz.hywenlv.cn/gtzkfsefqo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.havefunace.top/gtqlwpujgl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gthjjdgjzh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtequtmtii.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gtxqudzyvc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtrjvdzkmm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tanke756.top/gtelgeyqsu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gtcrfvgrfb.html

[J06] 计算两时间之差
来源：http://hz.dianchejie.cn/gtypeckkwi.html

Py:   (end - start).total_seconds()
来源：http://hz.zhiwuduotai.top/gtcnttbqnq.html

PHP:  $end->diff($start)->days;
来源：http://hz.aizwys.cn/gtbpngppmp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hfpthk.cn/gtuaxpxbtr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gtpmncvlcf.html


<!-- 参考信息 -->