代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.zhijiandao.cn/gtsxypanhy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.c1oappe.top/gtqvyengua.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtgqizptmm.html

C#:   interface IShape { double Area(); }
来源：http://hz.aibaodan.cn/gtuyniktxd.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gtotyotzsx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.kuanghao11.cn/gtvzceapwq.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtnjccuwlc.html

JS:   #private 字段；其余公开
来源：http://hz.mhx1999.top/gtxxvqdots.html

TS:   public / protected / private
来源：http://hz.wangshuangyany.cn/gtxeviucjh.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtbtziyang.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.haohaochexian.top/gtjvdxfqrm.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtpkibtypi.html

C#:   public / protected / private / internal
来源：http://hz.zhiwuduotai.top/gtkvurfnpj.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtedfdzgke.html

Py:   @property 与 @x.setter
来源：http://hz.hongshengwenyu.top/gtzcisgbqc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtdscqtajm.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtvxfmmalm.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gtzgunddjv.html

Java: public String getName() { return name; }
来源：http://hz.sufxvd.cn/gtneiiqebb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtilkvjzcs.html

Ruby: attr_accessor :name
来源：http://hz.xingfuxueyuan.xyz/gtfwyuqybw.html

C#:   public string Name { get; set; }
来源：http://hz.cqqwz.cn/gtpaxmepwq.html

[G12] 对象转字符串
来源：http://hz.chenzaomai.com/gtwqobcfoi.html

Py:   def __str__(self): return self.name
来源：http://hz.hammf.cn/gtxivisotm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtquoebmte.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtosphmxzb.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtbwdfjvqb.html

Java: @Override public String toString() { return name; }
来源：http://hz.redwolf501.top/gtnikczmpl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gtpeagflde.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtaakxkdoj.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gttqxwelsi.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtehqejroc.html

Py:   isinstance(u, User)
来源：http://hz.hfpthk.cn/gtohjjztps.html

PHP:  $u instanceof User
来源：http://hz.iojbl.cn/gtywlohgga.html

JS:   u instanceof User
来源：http://hz.guannengcc.top/gtqlbbpilp.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtsugwxgdb.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtbwgcvots.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtiaofjgui.html

Ruby: u.is_a?(User)
来源：http://hz.meibo888.top/gtbsspshwd.html

C#:   u is User
来源：http://hz.tian-w.cn/gtscxtelpv.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtilpzbvqd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtfsbmakhw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.9152youxi.cn/gtazohyulk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xylfe.cn/gtygevgxky.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtmvklohxt.html

Java: record User(String name, int age) {}
来源：http://hz.chenjidiqi.icu/gtsymdsvwv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.c1oappe.top/gtbdwmplpz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtglrizrfy.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258888.top/gtbggmqmal.html

[G15] 枚举
来源：http://hz.yuxming.cn/gtfxlremat.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtzerchkzf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtysmqdmwt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gtbjkuyufx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtfxovxhea.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhoulong.xyz/gtmvwhgnqd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtvtvivfoh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtxpicnzsl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtjibhtzjj.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtzrmgvcpg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yongpay.top/gttghsmryr.html

PHP:  get_object_vars($obj);
来源：http://hz.aizwys.cn/gtxmrgqgeh.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtyvqddujw.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtspsvyktx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gttesjiiin.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.c1oappe.top/gteqvsuqgq.html

Ruby: obj.instance_variables
来源：http://hz.hfpthk.cn/gtoxskbaum.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtckyvjlvb.html

================================================================================
来源：http://hz.sufxvd.cn/gtawkxdwog.html

H. 异常与错误处理
来源：http://hz.cheryme.top/gtsqwgjddd.html

================================================================================
来源：http://hz.gzhubu.top/gttcyscean.html

[H01] try / catch 基础
来源：http://hz.sxryk.cn/gtekqpmtha.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtudsrjrxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigfzy.top/gtqvfbnkkg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtjnbihpaq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtcssevafz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtcklgpass.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.9152youxi.cn/gtfzdcibth.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnqzz.top/gtxkqrvaul.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gteykkokym.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gtwhhgjgru.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gtatosteat.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gttzknawia.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtccwzmosv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtumajghhg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gthffpnkpg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gtjdyelhjv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtvfmowkyq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hongshengwenyu.top/gtpeafnejy.html

[H03] 主动抛出异常
来源：http://hz.cqqwz.cn/gtesxlugxw.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258888.top/gtuipmhzvw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtqffpxhmi.html

JS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtdsknzjli.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtfhbomjgy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.meibo888.top/gtfdhazbaz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ybcxt.top/gtpqnbhlty.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtnmpvvinb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtgislleob.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtzrttsayi.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtdvswiodm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtiaukbfdb.html

JS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtzdkbddxt.html

TS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtyvyhfglg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtjbwshaxh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinghuilouyu.cn/gtzevvfusq.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtlnzfnrod.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtzhlirwxj.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtddljxlua.html

Py:   except ValueError as e:
来源：http://hz.kuanghao11.cn/gthrtjfqao.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinghuilouyu.cn/gtpyxnhyan.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtimhzcajp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtywaldens.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tian-w.cn/gtuuroocsk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gogol.net.cn/gtvrlaavik.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuanzx.com/gtttuxlyui.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtsibcffxz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydjk.org.cn/gtuazbourj.html

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtxhkwffwo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhongyouzk.top/gtzwtqtdph.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtwxzlretb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtvbbyrxfz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.havefunace.top/gtzzangdyi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258888.top/gtyfclrpfn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtrhkciojs.html

C#:   obj?.A?.B ?? default
来源：http://hz.iojbl.cn/gtsdamixho.html

[H07] 断言
来源：http://hz.c1oappe.top/gtrvojbghs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtlmaaskeg.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtfsyamzlp.html

JS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtsbrzdikm.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtzrzpywhk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtjsycfodi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtveansmfq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtrtqiolpw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gthaczodid.html

[H08] 获取错误信息与堆栈
来源：http://hz.fengsongda.top/gtlixwjcvd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtxkmnwwcq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtwyfqksmo.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtrhwkvpye.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gthahbvodc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dianchejie.cn/gtpwbpzeht.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtjogsazgs.html

Ruby: e.message;  e.backtrace
来源：http://hz.52xcode.cn/gttvymaeac.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtifewcqtg.html

[H09] 带错误码的异常
来源：http://hz.shuidangran.top/gthowmudpr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cheryme.top/gtxlolegmc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cashguo.top/gtlbhtlvgu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtgguduhxu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtgfnrjhvk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daria6918.cn/gtsvuxehwl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sysykeji.top/gtwtunwore.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtrnyzcnbt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gtntqirbba.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtxawurjub.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hywenlv.cn/gtyccfrvyq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtqtjddsjj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gtcrnhvjdw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtulgghscu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtjtqngrtf.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtjwncfvgb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtllcgdlgp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtlsrapgus.html

================================================================================
来源：http://hz.ydzc1.top/gthwfpfonl.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtevmeymyg.html

================================================================================
来源：http://hz.andypj.xyz/gtlgwbqczg.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gttnzqnjyq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtjdnlsrdf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhaomingkeji.xyz/gtdysxezrn.html

JS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtrayxwhan.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtnternutf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtmhanltjr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtnfoumrlv.html

Ruby: s.match?(/\d+/)
来源：http://hz.c1oappe.top/gtoippsfqs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.iojbl.cn/gtbaahnyrn.html

[I02] 提取所有匹配
来源：http://hz.hfpthk.cn/gtmmoltswk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gtrythkpud.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gtlydzvyrz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtpmdrqobf.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtpcihkyso.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gthbncugpw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtdhxxghpb.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenlongwang.top/gtotmcngxi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuetiantiany.cn/gtxpeclnkq.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtcpiszguu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtfkulsnob.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hywenlv.cn/gtmamgusdu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shangyingyoupin.top/gtsmsrmghc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gtihtrrtbb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtumyrgwuy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.smart0.xyz/gtznssqubf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtypxdvdfc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinyuanbaomall.cn/gtpvdtqbqq.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtcvaivthe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aibaodan.cn/gtfebjsbtl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtpduaapzn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtsbxunlcn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtmiacmsbs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.redwolf501.top/gtpdfvhtdf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shangyingyoupin.top/gtlglxgdia.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydzc1.top/gtqdayyqbs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gtwhzsgpdh.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gthusibafv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtnurgzrbi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtbitudzac.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtcbvfkrnj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtuldgcnzi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.havefunace.top/gtjcpbdawi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenlongwang.top/gtccobnbhb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtzxvuynzz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhixingplan.top/gtifgqiigb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.iojbl.cn/gtjfndgsvr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtdjgspwil.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydzc1.top/gtodfnwsrq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtofjblltk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtqbfmoodu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhengqikj.top/gtujgbizjz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtvzdyymev.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.316326.xyz/gtptjzbwjl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtprhwklxm.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtyhelbygq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xingfuxueyuan.xyz/gtzydqzvjd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtslqvktxi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtuzvgxils.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtdhjsxhpr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtcbodmmao.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.smart0.xyz/gtgmcmorvg.html

Ruby: s.scan(/error/i)
来源：http://hz.havefunace.top/gtcadxkicv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhoulong.xyz/gtrdbibwvs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhongyouzk.top/gtcvmjuugi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yonumen.top/gtemwvykpf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shzxlz.cn/gtmajtzwib.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtbyymrzzs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtqwbszdeb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtfotmcdsn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cqqwz.cn/gtxnoiwtdh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jlsjyb.cn/gtufisonqf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtbdqgctcp.html

================================================================================
来源：http://hz.zhixingplan.top/gtoslzlmpk.html

J. 日期与时间
来源：http://hz.dianchejie.cn/gtuyxkdxjy.html

================================================================================
来源：http://hz.dianchejie.cn/gtkngxwetz.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtizbyeedb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gthcksrihe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtoestteie.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtkprrlxgv.html

TS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtjemqfygl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtjezmkmuu.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtcwpacxur.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtzoswmmrr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtixrytjta.html

[J02] 格式化输出
来源：http://hz.haohaochexian.top/gtkjobiufy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtxddwednj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtpfczkqxi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtqcpjcusp.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtovzlaoxx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gthfuuccel.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtehbbuyta.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtqftrcaex.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnxiangtu.top/gtdeonhotm.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtsgpxxigf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhijiandao.cn/gtayncpzby.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.smart0.xyz/gtitbcbgrn.html

JS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtveqheidd.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtkhiveyan.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtzabftikl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigfzy.top/gtufemettp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cashguo.top/gtmtypcnub.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtkcrwaqjv.html

[J04] 时间戳与日期互转
来源：http://hz.pengpengdd.cyou/gtqafevbqa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtdcqjsaes.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jiagoushi.top/gtsixdeeqa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtfdzbqpzj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sxryk.cn/gtvntbyzim.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgfzy.top/gtkaaxrmhx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gzhubu.top/gtwvisuwqj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtsgxfopeg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhiwuduotai.top/gthjhrmavv.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gtcfyseqxk.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtvklsxwdi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gzhubu.top/gtwgfcedhr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gttpdvywnx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtborxwqsu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtphsuxfen.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtnbmdfpyk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sxryk.cn/gtjgkzmddw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtossiqulo.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtimultmjt.html

Py:   (end - start).total_seconds()
来源：http://hz.tianlin.xyz/gtjvyycfjj.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtacmeohjo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gtjpreraed.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ehwqpu.com/gtootjhayl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtnikpxeck.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtxnqsulvw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinyuanbaomall.cn/gtrnskuvml.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtzgreitsb.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtrjfwsnwt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtrsrcbcle.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jianghu66.top/gtzcljshbw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gteagcogpg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtsspoevqn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtogmzcnqq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtppgsfjyx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtmwwtyhif.html


<!-- 参考信息 -->