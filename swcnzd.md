代发 wailian999

PHP:  public static function f() {}
来源：http://hz.aizwys.cn/gtbfytkfam.html

JS:   static f() {}
来源：http://hz.gzhubu.top/gtmnefouej.html

TS:   static f(): void {}
来源：http://hz.fengsongda.top/gtyetpbwbu.html

Java: static void f() {}
来源：http://hz.aizwys.cn/gtejvsyzhd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtmcmmhwtj.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtqzqzqzsn.html

C#:   public static void F() {}
来源：http://hz.nwbrower.top/gtcrmrhibk.html

[G09] 接口 / 抽象类
来源：http://hz.ydjk.org.cn/gtokglltkt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gttbuftzun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtnyyixefv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fzhhl.top/gtxzdnhrzi.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtfmrkoagx.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtrkqqvyts.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gotoacloud.top/gtajkhgkin.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhixingplan.top/gttpvhvora.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gteifjkjoh.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gtjfyquhew.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gtjimrcndc.html

PHP:  public / protected / private
来源：http://hz.yvedp.cn/gtlmhluncp.html

JS:   #private 字段；其余公开
来源：http://hz.gogol.net.cn/gtiunspzkv.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gticwxidku.html

Java: public / protected / private / 默认包级
来源：http://hz.hnxiangtu.top/gtgdjhmdab.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gtrwcnbjec.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtyopmpklh.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gtyezdpilq.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gtnuxtshxl.html

Py:   @property 与 @x.setter
来源：http://hz.wangshuangyany.cn/gticllgvpv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtlelvsrjw.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtzqnflmok.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigufen.top/gtwoeymkek.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtrcavpixw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtpdhlrsgw.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtxyuzsyyz.html

C#:   public string Name { get; set; }
来源：http://hz.tanke756.top/gtuyfysfvf.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gtzeawvdde.html

Py:   def __str__(self): return self.name
来源：http://hz.smart0.xyz/gtqcexlqsq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtajkmftmx.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtuokqzemj.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtbnmummsx.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtluwktiac.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtwqtshgft.html

Ruby: def to_s; @name; end
来源：http://hz.jlsjyb.cn/gtyxemoaok.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtkywugdba.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtgqsitavb.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtvjleoajp.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtodbkjlbl.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtdftfcxrl.html

TS:   u instanceof User
来源：http://hz.pycfn.com/gtkwuewkzc.html

Java: u instanceof User
来源：http://hz.pycfn.com/gtzunkclbi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tianlin.xyz/gtfzozrsqz.html

Ruby: u.is_a?(User)
来源：http://hz.aizwys.cn/gttrkrdztm.html

C#:   u is User
来源：http://hz.xinyue.icu/gtzglptqvx.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gtyqglanis.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aibaodan.cn/gtouwrwors.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gogol.net.cn/gtggbgzuon.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ehwqpu.com/gtlnrxlcse.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtakfyyrcs.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtkgdgsmvz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shzxlz.cn/gtzghwnnrh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhiwuduotai.top/gtfdsqqbex.html

C#:   record User(string Name, int Age);
来源：http://hz.ydjk.org.cn/gtumcobdsl.html

[G15] 枚举
来源：http://hz.yuxming.cn/gtsnefnyay.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tian-w.cn/gtbbvhbjbe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daxiang520.top/gtzccysbrm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.vqdsnc.cn/gtmbumvhov.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtwdmondoh.html

Java: enum Color { RED, GREEN }
来源：http://hz.shangyingyoupin.top/gtjemyvreb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtyrlsfwey.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nwbrower.top/gtmojiuezb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtyjdtgsdd.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gteghsyiwd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgufenzy.top/gtbywtqzlc.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtmzknrfqq.html

JS:   Object.entries(obj)
来源：http://hz.316326.xyz/gthjewjkoy.html

TS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gtcxbgygto.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gtzjsjnltk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhixingplan.top/gtpddqsfqc.html

Ruby: obj.instance_variables
来源：http://hz.wangshuangyany.cn/gtwwyaaidy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.meibo888.top/gtffqxnsuy.html

================================================================================
来源：http://hz.nanxuanxn.top/gteahpvahm.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtsxdrcjvp.html

================================================================================
来源：http://hz.316326.xyz/gtypuelusm.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtsitzkeqd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtaiwlzukj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtykgfchqb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtqnsfuulr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pycfn.com/gtnkfmswqe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgfzy.top/gtoizsrfqr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gtpprxuiww.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xziqi.cn/gthxjnaxsc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtrkjnepbm.html

[H02] finally / ensure 收尾
来源：http://hz.gotoacloud.top/gtqwiiknss.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxinkj.top/gtmgqbsqme.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtshbayiwi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtifaqrpty.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtgrywfldn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtwikzhnoy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnqzz.top/gtyhoemaym.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangdashe.top/gtnnjliybi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuanzhike.top/gtdvofsvoe.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtxiwyymxo.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtpcdcyubt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtzedkkiyv.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtxfthfvfd.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gthnpacwer.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtekjiqomb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daria6918.cn/gtejftqcko.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtcvstfmka.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gttggndypt.html

[H04] 自定义异常类型
来源：http://hz.yuxming.cn/gtebbuvisv.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtwlxdrrqa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtcohwacml.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtfmpbifzs.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtgvabshyt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtmeukrzgr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtqowlljds.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtfporxvbn.html

C#:   class MyException : Exception {}
来源：http://hz.guannengcc.top/gtxkrhjyvd.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gttpbrvpyv.html

Py:   except ValueError as e:
来源：http://hz.dashuyun.cn/gtfaylcqwd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daxiang520.top/gtajllaaid.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtpdnkikxg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtibtskmxy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daxiang520.top/gtbqoukzjp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtwegkaxah.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangshuangyany.cn/gtlyldhqvx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtjshzmxnv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuxming.cn/gtnqwfdwew.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtchsjxwev.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtuqspnypz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtfhzsflxr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtqeyolhbk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtjondxgjm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtwrhqkruj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guannengcc.top/gtpbyunghn.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtnqpyaqsq.html

[H07] 断言
来源：http://hz.wangdashe.top/gtwecugwep.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtfwztcvjz.html

PHP:  assert($x > 0);
来源：http://hz.xuetiantiany.cn/gtkdabtvpe.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtbhqjabxm.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtjecwimtc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtgevqtegi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydzc1.top/gtpnctbxob.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtnbphiojv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zdqjudy.top/gtkfkcrcoi.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtmydmiylh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtqvyxnmqq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gtlxisoqgj.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtlacetdrg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtukpknier.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtfthomdza.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gtxybptpph.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gternqcayt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtqqdvczmi.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtbhewojmu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtmvtkmtgo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtaclqvsxn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hysaishi.cn/gtjvqurung.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtymueygwu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtxuzfrkvc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gtdrdaetch.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydzc1.top/gtjhxegmvc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtdskuujdo.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtffmniwnq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jyoumei.cn/gtrwhiuxrt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ywan-chungtsiang.top/gtxcnhuhzf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtpgthbteu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtdpchduif.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgufenzy.top/gtbuwcxsla.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtoywefxah.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtpbbfxvwv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fzhhl.top/gtbcpnsqdt.html

================================================================================
来源：http://hz.ivvv.top/gtrojcoqeq.html

I. 正则表达式
来源：http://hz.birdmap.top/gtcyzbymsp.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmvgnmbmz.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gtglmnmywq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtxvvplpvm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtmrbywxfw.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtlpfftijn.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtkzcdpvwr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtxcgafmyq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtozswcdek.html

Ruby: s.match?(/\d+/)
来源：http://hz.iojbl.cn/gtmsdxggfn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhongyouzk.top/gtyvowgrnd.html

[I02] 提取所有匹配
来源：http://hz.shuidangran.top/gtwhmmtkhb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtxsevuapt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydjk.org.cn/gtzwuusyml.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.andypj.xyz/gtwcjsvfzl.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtkqnigwji.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gttwfxevdb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtyiarvsvy.html

Ruby: s.scan(/\d+/)
来源：http://hz.cucudq.cn/gtfxswtyro.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtglzruhao.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gtcemnibgm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtudhkcsnb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtgtoyzctk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhaomingkeji.xyz/gtxyuccyuo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhijiandao.cn/gtsmawjhem.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtsurotfcq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtrnqtlcpa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtqbhxbagv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pycfn.com/gtqophommh.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gthwrrddih.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtwxzlrpgl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gteaidpdhg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtgozrvalc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtnppstfjq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ppjwa.cn/gtdpyhsvdh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtenosffxg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hammf.cn/gtzpsggqak.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gtxoekujsy.html

[I05] 按正则拆分
来源：http://hz.wangshuangyany.cn/gtfoiepmmj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gtwfeaxolf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gtpbyevgxr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtzqjnbwus.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtaoaiedkq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.pengpengdd.cyou/gttekqresb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hfpthk.cn/gtevczdcdi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtesjvpaos.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gtsangreqd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.vqdsnc.cn/gtejzgcaps.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtmfhgecde.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtftjirnuw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtquaxnkqw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtlxeqsqui.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sysykeji.top/gtwdrhrbjy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtpjqstyty.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtitfrxhov.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtvtwzmhgd.html

[I07] 忽略大小写与多行模式
来源：http://hz.9152youxi.cn/gtfemvwqqk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gogol.net.cn/gtwngfuokk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.iojbl.cn/gtwhzlljuy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtqvakgefe.html

TS:   /error/gim
来源：http://hz.gogol.net.cn/gtfwdhwhbx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenjidiqi.icu/gtzhypqdjv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.feifeiyinyue.top/gtkkbpjulq.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtvtiyzdza.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtzgebejjq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhongyouzk.top/gtkrtljjcq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gthdvdmjrt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gthavsqvrj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtgaikqdbr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtfbcakmkw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yongpay.top/gtezsjeclt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtieibtbyd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtxryggpzf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtuuskjqoj.html

================================================================================
来源：http://hz.gzhubu.top/gtylfmbbhu.html

J. 日期与时间
来源：http://hz.jlsjyb.cn/gttllzraah.html

================================================================================
来源：http://hz.zhiwuduotai.top/gthsnqrbek.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gttapvaawv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pengpengdd.cyou/gtxvynwjsr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtjsiwupqm.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtjowzgnhz.html

TS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtsffcblll.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daxiang520.top/gtmbxixtam.html

Go:   time.Now()
来源：http://hz.hnqzz.top/gtgsjahdre.html

Ruby: Time.now
来源：http://hz.cashguo.top/gthycakqsa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtomtlanaf.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtbiupyoat.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtzihnqxxg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtfqfvfrnf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtpdnayjaj.html

TS:   d.toISOString()
来源：http://hz.xylfe.cn/gtifvsowdo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xziqi.cn/gtixnsurtk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtcxrmfcpo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtrhqoniev.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gthoovnifl.html

[J03] 字符串解析为日期
来源：http://hz.chenzaomai.com/gtstyivjku.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtdalbsmrg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nwbrower.top/gtmudatofy.html

JS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gttzjtynwl.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtklvtebjd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tanke756.top/gtemwrhphv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhengqikj.top/gtacdkggcs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtkljbncto.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtsutfitcb.html

[J04] 时间戳与日期互转
来源：http://hz.jlsjyb.cn/gtnhqjabfy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtnkezabbc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtqshxtkib.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gtucvofhri.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.9152youxi.cn/gtuwvfuqpz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xziqi.cn/gtwdgyltgf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtrbqpapqb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtofjkzgjf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daria6918.cn/gtzpkxbahe.html

[J05] 时间加减（加 7 天）
来源：http://hz.yueranfly.top/gtnskddwnr.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gteumlcytf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuetiantiany.cn/gtobgrcnbg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtmtrfjvpc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtduwwalby.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtjeuomjvm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gtffwlgvvy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xziqi.cn/gtwyfcgafd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangshuangyany.cn/gtcwvfnmth.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtzfclhklx.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtyssuuetp.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtyzedeawj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cucudq.cn/gttxvxoztu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.bjfxy.top/gtxwzkbfrx.html


<!-- 参考信息 -->