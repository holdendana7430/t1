代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtyrmvbwoz.html

Ruby: def self.f; end
来源：http://hz.52xcode.cn/gthiozrejh.html

C#:   public static void F() {}
来源：http://hz.c1oappe.top/gtvxmsugnv.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtehpetwgc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ehwqpu.com/gtfwvdzudi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gtlwiczgjb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yvedp.cn/gteupdvqal.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgufenzy.top/gtptazxldo.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gtuafswglb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtlztqoapj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258888.top/gtljfjolvu.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtunqrvfwz.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtngkdxjvs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gttypannev.html

PHP:  public / protected / private
来源：http://hz.nanxuanxn.top/gtvirqhsqh.html

JS:   #private 字段；其余公开
来源：http://hz.yonumen.top/gteamlzusu.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtvujjtnqo.html

Java: public / protected / private / 默认包级
来源：http://hz.vqdsnc.cn/gtbgufczbb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shangyingyoupin.top/gthzpvxcnm.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtbbkwvhbi.html

C#:   public / protected / private / internal
来源：http://hz.yuanzhike.top/gtkkhfydfh.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtxqbchmsk.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtepodluot.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtpawixhug.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtfbtqnmjy.html

TS:   get name(): string { return this._name; }
来源：http://hz.ybcxt.top/gtyqdezhln.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtkwltecjd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtpjybldbs.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtcuyakinj.html

C#:   public string Name { get; set; }
来源：http://hz.zhoulong.xyz/gtzguwwkvg.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangtech.top/gtjaqgysgf.html

Py:   def __str__(self): return self.name
来源：http://hz.gaohongyu789.top/gtnbtmqxrq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtzxovzzmc.html

JS:   toString() { return this.name; }
来源：http://hz.dianchejie.cn/gtamdzugnn.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtvfdxvbiw.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gtrkkmafsj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jyoumei.cn/gtmjutlnma.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtalgidwkg.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtcacmeyay.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gtxyzsufhm.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtukobxtzh.html

PHP:  $u instanceof User
来源：http://hz.316326.xyz/gteeudgvsu.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtesklnpmx.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtyqdadlru.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtnzfgbtlf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zdqjudy.top/gtarxhjrxg.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtaqfxhigx.html

C#:   u is User
来源：http://hz.tanke756.top/gtnguenlto.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtptwtiomo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shangyingyoupin.top/gtevzrrxjq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtkjupygrz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gzhubu.top/gtneukmdbj.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtughvuoay.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtsdnlkjeo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtjmfzqnqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yangfankeji.com/gtpxtdutzq.html

C#:   record User(string Name, int Age);
来源：http://hz.havefunace.top/gtboogmrji.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtzluynwph.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tian-w.cn/gtxmyinybu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.vqdsnc.cn/gtzolfcumr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtfayeucyi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtlwozagjw.html

Java: enum Color { RED, GREEN }
来源：http://hz.jianghu66.top/gtmuscrgwl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gthdkpzqvv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hammf.cn/gtyguyzbtn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtfkuuxjgs.html

[G16] 对象转数组 / 字典
来源：http://hz.ydjk.org.cn/gtkpbkhlzv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dashuyun.cn/gttaxnauwg.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtkuefjnmr.html

JS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gterlvhviy.html

TS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtxrqaeaiw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gogol.net.cn/gtukmhmplj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtraowagax.html

Ruby: obj.instance_variables
来源：http://hz.gaohongyu789.top/gtjzklzvze.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigufen.top/gtgbxjfwnd.html

================================================================================
来源：http://hz.52xcode.cn/gtoasodtqm.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtrahedoah.html

================================================================================
来源：http://hz.jiagoushi.top/gtavkioxta.html

[H01] try / catch 基础
来源：http://hz.jinyuanbaomall.cn/gttjibssfv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtjpleitil.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtlyrovuej.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtabuobscw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtderxxadb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtjtdlkqvl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtsictihwj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cdnleiting.top/gtibjukwgp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gttbkyaoga.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtmqgnbdwf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxinkj.top/gtfxherwkt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtlobttqet.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtojjpqhlw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtwohhzbls.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtibfqlzyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gthqfebeok.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.mhx1999.top/gtkxmbgozg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtsdrylnfp.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtjujivibn.html

Py:   raise ValueError("错误信息")
来源：http://hz.xziqi.cn/gteqcoaxrn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtvphlpjbm.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtcwinuxhl.html

TS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gthupoumfa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtqquwrtoi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.iojbl.cn/gtenmzfgsc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxinkj.top/gtowuljlmw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtbctuhktl.html

[H04] 自定义异常类型
来源：http://hz.wangdashe.top/gtzrgjlzmb.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtsbhdipqp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gtdowldzsm.html

JS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gterqgwelu.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtsyvetqfd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtiadkvdet.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.birdmap.top/gtsvnazosk.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gtypvvkvek.html

C#:   class MyException : Exception {}
来源：http://hz.haohaochexian.top/gtaxpzyecu.html

[H05] 捕获特定类型
来源：http://hz.zhoulong.xyz/gtheytmbpv.html

Py:   except ValueError as e:
来源：http://hz.yuanzhike.top/gtobuxurbf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gthtbesquj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtdnarkerh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtghimkcvk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinyuanbaomall.cn/gthvszpxfl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtnjclbdui.html

Ruby: rescue ArgumentError => e
来源：http://hz.jiagoushi.top/gteohjeyir.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zycfv.cn/gtetspjuhd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtvlzofqwc.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtnsjrnbak.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtptjjspws.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtgsqehfgg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtyxkmbdxn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtnskoetvd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtlwckqvby.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gthnnzcssx.html

C#:   obj?.A?.B ?? default
来源：http://hz.sufxvd.cn/gtvbbdwqka.html

[H07] 断言
来源：http://hz.jqgfzy.top/gtxdpveguz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gthwtxonbh.html

PHP:  assert($x > 0);
来源：http://hz.0kj1m.cn/gtiqjgstue.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtxddesaij.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtbrkxzipz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtxxpwzqlo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtjkqgxghm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cucudq.cn/gtgqilaxfw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.bjfxy.top/gtiajpeuvt.html

[H08] 获取错误信息与堆栈
来源：http://hz.fzhhl.top/gtzxrjsrqd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxuanxn.top/gtyyrhpyot.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtkuttygxw.html

JS:   e.message;  e.stack
来源：http://hz.meibo888.top/gtuigsdybi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yonumen.top/gtcbsffstu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtfbmhpzvq.html

Go:   err.Error()
来源：http://hz.hnqzz.top/gtodknbixc.html

Ruby: e.message;  e.backtrace
来源：http://hz.ywan-chungtsiang.top/gtsmeiplqv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.havefunace.top/gtefbpiqht.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtkwaqgwre.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtjtwckdch.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtobzcfqxa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtppidyyqg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtnxjcpxca.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.iojbl.cn/gtjmksbllz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.316326.xyz/gtbcbhmzku.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtqaxsmfxl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ivvv.top/gtpcjvvymy.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtnfxisdwl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daria6918.cn/gtaajjpknm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yvedp.cn/gtxrbrdrxo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtcbfqngxl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtrnchnhje.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtgysfmokz.html

Go:   defer f.Close()
来源：http://hz.wangshuangyany.cn/gtdefjtbmv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtbfcjmhow.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtdwjbzdgc.html

================================================================================
来源：http://hz.tanke756.top/gtqbfybwva.html

I. 正则表达式
来源：http://hz.quarkkingdee.top/gtdzhxhoqp.html

================================================================================
来源：http://hz.hammf.cn/gtgvjtpcce.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtepouwjkd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gthposppqp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gtbkovcksk.html

JS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gthoxbyclq.html

TS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtplfmuqzc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gtyerxovxc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yueranfly.top/gtvemaplim.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtnoopxisp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yvedp.cn/gtofyfrhtb.html

[I02] 提取所有匹配
来源：http://hz.ywan-chungtsiang.top/gtwaggqyfr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtevylvazi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtgrnkjuuh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuxming.cn/gtxxxianah.html

TS:   s.match(/\d+/g)
来源：http://hz.tianlin.xyz/gtykltmmmi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigfzy.top/gtvlpqrmpo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.kuanghao11.cn/gtzjlwnxhp.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtrfhxhwrf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fzhhl.top/gtygeuflyb.html

[I03] 提取捕获分组
来源：http://hz.zhengqikj.top/gtjsrcuqut.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtpeinrcsr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtxiutqatx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtjuotwayh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.dashuyun.cn/gtwhxmuwra.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuxming.cn/gtugaqbcyz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtahairpqi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtdvrtjtha.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtdefgsxaq.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtmuegycab.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cucudq.cn/gtuugmhxqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtzxnlspmk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtrniobaol.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtrkdvzmgo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gtkxmbwvar.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.snrcjt.cn/gtarkaxapq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gtxffizgcj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtkrslyxer.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtoxyiagsp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gthjlmabhr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daria6918.cn/gtxyrpxdhg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtpzhpiufr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtbthgnauk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gtedfjxoou.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtqrcykzxp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtumcowoqp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jiagoushi.top/gtldhirrls.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jianghu66.top/gtpnlkqavb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gticghcqtt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daxiang520.top/gtzrgmztzs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtjmidcegm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtwyxjebxq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hfpthk.cn/gtphdzlrrz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yueranfly.top/gtfpjrkkgy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dashuyun.cn/gtssirlooi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtkzdwjqvh.html

[I07] 忽略大小写与多行模式
来源：http://hz.yonumen.top/gtmvxwsxku.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtdhwxgroa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gtgbjzgnhg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtpfchdmgg.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gtctzsjvkw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtygrurxqw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.redwolf501.top/gtblujsvzf.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gthwbfvjmv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gteadpmeyb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tianlin.xyz/gttxefdymc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhaomingkeji.xyz/gtgzdmkvya.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yonumen.top/gtrchtlyzk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtndbfzupy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gthmdapwrp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtsxveenjt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtyygriurz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtvfskxuil.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtbnnhmrjh.html

================================================================================
来源：http://hz.gogol.net.cn/gtukpdjiif.html

J. 日期与时间
来源：http://hz.smart0.xyz/gtsbysheyz.html

================================================================================
来源：http://hz.yonumen.top/gtaczsicsp.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtkevyvldt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gtywcctjte.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtzmzojisj.html

JS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtwhrtvkxn.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtvqmryeoq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtigvvqzmh.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gtjrxjgofk.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtylxmnotl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtdxupepmb.html

[J02] 格式化输出
来源：http://hz.mhx1999.top/gtbzrwveil.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtmzdllkbw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtqlitxjwj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtqowpawvc.html

TS:   d.toISOString()
来源：http://hz.yvedp.cn/gtuvbvycij.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtzfgckaar.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhengqikj.top/gtgmxbjtac.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtgzagtcni.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtxemdvhru.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtcybwfauj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gtwpxtawms.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dashuyun.cn/gtqsfigwir.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtkjhpikoc.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtsdueuaek.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtjsrtiouh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.9152youxi.cn/gtepqljwvc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gthtnmaoul.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.0kj1m.cn/gttvjjbred.html

[J04] 时间戳与日期互转
来源：http://hz.shuidangran.top/gtiszianpe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ppjwa.cn/gtldstczfv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hammf.cn/gtruwhhizs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtzcslbbdk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gtlpgaqfcn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aizwys.cn/gtpjpeokrs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtzvmznoxk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtafyakmwg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sysykeji.top/gtxhyzdiuu.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtxhgunfun.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gttggchlte.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtfionzdoz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtiwxcbzgi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtiemlolxd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtcqidikty.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtlxaovxfw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.smart0.xyz/gtaerkrkfr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtowkubazl.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtkkkxsype.html

Py:   (end - start).total_seconds()
来源：http://hz.svipenyu.cn/gtzpwupjxk.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtbdchwggv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtdedbxvwj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtpthyukmp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtysytxtnf.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gttwejirpd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhoulong.xyz/gtvrweoumb.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtwvbgxmbr.html


<!-- 参考信息 -->