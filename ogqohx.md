代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jyoumei.cn/gttjqywjpo.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtwbfbqhli.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtbmjeqwgl.html

[G09] 接口 / 抽象类
来源：http://hz.dashuyun.cn/gthdcidxsx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtgsrifusq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtyernxiye.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtqupfhwkg.html

TS:   interface Shape { area(): number; }
来源：http://hz.tian-w.cn/gtdechozdj.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtkwsxddtn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hongshengwenyu.top/gtstskqtqb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtqcxylvkw.html

C#:   interface IShape { double Area(); }
来源：http://hz.hysaishi.cn/gtfcfgpuxn.html

[G10] 访问控制
来源：http://hz.jlsjyb.cn/gtafyktucm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yuanzhike.top/gtsjipfkgm.html

PHP:  public / protected / private
来源：http://hz.zycfv.cn/gtvinandwh.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtanprtakk.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtylbpnimh.html

Java: public / protected / private / 默认包级
来源：http://hz.daria6918.cn/gtatrclyha.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtoqywgrii.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gttqbciadj.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtpwaonboa.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtmlpulzrk.html

Py:   @property 与 @x.setter
来源：http://hz.jyoumei.cn/gtvxajhfwr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtnoqqhopm.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gtexjiizuh.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtvinrabjy.html

Java: public String getName() { return name; }
来源：http://hz.zdqjudy.top/gtsoqdfbid.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nwbrower.top/gtuafmkryc.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangtech.top/gtudlwgilt.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtrsdotboo.html

[G12] 对象转字符串
来源：http://hz.andypj.xyz/gtdijlukvv.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtevuenaem.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtklfrdjtx.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gttollbtmw.html

TS:   toString(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtvjxaoilz.html

Java: @Override public String toString() { return name; }
来源：http://hz.xziqi.cn/gtvigvktqj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtnlmzjhrx.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtfrpntnki.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtnxjsmoov.html

[G13] 判断对象类型
来源：http://hz.jiagoushi.top/gtuvbmzqct.html

Py:   isinstance(u, User)
来源：http://hz.jqgufenzy.top/gtobuqhsla.html

PHP:  $u instanceof User
来源：http://hz.316326.xyz/gtuzjmsngq.html

JS:   u instanceof User
来源：http://hz.jianghu66.top/gtklqztlwm.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtsyhzyglt.html

Java: u instanceof User
来源：http://hz.hfpthk.cn/gtfwexapqt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hywenlv.cn/gtmydhmmqt.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gthjxqwjzx.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtuaztqhou.html

[G14] 数据类 / record
来源：http://hz.guannengcc.top/gteppoelni.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cqqwz.cn/gtkgaabjel.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtnzrzupdj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nwbrower.top/gtudtylqra.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtovdshufl.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gtwhtbcmbe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ppjwa.cn/gthkybuctl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtzcntzqso.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtkosaphbr.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtcwbdqttq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtyxplaryy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.52xcode.cn/gtnwibhgxb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gthitjsjfw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtugqgjjxk.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gtotjpafvz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtvsdcmhuu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gtzfjbolwr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtawrjrnkk.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gtetkloxtn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cashguo.top/gtdtrymhqj.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgfzy.top/gtzatemfkv.html

JS:   Object.entries(obj)
来源：http://hz.sweek.top/gtotwrrfyv.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtayisylbv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gthivpswaw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ivvv.top/gtiawdasme.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtuujkmpbt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenjidiqi.icu/gtddtmqzhd.html

================================================================================
来源：http://hz.birdmap.top/gtyqmrnbhg.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gttwspwlfz.html

================================================================================
来源：http://hz.hnqzz.top/gttbtaouzm.html

[H01] try / catch 基础
来源：http://hz.aibaodan.cn/gtdfampxpc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sxryk.cn/gthduxyymo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtjbqrkcxw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtnwbhqugz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtzwqbmlzd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtvxkxqkeg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtoetmvzbm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtfpeylihh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtbkayygsl.html

[H02] finally / ensure 收尾
来源：http://hz.cqqwz.cn/gttejdtdtn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.svipenyu.cn/gtzskipfkw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtzptcmzku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtcnhcmaxt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gthepakown.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtfhiyetkm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtkvezjvgb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gteixoztwe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtimtqczsj.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtumxlgnsz.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxuanxn.top/gtxgtvwcss.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtwrvfqcsu.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtzuzkkjmd.html

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtcejahusm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtvjdrlhac.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtnibpbytl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guowangkeji.top/gtbrmibgxp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gtspctlyfs.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gttlsgqrgv.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtuluejgeq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daxiang520.top/gtnfryegfi.html

JS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtrbvvuecm.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtzwxbtqrw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtrdnszgcn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtxbyzkako.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtlzzilmyx.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtcnfioywy.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gtpwohvcyf.html

Py:   except ValueError as e:
来源：http://hz.sysykeji.top/gthwvwxorl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtjihthxos.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtreyzhvjc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtaimbjpgn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtgdvroxxn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.vqdsnc.cn/gtgyybrcsd.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtqwtglnzt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtkikzktms.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nwbrower.top/gtesoqpvnk.html

Py:   value = d.get("k") or default
来源：http://hz.ybcxt.top/gtslpmbifp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtbeoyihte.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtvfvcmofq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtmdgzuxfb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtgxwtwchs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtnwtghtbm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.snrcjt.cn/gtembrfgmz.html

C#:   obj?.A?.B ?? default
来源：http://hz.redwolf501.top/gtfhhoqvkn.html

[H07] 断言
来源：http://hz.andypj.xyz/gthmpkxuts.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gotoacloud.top/gtrmnxdozz.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtqintxvvl.html

JS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtdfhhbsln.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtzetokjdu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gtfynyqzrq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.iojbl.cn/gtnnxeklue.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.kuanghao11.cn/gtkriitica.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258888.top/gtyytbxvib.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtqhojdjdm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.feifeiyinyue.top/gtiezqldrj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtbpfqbcyx.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtpjvzjexw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gtgssomnmv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtdsrthpck.html

Go:   err.Error()
来源：http://hz.hongshengwenyu.top/gtjawahyoc.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtqdvrzmpg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnxiangtu.top/gtbkcaqvhw.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gttjgmdfnq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gtsdejepny.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtxzqzphgc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnxiangtu.top/gtzjqwpazv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtceplmkvd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhixingplan.top/gthildyduv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zdqjudy.top/gtyjvgzwsq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cashguo.top/gtqzojmijm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hongshengwenyu.top/gtymqfxshu.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtxzncelfj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.vqdsnc.cn/gtnncebsil.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gtywhothkm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtnjltrmzu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtminohhky.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gaohongyu789.top/gtpkwckcuv.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gttbjfjdhl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtgoanzcwh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.feifeiyinyue.top/gtzluziwyc.html

================================================================================
来源：http://hz.hnqzz.top/gtysopltvs.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtaiuezdlw.html

================================================================================
来源：http://hz.hammf.cn/gtfxnydmpe.html

[I01] 判断是否匹配
来源：http://hz.feifeiyinyue.top/gtsuptenxa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtegkqkndo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gteaidgdji.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtxfieaotn.html

TS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtpfwvplux.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtqunhxtga.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.andypj.xyz/gtdfcwaebq.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtwumomdba.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinyuanbaomall.cn/gtfizjndnm.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gttkyhmbyk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtdvqtivxw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.vqdsnc.cn/gtxntxmptr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtsljndewm.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtktskiget.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtcdtglezu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yvedp.cn/gtrgpuyabk.html

Ruby: s.scan(/\d+/)
来源：http://hz.yanxiufei.cn/gtxoipjwpy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtbkqqlphz.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtvjklczpa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtvznhsovz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtzhqbazfv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.0kj1m.cn/gtfbxfupnk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daxiang520.top/gtplmsbozu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtiawnrrls.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtywsdopqp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.feifeiyinyue.top/gtfatonqel.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtmrzncawg.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtisyzzgqv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.mhx1999.top/gternmetkq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtbspihacs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtdxbtjamw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtaruygcjc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cucudq.cn/gtblgqpkpp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gtitnjzoym.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xylfe.cn/gtjzebrxle.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtamszslrg.html

[I05] 按正则拆分
来源：http://hz.dianchejie.cn/gtelvdugri.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtjkqkmprm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shangyingyoupin.top/gtbueilwrk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtbplpyqvs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtjldcjnvk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtgidimgtk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtiiggxwkl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtsgcplpij.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pengpengdd.cyou/gtlzpumpiw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fzhhl.top/gtbfhncjwz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtaxfdjqep.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.mhx1999.top/gttgblowtv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtbqbburpr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtjqemrzum.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtoqjgcrui.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hongshengwenyu.top/gtbrzlrtlu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xziqi.cn/gtggjradfy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtooewdeqr.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtdsbzadrm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.kuanghao11.cn/gtcmxmukom.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gtkupucgdl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daria6918.cn/gtnzelcmuo.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gteocsqqts.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtgjgfmfoo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtdltpeczg.html

Ruby: s.scan(/error/i)
来源：http://hz.xylfe.cn/gtjywhtcet.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cheryme.top/gthhvmyevj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gtudsycwih.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gteoohaxpc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gzhubu.top/gtfufsgamz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gthkudhcge.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtslbfbiyj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtuacixade.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtoafgrqne.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtwtincsog.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtfqpqeefw.html

================================================================================
来源：http://hz.316326.xyz/gtqhecbdqs.html

J. 日期与时间
来源：http://hz.yueranfly.top/gtssbphczd.html

================================================================================
来源：http://hz.cdnleiting.top/gttbxfmiqt.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtpilrqawj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cqqwz.cn/gtcpdfvcuq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtpeqotjzq.html

JS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtoutmwtxq.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtzcjfqihx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ywan-chungtsiang.top/gtfntncboe.html

Go:   time.Now()
来源：http://hz.zhengqikj.top/gtjdosedaf.html

Ruby: Time.now
来源：http://hz.0kj1m.cn/gtiuzlfmkg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gtounqfhjd.html

[J02] 格式化输出
来源：http://hz.jyoumei.cn/gtwifspnun.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtgbtupbim.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtaplnyirs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yangfankeji.com/gtmpfaucxt.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gtlslsvaum.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.vqdsnc.cn/gtiajiraqm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258.top/gtsibjyifc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtflvgyztf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtbtcgypba.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtmkdyhobs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtxvlpibni.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yueranfly.top/gtsyxjiurv.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtcidrtcgh.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtjwucnrjz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtgtvobzvi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtkexocrpb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtfsiavgpl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtjmktjyen.html

[J04] 时间戳与日期互转
来源：http://hz.tanke756.top/gtkyyterpa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.meibo888.top/gtparkjkyj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtzqcoizae.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gteyzxebtd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtxwhzivbb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtuutumiws.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yanxiufei.cn/gtfamnosgc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzhubu.top/gtunoqhmxz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.birdmap.top/gtwtalevnb.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gtbvsccdcs.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gthdgmpuch.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtjfjduhhf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gttkbehonp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtbiqujlna.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.0kj1m.cn/gtolqiwlhc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sxryk.cn/gtwedgjwxc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.smart0.xyz/gtkwbqihmj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtfsdwnrwk.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtchoeyxhy.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtemmwqzhr.html

PHP:  $end->diff($start)->days;
来源：http://hz.hongshengwenyu.top/gtamhhmapd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gttthxqexc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gtimiyoein.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.birdmap.top/gtscdyybmc.html

Go:   end.Sub(start).Hours()
来源：http://hz.gzhubu.top/gtyoxyurpu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangshuangyany.cn/gtdftahdyz.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gtaajfjptt.html


<!-- 参考信息 -->