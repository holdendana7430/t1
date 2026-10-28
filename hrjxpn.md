代发 wailian999

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtlxwsoplc.html

JS:   static f() {}
来源：http://hz.nanxuanxn.top/gtdgmlkxxn.html

TS:   static f(): void {}
来源：http://hz.yongpay.top/gtdkanppfe.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtadzbkycq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtlirctouu.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtxygdtiqy.html

C#:   public static void F() {}
来源：http://hz.zhoulong.xyz/gtvmswguzy.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtdlzmyoie.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cdnleiting.top/gtrsiavpng.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ppjwa.cn/gtrhfpvuzz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhongyouzk.top/gtdctilppq.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gttzffkzqj.html

Java: interface Shape { double area(); }
来源：http://hz.xingfuxueyuan.xyz/gtprtqcyoz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.haohaochexian.top/gtbikmgzjx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gtxucoeisi.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gtoztjmzfe.html

[G10] 访问控制
来源：http://hz.shanyushiyangtech.top/gtjrrumobh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gtxuwrcizc.html

PHP:  public / protected / private
来源：http://hz.nwbrower.top/gtneplnobr.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtndrbdlge.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtauoltktx.html

Java: public / protected / private / 默认包级
来源：http://hz.c1oappe.top/gtqkagizkr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.kuanghao11.cn/gtidsginkk.html

Ruby: public / protected / private
来源：http://hz.zhiwuduotai.top/gtfzjxqkxz.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtkamiiecn.html

[G11] getter / setter
来源：http://hz.ivvv.top/gtzqisuosf.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gtggxdbspd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ivvv.top/gtiolhvsui.html

JS:   get name() { return this._name; }
来源：http://hz.sxryk.cn/gtnppaynbb.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtyneapjjm.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtorcggcwp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pycfn.com/gthuedpywc.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtzxfgfvnf.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gttcgtnsrp.html

[G12] 对象转字符串
来源：http://hz.cucudq.cn/gtjejcjcop.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gthffhdqjr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtgabrvzpb.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtimnrwhdk.html

TS:   toString(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtrwtlsnii.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtwsdonfll.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gtblntepww.html

Ruby: def to_s; @name; end
来源：http://hz.ppjwa.cn/gtqpccuyfh.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtkycdhfev.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gtczfzebyv.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gttgxwlmrn.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtukyeublv.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtnlkmurzu.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtgsarqvuk.html

Java: u instanceof User
来源：http://hz.iojbl.cn/gtdmnouzlr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtulbnngoh.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtixdzjhsj.html

C#:   u is User
来源：http://hz.nanxinkj.top/gttytbdbwb.html

[G14] 数据类 / record
来源：http://hz.9152youxi.cn/gtzrwbathw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hongshengwenyu.top/gtcystcedy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pengpengdd.cyou/gtvxrlrwub.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtlopwaklo.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtnnmcyyuy.html

Java: record User(String name, int age) {}
来源：http://hz.hnxiangtu.top/gtijyoxvmc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtfpwpesxz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zycfv.cn/gtuauxdxba.html

C#:   record User(string Name, int Age);
来源：http://hz.cdnleiting.top/gthlcuhtqx.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtbuzargii.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.mhx1999.top/gtflacfmir.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuxming.cn/gtysyltyzy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sysykeji.top/gtawawoxjl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtmsrhylsu.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxinkj.top/gtcixcjfck.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gogol.net.cn/gthovdffpd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtivjzewzs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtarvrnlek.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtrzamvceq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gtorslvqox.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtehacbqwl.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtapngsmiq.html

TS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtjgfjcbed.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gtlheqkgav.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258888.top/gtebtjvdga.html

Ruby: obj.instance_variables
来源：http://hz.daxiang520.top/gtbygfcrhz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtuedlwuwv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtavpdvron.html

H. 异常与错误处理
来源：http://hz.jinghuilouyu.cn/gtvcevurjf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthmpcgydf.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gthlbmcqpr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtfmgzgriu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gttmzzidkq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtpnllazut.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gthremntpq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.meibo888.top/gtdyxbrtqd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtxuadojtn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtososrere.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jlsjyb.cn/gtrhysqzeb.html

[H02] finally / ensure 收尾
来源：http://hz.haohaochexian.top/gtbwsjhcdm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtlhqanhfo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtklnxjxuo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtwrvhtbfx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtfibbuwdc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtjddoipin.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.andypj.xyz/gtelrfpmzf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtdngwdkqv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtpvthksxq.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtqvqybxrm.html

Py:   raise ValueError("错误信息")
来源：http://hz.cdnleiting.top/gtxyqqzroq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtvpepdhap.html

JS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtukuqvoam.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtmppyzaiu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtwrzwkcto.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sxryk.cn/gtavcverhd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hysaishi.cn/gtdgcwdadj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtemksqegr.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtcrgvwfvw.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gtibsoynpq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtfttlpzzs.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtzznfwoab.html

TS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtfmmzdkjl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daxiang520.top/gtktwbqtpv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigfzy.top/gtevyymeix.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtxpydeiae.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtjmybbrjh.html

[H05] 捕获特定类型
来源：http://hz.hammf.cn/gtbsarppur.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtaxidvqhi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gthvvwmxqe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtbwdqclzn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtcvkzfwmv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yvedp.cn/gtsbwmlgyw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangdashe.top/gtkiuffklk.html

Ruby: rescue ArgumentError => e
来源：http://hz.quarkkingdee.top/gtbkcxcohr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtrvqhodwu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gtzcgpgonc.html

Py:   value = d.get("k") or default
来源：http://hz.9152youxi.cn/gtohzeumsi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtvqdedalm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtporngsdn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtaztdpsbn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hongshengwenyu.top/gtxokvwqtc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtzdpeaytl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigufen.top/gtrevcefjs.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgufenzy.top/gtsypowwpd.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gtvmwzquir.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shuidangran.top/gtmjjjfnsv.html

PHP:  assert($x > 0);
来源：http://hz.gogol.net.cn/gtsippbjdi.html

JS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gtoleekcat.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtotqgzako.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtgizzxwrt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtxjfldnch.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guowangkeji.top/gtjxhmhpgs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtftpzjibz.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtsfjijsjh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sysykeji.top/gtvbmetexn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtwbndkbum.html

JS:   e.message;  e.stack
来源：http://hz.cqqwz.cn/gtfwkaqdue.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhiwuduotai.top/gtlnkzoouc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtvwnoywln.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtkzbrrhpp.html

Ruby: e.message;  e.backtrace
来源：http://hz.havefunace.top/gtegiggofu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtzzramdlq.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtplrrgnzs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtlthynohq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtpdycdypf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhixingplan.top/gtpaqbgdie.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydjk.org.cn/gtugslswsk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtltikhahg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cashguo.top/gtotslnppc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgufenzy.top/gtkcsnxwgr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtqohponoo.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtjqarhqnz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gtpcjdefmr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hysaishi.cn/gtcrecqwxn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtlvciguec.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtbwjgboma.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gthkxqsnwq.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtfvcugrzu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtbzuzsfhn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.feifeiyinyue.top/gtwzngswxw.html

================================================================================
来源：http://hz.hfpthk.cn/gtifcryvwl.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtsucaxxdb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcegxjnux.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gtpeqvdlho.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtqoqlaxch.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zdqjudy.top/gttjbtbktk.html

JS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtbltfcdvg.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtwefejqsu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtdgpoktai.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenlongwang.top/gtzswulqph.html

Ruby: s.match?(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtrozmxeot.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gthciskqal.html

[I02] 提取所有匹配
来源：http://hz.feifeiyinyue.top/gtnccgazfs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtvvlfdevy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jlsjyb.cn/gtjhopjfor.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gteiodnicy.html

TS:   s.match(/\d+/g)
来源：http://hz.jianghu66.top/gtdsxqpgqq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gttvzmshgy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gthavcufkq.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtloxfoqxq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gtatvoaygb.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gtemvtgvvs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtrboufaij.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gtjhlvcoso.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtkcpixasd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gzhubu.top/gtpbkqftiy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ybcxt.top/gtzpevczve.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jlsjyb.cn/gtoextrtgf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtxwmgnmfg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.haohaochexian.top/gtgjmzgvmm.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtfuoklkap.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtfdmwhmmd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtyfylnjoy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtposnvgge.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtnboqsuef.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtaksdzwaf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guowangkeji.top/gtqjrotfeh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydjk.org.cn/gttzshabuu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gticztwasp.html

[I05] 按正则拆分
来源：http://hz.daxiang520.top/gtcowipbvb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtowxgxcke.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gtbaupdazv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtankmjfxh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtoabrhjal.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daria6918.cn/gtjixfclke.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtfvedrwrv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtatsuxdex.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.dashuyun.cn/gthtfqulbp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.svipenyu.cn/gtxhrpjhwu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtrgcmxmqe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtxwfcaoyr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtvjbmerpd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtmfacvzts.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtobsnxils.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtdielbbub.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtlabreomd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtdxvdhjfj.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtngvukhio.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gttafidcyl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtztphoymr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guowangkeji.top/gtbopchywr.html

TS:   /error/gim
来源：http://hz.snrcjt.cn/gtfatpbuyn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxinkj.top/gtrjbzlbec.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.52xcode.cn/gtyahfkkii.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gtgfegjnxb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtwvjnrayq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xylfe.cn/gtnohkumky.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinqigufen.top/gtcuasulac.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtdjevdkye.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtrusjktag.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtlilvwsok.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.birdmap.top/gtxadzdfrj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gthfsvhyba.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tian-w.cn/gthrghppmc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtscrhpgzg.html

================================================================================
来源：http://hz.wangdashe.top/gtmgkqktei.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtekzlvdur.html

================================================================================
来源：http://hz.fzhhl.top/gtsqumvlua.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtlxxmppyh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gttdbgoabq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gthfpvfbij.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gteuskaend.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtytubqusv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtupkpyzsm.html

Go:   time.Now()
来源：http://hz.yj202588.top/gthomechbe.html

Ruby: Time.now
来源：http://hz.zhoulong.xyz/gtqymipbca.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jyoumei.cn/gtmrusnuee.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gthfxzlmuz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtpuvnxkjw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtnjpwdvle.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtyrfepjkr.html

TS:   d.toISOString()
来源：http://hz.daxiang520.top/gtmtreddjc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtqkobpkwj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shuidangran.top/gtrpledzou.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtkpfyjyql.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtkbwueybr.html

[J03] 字符串解析为日期
来源：http://hz.daxiang520.top/gtzihnlkup.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fzhhl.top/gtzrldyewe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ehwqpu.com/gtekapwiek.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtcwhzeahw.html

TS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtettvicni.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.316326.xyz/gtwkkzyjul.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtunqjnflt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtlgeqnhmt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.haohaochexian.top/gtzxdehvkz.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258.top/gtlbsvmdhl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gttemvtqag.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtquotmnvx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtrlveydev.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtnoxoidcc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtwqyjcbju.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtbcqxieui.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtmjedajky.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigfzy.top/gtmqrekban.html

[J05] 时间加减（加 7 天）
来源：http://hz.quarkkingdee.top/gtlyitlfbu.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtrzynrong.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yanxiufei.cn/gtkmypbvac.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtribefaoq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtundephtr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangkeji.top/gtbkqidqbi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtkefhhkke.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cashguo.top/gtyidpporf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dashuyun.cn/gtohbulzwz.html

[J06] 计算两时间之差
来源：http://hz.yongpay.top/gtduxscbas.html

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gtcdwdsqwv.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtmaklrysl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtqmwpwtdu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xziqi.cn/gtihlhegix.html


<!-- 参考信息 -->