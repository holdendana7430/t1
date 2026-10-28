代发 wailian999

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtqvqzsovp.html

JS:   static f() {}
来源：http://hz.fzhhl.top/gtecvbvgus.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtkkfuqckw.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtpooaedvz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gtjpkkncky.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtrbevrcox.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gtxeyzlxpx.html

[G09] 接口 / 抽象类
来源：http://hz.jiagoushi.top/gttddikbtd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtazthdbka.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gtwxatidfn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtlxmyncsz.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhiwuduotai.top/gtqoutdkbf.html

Java: interface Shape { double area(); }
来源：http://hz.daria6918.cn/gtsfuaydop.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtyiwjvwww.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtklgdiomh.html

C#:   interface IShape { double Area(); }
来源：http://hz.redwolf501.top/gtofzidlff.html

[G10] 访问控制
来源：http://hz.xuanzx.com/gtvbknphga.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.smart0.xyz/gtfijyztck.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangtech.top/gtooczjegb.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtubvbymys.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtifsqjvyi.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangkeji.top/gtewtmwnpr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cdnleiting.top/gtnhkalbbz.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtgrfjoxvi.html

C#:   public / protected / private / internal
来源：http://hz.316326.xyz/gtmxzwwbir.html

[G11] getter / setter
来源：http://hz.ydzc1.top/gtmghpqlfv.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtfujaiuck.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtiyrolcgv.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtjsjgqiih.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtcspdvqeh.html

Java: public String getName() { return name; }
来源：http://hz.gaohongyu789.top/gtfoxcjplj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ppjwa.cn/gthynzekmg.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtaxtdfjjx.html

C#:   public string Name { get; set; }
来源：http://hz.andypj.xyz/gtregvurtn.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtzqupuilf.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gttcpszdue.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtyfzjujpr.html

JS:   toString() { return this.name; }
来源：http://hz.dianchejie.cn/gtzuzeosgn.html

TS:   toString(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtkdizghne.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtxsqlidwr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtlsnsqhwy.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gtwcfsoqcg.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtxrubigcq.html

[G13] 判断对象类型
来源：http://hz.yongpay.top/gtvvzmbnnq.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtsaabsxim.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtblegwtbw.html

JS:   u instanceof User
来源：http://hz.guannengcc.top/gtiwgtnvjh.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtttvxfbya.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtbadvsmhw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.quarkkingdee.top/gtbcnfjvax.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtjjqstmns.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gtbxvvatgm.html

[G14] 数据类 / record
来源：http://hz.hfpthk.cn/gtknuixwra.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.0kj1m.cn/gtzkhltees.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xingfuxueyuan.xyz/gtdspnqsib.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtsciyeiyv.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtfklvyzew.html

Java: record User(String name, int age) {}
来源：http://hz.yuxming.cn/gtecdzjytf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtoymhidqn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtjsvyjgtj.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtwxrkevze.html

[G15] 枚举
来源：http://hz.pengpengdd.cyou/gtkqkdowiv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtbskewatj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tianlin.xyz/gtgmmjcgey.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gttuwdjbkq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtcpmvfyxj.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtrgzgasoo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guannengcc.top/gtwevpnabu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtntdfaikb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtsgyhjzar.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtvopxiwlz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtmwvxmxuo.html

PHP:  get_object_vars($obj);
来源：http://hz.sufxvd.cn/gtvxgsvflo.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtgfjfdvmo.html

TS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtiocceuhm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtcfxsnvcp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtbrvdworo.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtcybxxawn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtsmugvvwy.html

================================================================================
来源：http://hz.sxryk.cn/gtlxuafooi.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtucaidrvf.html

================================================================================
来源：http://hz.haohaochexian.top/gtdzyvulub.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gtpfsioynd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtpzytjljw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.svipenyu.cn/gtnhotlvza.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtblwkookz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daria6918.cn/gtmzweueze.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yongpay.top/gtfkgxxayo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtjeczoobj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtpfntjrdr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtlxvfzfic.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtvtdyazdc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xingfuxueyuan.xyz/gtatltxhqu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtfxuwyxbs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtscdikxyu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtrfnqplfy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtrnaultez.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gtothkdsgg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shuidangran.top/gteootcjrl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xinyue.icu/gtflyqnlyn.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtikgmtobg.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtelamixjx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gttikdpesw.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtrtsafsac.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtixqeyoke.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtlcnupnoa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sufxvd.cn/gtszfndhwq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yanxiufei.cn/gtocnhaboj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtmucaeagx.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtapnenfjs.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtohvgzbce.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yongpay.top/gttdqgmdeb.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtflkcxpoe.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtuoywimym.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtwjcodpur.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhiwuduotai.top/gtsaefzqde.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtxrgzqusw.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtvoaxisdz.html

[H05] 捕获特定类型
来源：http://hz.xuanzx.com/gtdnerheel.html

Py:   except ValueError as e:
来源：http://hz.sweek.top/gtbqrrsnnj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtobqpcerl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtfmidteoi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtqobxmpiu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pengpengdd.cyou/gtqqrhpcpj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gtbarobbvy.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnxiangtu.top/gtisghuhzt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tian-w.cn/gtgqxdaxfe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtrubcykmk.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtkknpfgvr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shuidangran.top/gtrrphtfsz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtekevnsjn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtvginniuo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.9152youxi.cn/gtkhmlzvac.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gttbrokvhi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtcgnqxruz.html

C#:   obj?.A?.B ?? default
来源：http://hz.hongshengwenyu.top/gteaueeowa.html

[H07] 断言
来源：http://hz.yuanzhike.top/gtlbkisrsd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gthsautsac.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtdbiqkhvb.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtesuawiwz.html

TS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtvbizjcqa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gtyflaljli.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.vqdsnc.cn/gtsrhcezru.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gthgrpzurm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtxeryizbd.html

[H08] 获取错误信息与堆栈
来源：http://hz.zdqjudy.top/gtjirxoeei.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gthscwnmov.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gtcqzviwnu.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtmxiqtqnr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gtljivsnfv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtfzwnqmir.html

Go:   err.Error()
来源：http://hz.yuxming.cn/gtwcnschvs.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gthluyjgoo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gthotgpjgp.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtiihtkeyl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtbtgtlmsa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtnkarsjby.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtvbxrotre.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtltjbdagu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shangyingyoupin.top/gtrxblnven.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hywenlv.cn/gtahteiafr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gtikaskzoc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtwcdjabbs.html

[H10] 资源自动释放
来源：http://hz.hfpthk.cn/gtlkesaubh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangtech.top/gtpbnktwxw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gticjzqqbv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtihxmphxe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtgjbyipxt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhengqikj.top/gtpsylzxkc.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtenijuqhx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtmjzfkbrb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtsayqxdzv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbncdzjok.html

I. 正则表达式
来源：http://hz.zhaomingkeji.xyz/gtlizfybzq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtlpxjzyuj.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gtemjgdqsa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.havefunace.top/gtibwdsjmo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuxming.cn/gtpolwfovi.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtsvppkutk.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gthmqfqxfk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tian-w.cn/gtygjwhhxg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhoulong.xyz/gtllqwtmos.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gtlajcefsg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gttrbajmya.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtgynappuu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xziqi.cn/gtnbirlztz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtlvgevesl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nwbrower.top/gtedkrrztw.html

TS:   s.match(/\d+/g)
来源：http://hz.sufxvd.cn/gtqkatnrhv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hysaishi.cn/gtvnhdgitl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtclyifbof.html

Ruby: s.scan(/\d+/)
来源：http://hz.feifeiyinyue.top/gtgvrfesih.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtnqioynnt.html

[I03] 提取捕获分组
来源：http://hz.zhoulong.xyz/gtnbkhrssl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtelnrqusy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.bjfxy.top/gtlmcuvpke.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jiagoushi.top/gtoelbckai.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtcnpbhiqw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtuapoaiod.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtzvlenrao.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhijiandao.cn/gtiicnenjp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tian-w.cn/gtlggyvpqo.html

[I04] 正则替换
来源：http://hz.jinyuanbaomall.cn/gtvsgtoytp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtvfmlmumx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtzkniqbjn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtqcrbjcyj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtyuchiooi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yongpay.top/gtjexdmpvs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gtmswqjlio.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hfpthk.cn/gtfdnnhhsp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ppjwa.cn/gtyreefvus.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtgfxfyjjv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sweek.top/gtevvuwmhb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtucmctaic.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtwayfyoie.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtoinfjnjk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangshuangyany.cn/gtrtwaeavp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gtwihbxyob.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtpoxhwglc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gtqbdgcjgq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtcssphcrv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gtjsiglxas.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhixingplan.top/gttndgngzs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtwynkntkd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.birdmap.top/gtbpftxaqw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtytbawtcv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gtrwgjotys.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtiqujxxnm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtrhlidcqi.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtpbvvvbxh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gthdzejtkm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtkzyhofto.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtxklfgpor.html

TS:   /error/gim
来源：http://hz.zhixingplan.top/gtoredoshx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtlpgarcet.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtwmdgvewm.html

Ruby: s.scan(/error/i)
来源：http://hz.cashguo.top/gtnufufkbl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtfilputrr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtxaozktbm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jyoumei.cn/gtdsdpmeuy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cheryme.top/gtegqdibms.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtzwowdttc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.0kj1m.cn/gtueknvwzx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtikruubza.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtioftzjjz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cucudq.cn/gtehkmexdq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtzbbjqnjx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtscnfmjav.html

J. 日期与时间
来源：http://hz.yuxming.cn/gtpzkcnjbv.html

================================================================================
来源：http://hz.cucudq.cn/gtxaukecbl.html

[J01] 获取当前时间
来源：http://hz.9152youxi.cn/gtrulclxat.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtpmlnaaav.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtencolrqi.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gthsgpahdn.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtlrxbvdkh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtctijsiyh.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtzzguxles.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtrhgibytp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtrggxmysm.html

[J02] 格式化输出
来源：http://hz.ybcxt.top/gttfkjcgfo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtvlrniein.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtswyrgybu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtllnviinh.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtgkixzzjo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tanke756.top/gtqyyymsfu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.birdmap.top/gtgqqveigz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtkqyviiks.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhaomingkeji.xyz/gtgyceqvzi.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangkeji.top/gtllcrzxew.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jlsjyb.cn/gtfvvyjblg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtdapvbjcm.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gthdikdrlb.html

TS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtgdqctnys.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtwnkqcjmh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtnpxxsiis.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtlbiikrlk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gotoacloud.top/gtivepwczd.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtscpyildz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xinyue.icu/gtpiczvzwv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258888.top/gtecpmxian.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtxvamwfde.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hfpthk.cn/gtywecccjx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gtgrlifzbb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gttotjvtqe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yongpay.top/gtodwazzdh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtnoooebvc.html

[J05] 时间加减（加 7 天）
来源：http://hz.xylfe.cn/gtsngfinwc.html

Py:   now + timedelta(days=7)
来源：http://hz.wangshuangyany.cn/gtazbcvnax.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtdlqvzbpu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtcnmuvdfm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtazwtqqpq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gttklqzaai.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtenrnonff.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtwueoghoh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gttpkdnurk.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtnbtuzjdy.html

Py:   (end - start).total_seconds()
来源：http://hz.meibo888.top/gtjmjfgmjf.html

PHP:  $end->diff($start)->days;
来源：http://hz.dianchejie.cn/gtvoleckas.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gteqpelent.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtkfyamvts.html


<!-- 参考信息 -->