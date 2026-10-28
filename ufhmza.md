代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtwsglyojh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fengsongda.top/gtybnotmcx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zdqjudy.top/gtluqsxqbm.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtwlmaaren.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtebbfpkgc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.haohaochexian.top/gtkmbuzpwm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtxvetlqej.html

C#:   interface IShape { double Area(); }
来源：http://hz.haohaochexian.top/gtjnrwrhov.html

[G10] 访问控制
来源：http://hz.fengsongda.top/gtsnibtihu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangshuangyany.cn/gtlcuwjkhz.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtoylfivit.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtbzceiamn.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtlzlqsdyu.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtyxrxjcms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gtejzhbrvf.html

Ruby: public / protected / private
来源：http://hz.daria6918.cn/gtwwkgdhba.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtboddmnit.html

[G11] getter / setter
来源：http://hz.quarkkingdee.top/gtnmdklgnw.html

Py:   @property 与 @x.setter
来源：http://hz.pengpengdd.cyou/gtokslnpmy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtatvbgybd.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtfbftrzwi.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgufenzy.top/gtcpcaypxl.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtamevnjqn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuanzhike.top/gtzftbnljy.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtgwmqbyoi.html

C#:   public string Name { get; set; }
来源：http://hz.jiagoushi.top/gttieaytji.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtqpvfipmi.html

Py:   def __str__(self): return self.name
来源：http://hz.pycfn.com/gtmjoebnik.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtisiaqbto.html

JS:   toString() { return this.name; }
来源：http://hz.yj202588.top/gtfctmvpdo.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtejuplidb.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtcogkdqda.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtgdfncwag.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gttlgnbosc.html

C#:   public override string ToString() => Name;
来源：http://hz.shangyingyoupin.top/gtzenovihe.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gtsphjfmja.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gttmrxgymu.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtfvmtccgi.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtwbvvmklz.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtvmpadnjt.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtbmwiljru.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.vqdsnc.cn/gtwgnstyon.html

Ruby: u.is_a?(User)
来源：http://hz.316326.xyz/gttzjimsml.html

C#:   u is User
来源：http://hz.cucudq.cn/gtlutymilu.html

[G14] 数据类 / record
来源：http://hz.jinqigufen.top/gtsiwubmlv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xingfuxueyuan.xyz/gtjjgvvaau.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtgeytkxsx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gtddudmpiu.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtivsaiqfi.html

Java: record User(String name, int age) {}
来源：http://hz.yonumen.top/gtuoaandnu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yanxiufei.cn/gtihmwholg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangkeji.top/gtmgxphevr.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtakvxgqrn.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtsweetogg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtghplkmon.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtggixgclr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gotoacloud.top/gtgkbzaiqd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtoacwbtgy.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gtemeiwnuc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtuxmliqvs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtbnfjnqkc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtwxfmavlz.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gtmxoohrkq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pycfn.com/gtfahqajzr.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gtloiimgnd.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gthpkshwgz.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtdqiwbfra.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.havefunace.top/gtdledsyxy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuanzx.com/gthcgkqbnc.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtamhmztad.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gthedmdeqi.html

================================================================================
来源：http://hz.zhengqikj.top/gtmhdbwqfs.html

H. 异常与错误处理
来源：http://hz.haohaochexian.top/gtvhbhobht.html

================================================================================
来源：http://hz.hammf.cn/gtnflqcxyn.html

[H01] try / catch 基础
来源：http://hz.jinghuilouyu.cn/gtyhxfgfip.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtvjxvfmym.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinghuilouyu.cn/gtitgoretp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtndaafgxg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.9152youxi.cn/gtjlqyrmoi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.andypj.xyz/gtprzfaxlv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cheryme.top/gtydxfajzo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtqikggjoc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtrtfrdijk.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtzxxwqhmo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtuajaijvz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtikgjkulr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtfqnufswl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gthfdgrhmq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtzgcvkwgm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hywenlv.cn/gtznbvhivw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtgbjxfdrf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhengqikj.top/gtwaezmddu.html

[H03] 主动抛出异常
来源：http://hz.tianlin.xyz/gtlgablxcs.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtgjwddfsb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtxravqrdz.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gthzscvpvr.html

TS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtxzwuhlun.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gthqqwztqo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gtomaumzns.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yanxiufei.cn/gtwysyzfjk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtsultetdk.html

[H04] 自定义异常类型
来源：http://hz.sxryk.cn/gtgkdwvjuy.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtlmsuudrq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtwyjugncv.html

JS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtraxunqgw.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtenxxudyn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnqzz.top/gtjteqjtuv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtuazuekyl.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtwnsnjbtl.html

C#:   class MyException : Exception {}
来源：http://hz.fzhhl.top/gtordvjyaa.html

[H05] 捕获特定类型
来源：http://hz.daxiang520.top/gtzawxbeol.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtljxkqoyi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhoulong.xyz/gtbjpofvpf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtjawwitqq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gtohrgglmm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gthmszttgo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hysaishi.cn/gttsultafi.html

Ruby: rescue ArgumentError => e
来源：http://hz.zycfv.cn/gtldhlicaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zdqjudy.top/gtoapvboeg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hongshengwenyu.top/gtxivqsuda.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtmxmftyka.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtdwizxrqu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtphimgklu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gthergilfq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gtjnssyxqa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jiagoushi.top/gtkjwlsfvh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtrnoiclbj.html

C#:   obj?.A?.B ?? default
来源：http://hz.gogol.net.cn/gtfsgaqgsd.html

[H07] 断言
来源：http://hz.tian-w.cn/gtzngnqvah.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuxming.cn/gtklzgucjg.html

PHP:  assert($x > 0);
来源：http://hz.hongshengwenyu.top/gtmlffmdiw.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtkzbdiwir.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtmcjhrbcn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhaomingkeji.xyz/gtgqeqkzwd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shangyingyoupin.top/gthmcjqngu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jiagoushi.top/gtksepcqjb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xziqi.cn/gtfwfzzmrv.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinyuanbaomall.cn/gtnalnrfzw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yueranfly.top/gtefvwbccc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.kuanghao11.cn/gttykzeiep.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtjrntlkly.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gaohongyu789.top/gtpozpqzny.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cdnleiting.top/gtpsrhbgjj.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtecoespva.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gttpejwpny.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtibgigbcf.html

[H09] 带错误码的异常
来源：http://hz.sysykeji.top/gtbqdddskc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinyuanbaomall.cn/gtoqdtaoqc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnqzz.top/gtasktbvcb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gttaxxgkqz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtxqivxugt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtqpizebyw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtdrlkkljd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtgzsgetfk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guowangkeji.top/gtdbgpwkwm.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtpgxubeoy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jianghu66.top/gtdwvqiiyy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtknysoijb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtfryqyewd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gttxajligb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xinyue.icu/gtvhrxlvfw.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtluiesogc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.9152youxi.cn/gtfbezjwzn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jiagoushi.top/gtnxdedqjs.html

================================================================================
来源：http://hz.yj202588.top/gtylbrdkzp.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtnsrigavc.html

================================================================================
来源：http://hz.cucudq.cn/gtxirfkwfd.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtifhgbbui.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dianchejie.cn/gtpsbmctms.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guowangkeji.top/gtfxmgluur.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtlsbkykob.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtwtbpbmep.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtmthmspvm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gttgytketb.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtylngbdqv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnxiangtu.top/gtqwofrruu.html

[I02] 提取所有匹配
来源：http://hz.zdqjudy.top/gtuluiznnh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtpfffjkfc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gtcdofrano.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenzaomai.com/gtawuqejzd.html

TS:   s.match(/\d+/g)
来源：http://hz.yj202588.top/gtsboipqmo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fengsongda.top/gtitssuuzr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gtkszymwhe.html

Ruby: s.scan(/\d+/)
来源：http://hz.hammf.cn/gttmhqxrrl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yanxiufei.cn/gtljzsfzyd.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtvzkrxssw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigfzy.top/gtjxkwhdcy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sxryk.cn/gtdlbpddsx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yanxiufei.cn/gtjbwhpleb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gtpqdazzev.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gtmwpeaclq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangtech.top/gtgmdanfol.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gtsegjlfsh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gthjklwdis.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtsrsfgfif.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.havefunace.top/gtekttgedi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtxrifcwse.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtzdvgvstc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gthfrsskpj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenlongwang.top/gthquhskga.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuxming.cn/gtqcpfpmfs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtnsqbdeym.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtpshgcoxl.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gttlsuxzwz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtjhnogmtj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtskgdtvsn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtypftqlpw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtxsbiunmu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxinkj.top/gtbbotouze.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangdashe.top/gtpamuddik.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtcomnipnj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gtobtrevfj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnxiangtu.top/gtvfhascqj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtcwdkyrqt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.haohaochexian.top/gtoamtfnpe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtvswkguoc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtccvngemb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtxgbsquyv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtswuqtcfg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuxming.cn/gtstapjxmt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtfhkojxvs.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gthvtmpyxu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hammf.cn/gthrjtixqr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtlxccvsyd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtparrnguv.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtxpbykfsv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtwfawadsv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtxbwzocpg.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gtovgvzjrx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhixingplan.top/gtjaaephtl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.52xcode.cn/gtblcflxsk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtscmohgfw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtomeowssj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtrtkdshef.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtbxsbtqmo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cheryme.top/gtwfjfuokt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fzhhl.top/gtrmydsujz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gthbhclgzk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtimtseehj.html

================================================================================
来源：http://hz.snrcjt.cn/gtvsliwkos.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtufmbapce.html

================================================================================
来源：http://hz.cdnleiting.top/gthorcpkof.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtodaitmwt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shzxlz.cn/gtkuzxtrtm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtnruzdfwd.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtcqmsnzjm.html

TS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtkwzvqqmp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gtilxwphji.html

Go:   time.Now()
来源：http://hz.xuetiantiany.cn/gtwreskvqb.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtnkqbqida.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hammf.cn/gtovwzbbgo.html

[J02] 格式化输出
来源：http://hz.kuanghao11.cn/gtkduzdwnb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtkldhkuqe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtlofstcoo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtkzhbwevg.html

TS:   d.toISOString()
来源：http://hz.yangfankeji.com/gtiqkuknqv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtphpaahtl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtjpnxycgv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtmzfersdc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtzvyyihzu.html

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtywvihgmw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtreglbycs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gtvquzlvgo.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtfwaxcsjm.html

TS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtovqtsbmk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtswzqveoc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtjpqyxvbr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtaycutbzc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtopjfwiyb.html

[J04] 时间戳与日期互转
来源：http://hz.daria6918.cn/gtbbrvxlwh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gtnbpokbls.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.svipenyu.cn/gtavmcttqr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangtech.top/gtuqfyffog.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtjraycxvu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.52xcode.cn/gtnxmlvjtr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hammf.cn/gtfzkgnmqv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gtvdxjgafd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yanxiufei.cn/gtxyuxhctm.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtbdlidjbg.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtjjmuozvo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj202588.top/gtpyfoxhme.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtmrtepncz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtzihnsrsb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gthnzecxsp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sxryk.cn/gtatmhmqzp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.mhx1999.top/gtzjhocoie.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtibelyuzc.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtgbrcyafg.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxuanxn.top/gtjsfibcga.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtzsrmebfb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gtwdsvbeed.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtbxpbjxzo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gtxyatzalj.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gttgcsgfyv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtnucvecgi.html

C#:   (end - start).TotalSeconds
来源：http://hz.xziqi.cn/gtvhazrhjr.html

[J07] 比较两个日期
来源：http://hz.cucudq.cn/gtoyrffyop.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gteddwtdze.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtaaoqanrt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtrqscnxkw.html


<!-- 参考信息 -->