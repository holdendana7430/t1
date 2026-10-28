代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnxiangtu.top/gttsycqjve.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtvnxfwxve.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xziqi.cn/gtcpbzxdmr.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gtjbvqvxlk.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtcvktupss.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtpengjswv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cdnleiting.top/gtwhyozocj.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydzc1.top/gtgozyjvqs.html

[G10] 访问控制
来源：http://hz.9152youxi.cn/gtkavelyjk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtksdmhikj.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtocjoqpun.html

JS:   #private 字段；其余公开
来源：http://hz.fengsongda.top/gtflnfumme.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gtbxrwwngv.html

Java: public / protected / private / 默认包级
来源：http://hz.9152youxi.cn/gtdijimrwj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtrfexsgqx.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtiwajcyfu.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gtqacbzlpp.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtlmzjcyel.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtrtgxzsni.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtdymxluae.html

JS:   get name() { return this._name; }
来源：http://hz.52xcode.cn/gthvabvhfz.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtjangupem.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtpzxowbld.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtcpcteonf.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtnnrjfnkv.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtmvvhqrwi.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtprbjfmls.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gtziqqolwg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtfclrvyxm.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtwfcuajqy.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtbdswgjnb.html

Java: @Override public String toString() { return name; }
来源：http://hz.yonumen.top/gtjmxfuwzg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtgdjogevv.html

Ruby: def to_s; @name; end
来源：http://hz.jiagoushi.top/gtjbucyizf.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtyephuzuc.html

[G13] 判断对象类型
来源：http://hz.zhengqikj.top/gthhqmkrzb.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gtylokuoyi.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtbzgvekdo.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtogpmphwi.html

TS:   u instanceof User
来源：http://hz.zhengqikj.top/gtgdyanvxm.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtpiocuyzj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gtrwffeibz.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtyenwmocv.html

C#:   u is User
来源：http://hz.xylfe.cn/gtwqvuglfm.html

[G14] 数据类 / record
来源：http://hz.dianchejie.cn/gtlbqcnqnv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtjixqiohr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangshuangyany.cn/gthxzbhvcb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtncubmpkg.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnqzz.top/gtwdzkeeef.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtkvuufysm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shangyingyoupin.top/gtetsmkctr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pycfn.com/gtqaxssuib.html

C#:   record User(string Name, int Age);
来源：http://hz.smart0.xyz/gtrykilbhc.html

[G15] 枚举
来源：http://hz.ywan-chungtsiang.top/gtppienlkb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtudujmxxh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gtypauabdo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.52xcode.cn/gtmyegehbv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtelgxvcmk.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtanrouyld.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtbrmfryzq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtmijxspwd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtwqgerkfd.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtcvikawmy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigufen.top/gtxywsfqtn.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gtiqpcrgwb.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtjrjblzpt.html

TS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtmixohnvi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtdzkmgxfp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ivvv.top/gtmjkavtbx.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtpsbzonph.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gtqvxtozhj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrhfluopg.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtpovocyce.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthqoasniu.html

[H01] try / catch 基础
来源：http://hz.xuanzx.com/gtxnknoavz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtfiwpmsbu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxinkj.top/gtpsggewtw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtqpbjboky.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jiagoushi.top/gtbisbxtdp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtiwzqsvlt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangtech.top/gtqqdpoyow.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtpkisfcfr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jiagoushi.top/gtedsovzah.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtdyycecxt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtduscypwu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtlhfitiwz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gttqoolbkq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtrmfyebjd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtwnkxolvt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangtech.top/gtxzfnbmnb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtmedjylwb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtqspoboob.html

[H03] 主动抛出异常
来源：http://hz.feifeiyinyue.top/gtvihxlfxz.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtnqfbevvh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.birdmap.top/gttbngvowj.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtijdtpclc.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtgqblhpxh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtuudeheqd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gtgdnocqdl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangshuangyany.cn/gtvnqsgynk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtjopjzggb.html

[H04] 自定义异常类型
来源：http://hz.yuanzhike.top/gtmjuirtnb.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtvjlxvpqa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtjdpwjsuu.html

JS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtalzxwhsi.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtnsgeltsc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gthnjhmtaf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gtaysnfmal.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gtivdpzgot.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtsaepbzpd.html

[H05] 捕获特定类型
来源：http://hz.vqdsnc.cn/gtnoesntuc.html

Py:   except ValueError as e:
来源：http://hz.gaohongyu789.top/gtrdwracls.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daria6918.cn/gtylbnsmfm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtegvcivez.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gttkwlwxom.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ywan-chungtsiang.top/gtcmwonkep.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuanzhike.top/gteulvxlbc.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtvlvvdbzp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gtymiobepo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuxming.cn/gtfagvvhaw.html

Py:   value = d.get("k") or default
来源：http://hz.wangshuangyany.cn/gtxnlxmcod.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.iojbl.cn/gtafsspynq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gttrpfwtsk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gticwyprhk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtuwayedtm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gtqiveittu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.snrcjt.cn/gtovpcqzcy.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258.top/gtrpoqzdgm.html

[H07] 断言
来源：http://hz.zhongyouzk.top/gttsaqjbvl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tanke756.top/gtmigbhpmc.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtgjwvprcu.html

JS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtzopovfyr.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gttpxtywwq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtaqxnfnoq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtvxwvphcq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cqqwz.cn/gthjwbehlf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gaohongyu789.top/gtcfkfghuo.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhengqikj.top/gtuwenogdf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sufxvd.cn/gtekesfykq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnxiangtu.top/gtuhgaeudq.html

JS:   e.message;  e.stack
来源：http://hz.zdqjudy.top/gtdoplasln.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtsnndiuah.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gttammgfxp.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtezfnmfxu.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtzjaoartr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xingfuxueyuan.xyz/gtbcdnbcig.html

[H09] 带错误码的异常
来源：http://hz.sxryk.cn/gtzdeglgll.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtykpywbzy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guannengcc.top/gtdmguijit.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtcbalajwu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtanwxqvhq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hammf.cn/gtcaaylfrh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtnwoxcyxb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gtztvlrboc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtghvfzipa.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gtalkyspqp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnqzz.top/gtazkkxhpm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtcxkgpxpf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtjjylhnst.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gttcjcpqul.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gogol.net.cn/gtyoypgrri.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtqrmkmqlw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtowgvujle.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtlbnxflux.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqaavcgmv.html

I. 正则表达式
来源：http://hz.havefunace.top/gtrgtannug.html

================================================================================
来源：http://hz.yuanzhike.top/gtiqnspfud.html

[I01] 判断是否匹配
来源：http://hz.gotoacloud.top/gtwfrwauly.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtybrihkxu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pengpengdd.cyou/gtpslkmexc.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtoyhsawru.html

TS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtbweshsbr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtzhdulzzd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtvylaicec.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtweootepd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gteqddqbbq.html

[I02] 提取所有匹配
来源：http://hz.snrcjt.cn/gtaboojbhz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtkhhsmdmr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hongshengwenyu.top/gtfizfcjhx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gtwawglxza.html

TS:   s.match(/\d+/g)
来源：http://hz.chenlongwang.top/gtxfvhzwbi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gthjhynoxs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shzxlz.cn/gtzmsphwse.html

Ruby: s.scan(/\d+/)
来源：http://hz.yvedp.cn/gttjgnehut.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shangyingyoupin.top/gtwyqpgsxm.html

[I03] 提取捕获分组
来源：http://hz.svipenyu.cn/gtstnrnohm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xziqi.cn/gtcwxmtqhk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nwbrower.top/gtgowawcty.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.bjfxy.top/gtrksqxndv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.vqdsnc.cn/gtxrpyqrye.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gteegsgcqx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xingfuxueyuan.xyz/gtlfsvgoet.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtnejaylhy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtorxdgqmy.html

[I04] 正则替换
来源：http://hz.gaohongyu789.top/gtpzlcbbme.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxinkj.top/gtwnfgclwu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtoschdgrs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtflatozxm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtunuxuzgq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtpfmrakra.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinqigfzy.top/gtlctxfzgc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gthjogwmeo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtgxnxiekg.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtnwtkidug.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtyfohcnxt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sweek.top/gtahttkdtq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtuujyxjeq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtclhkasxk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gtzpekknof.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gtynidtxtv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtjasnwgfb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jlsjyb.cn/gtyxsjkpww.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gthomwtqmg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtkiqskkpf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gtcyisgyuz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtorsirjne.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtsnxjibok.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cheryme.top/gtmcsdgnby.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtuypituhz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hfpthk.cn/gtrlpnrqak.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtaiuyfixo.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtmwamiatt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.0kj1m.cn/gtlutdsuty.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cheryme.top/gtqjjzolov.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hywenlv.cn/gtmhiazbtv.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtbjjvotsi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuanzhike.top/gtnklladcm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nwbrower.top/gthckttmvd.html

Ruby: s.scan(/error/i)
来源：http://hz.jlsjyb.cn/gtpwlhhhxx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtuomtyqzr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.haohaochexian.top/gthbzdednf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtsydzcbya.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtnvkavcxj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtwibruxcg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtxaiixkwp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gttlgajnnh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xingfuxueyuan.xyz/gtmazpkwuq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.c1oappe.top/gthienobdt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gttbftwdmi.html

================================================================================
来源：http://hz.tanke756.top/gtktkkqimg.html

J. 日期与时间
来源：http://hz.daxiang520.top/gtlgwvbdli.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrzjjfapt.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtpnnsukbz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gtrwlrgqkx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtiofifvgp.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtntasifix.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtsldlkujl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gtkzrsmpte.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtauyofrll.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtucomjytn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shangyingyoupin.top/gtraennwpp.html

[J02] 格式化输出
来源：http://hz.fzhhl.top/gtihuletjr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtgiykxjlp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtkaszzkhf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtyrstiigr.html

TS:   d.toISOString()
来源：http://hz.sweek.top/gtxscaxzrc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gturvkhsoh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangshuangyany.cn/gtatkuyomg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtlxwlaobw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gtsknlozqm.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gtpdbzsoue.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtmqogmtkh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gtsjsudxkt.html

JS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtzakueqiy.html

TS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gttukrxlog.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gttrlnrnxx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gtludrqjvn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtebxhhxlh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtpenovaaq.html

[J04] 时间戳与日期互转
来源：http://hz.iojbl.cn/gtevqjurwi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtssslmmiq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gtzmjmvfsj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gttzbhvclw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangtech.top/gtenlpkydn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtpquyuwmk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtmmzuagac.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gtqmxtlosm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtotvlmxqn.html

[J05] 时间加减（加 7 天）
来源：http://hz.zycfv.cn/gtugxialqc.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtahovgahy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtgfpodiso.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gteajoijil.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtzrnaqxjn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shuidangran.top/gtnlcwriuz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtkjtfesin.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhongyouzk.top/gtpcppwbqi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtwhytvydc.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtmtuuydvc.html

Py:   (end - start).total_seconds()
来源：http://hz.chenlongwang.top/gtukxginrc.html

PHP:  $end->diff($start)->days;
来源：http://hz.daxiang520.top/gtnghfaeys.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtamzezjtm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aizwys.cn/gtlazuyxhh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtypajmksy.html

Go:   end.Sub(start).Hours()
来源：http://hz.vqdsnc.cn/gtsznzjdxw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangtech.top/gtqblspsry.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258.top/gtuidettei.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtupniaiou.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtvduscrcd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtshbskknd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtkbsgopfx.html


<!-- 参考信息 -->