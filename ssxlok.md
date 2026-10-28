代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangtech.top/gtvuzrjubi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgfzy.top/gtllgleedy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fengsongda.top/gtvxxvzoat.html

TS:   interface Shape { area(): number; }
来源：http://hz.shuidangran.top/gtvbqrottl.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gtuzujrxuo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtmqbxqalf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zycfv.cn/gtodgqncoi.html

C#:   interface IShape { double Area(); }
来源：http://hz.ppjwa.cn/gtyjlfwlao.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtrpibvqlp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dianchejie.cn/gtpfudyrnn.html

PHP:  public / protected / private
来源：http://hz.zycfv.cn/gtcljbhrhg.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtlbfjyckm.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtsmvllzst.html

Java: public / protected / private / 默认包级
来源：http://hz.sufxvd.cn/gtfgfckwpe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgfzy.top/gtlygpticv.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gtfdkswlki.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtlgviyaiq.html

[G11] getter / setter
来源：http://hz.chenlongwang.top/gtdsiznuxw.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtsvvkppvv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtjqmuwwxw.html

JS:   get name() { return this._name; }
来源：http://hz.kuanghao11.cn/gtcjskmkdw.html

TS:   get name(): string { return this._name; }
来源：http://hz.jiagoushi.top/gtbgdxzoib.html

Java: public String getName() { return name; }
来源：http://hz.52xcode.cn/gtvnwgqmti.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtzzjxwynw.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtwrntdtug.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258.top/gtaghxgmgo.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtjwlamfyy.html

Py:   def __str__(self): return self.name
来源：http://hz.smart0.xyz/gtlbayeklj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtoubmccrq.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtyqjrtyop.html

TS:   toString(): string { return this.name; }
来源：http://hz.52xcode.cn/gtcycvdovg.html

Java: @Override public String toString() { return name; }
来源：http://hz.c1oappe.top/gtjehibruk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gtygpdpyie.html

Ruby: def to_s; @name; end
来源：http://hz.zycfv.cn/gtdxwlqirq.html

C#:   public override string ToString() => Name;
来源：http://hz.ydjk.org.cn/gtwsnjvefd.html

[G13] 判断对象类型
来源：http://hz.svipenyu.cn/gtyksubeln.html

Py:   isinstance(u, User)
来源：http://hz.zhijiandao.cn/gtklufjcfr.html

PHP:  $u instanceof User
来源：http://hz.sysykeji.top/gtjoqgnoik.html

JS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtzgypkmss.html

TS:   u instanceof User
来源：http://hz.nanxinkj.top/gtcrufgvgx.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtdacynsln.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.snrcjt.cn/gtsjiwxpou.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gtzwxluvvb.html

C#:   u is User
来源：http://hz.sxryk.cn/gtmmnadqws.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtaoyavspt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtmehzkhcf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtrjrpivog.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.vqdsnc.cn/gtpqqttufw.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gthliqtdms.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtijuwuibv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtqnblwwev.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtdkgcuybo.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gtntziupur.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtcstyyscc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtbzeqfqpc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gtfecpvhtz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinghuilouyu.cn/gtoqrqgfqs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtufeorpmq.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtdaealqug.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gogol.net.cn/gtbmkyrkdo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtzxosdgdx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtygjbfedk.html

[G16] 对象转数组 / 字典
来源：http://hz.xylfe.cn/gthagnycrl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtxpjzwxsq.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtnhvcfoyx.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtvdexuklj.html

TS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtgzosfwwd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtxovxlhcl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtylmctkoq.html

Ruby: obj.instance_variables
来源：http://hz.jinqigufen.top/gtahxwczbu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtncroshen.html

================================================================================
来源：http://hz.hysaishi.cn/gtkhnqlphh.html

H. 异常与错误处理
来源：http://hz.ydjk.org.cn/gtlnlaexln.html

================================================================================
来源：http://hz.fengsongda.top/gtqyvfcfhn.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtlidxeclb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.haohaochexian.top/gtruqwmeye.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtpvxmfpfy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtwvxbfned.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtqpxoxjuh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.meibo888.top/gteuoqnjnn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtqnpifthm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tianlin.xyz/gtrisecamc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pycfn.com/gtcrwmcggv.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtgxyejagx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxuanxn.top/gtshffbxzw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtyzizmtww.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gttpdffbas.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtejcpmyfx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtfbgvxfsl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtpjtbzyps.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtzhvkeyct.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtslmaivsl.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtjerrmkur.html

Py:   raise ValueError("错误信息")
来源：http://hz.shangyingyoupin.top/gtfhjwohuu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtxvydkrzm.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtpluzmhng.html

TS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtqzbqhokh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtfrhtvnsf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xylfe.cn/gtjnzprgcg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.haohaochexian.top/gtdmcqoxap.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtvmlolnbm.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gtsxmfjoda.html

Py:   class MyError(Exception): pass
来源：http://hz.9152youxi.cn/gtwugtfkev.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtshfztbtu.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtbyjeqdpx.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtojeqytbo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtmsxtbgfk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtifeeaedu.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinyuanbaomall.cn/gtqvfjsxck.html

C#:   class MyException : Exception {}
来源：http://hz.shuidangran.top/gtexwzqdxb.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtbshlgdnj.html

Py:   except ValueError as e:
来源：http://hz.zhixingplan.top/gthaxtfkva.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sufxvd.cn/gtyvqrfxva.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtufbzpayi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtuyxbboxe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinghuilouyu.cn/gtoqxolhqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gtyhpjidni.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gtxpcmlmfp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtdmejflci.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtdpkjqwxu.html

Py:   value = d.get("k") or default
来源：http://hz.yuxming.cn/gtquzjwhxh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtfvigtltx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gthwgywsox.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtfixqwfyq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtfztejxuq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ehwqpu.com/gtgmfxaqzn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shuidangran.top/gtxrvxjhlp.html

C#:   obj?.A?.B ?? default
来源：http://hz.yanxiufei.cn/gtmuaitqbm.html

[H07] 断言
来源：http://hz.wangdashe.top/gtxzymmttb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gtauoeuzkq.html

PHP:  assert($x > 0);
来源：http://hz.meibo888.top/gtgkxvwofe.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtmmoejkuq.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtiextdtuy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gttlghfzux.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtnfvhxwnd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtbpnyxlht.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gtyetnaouc.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhaomingkeji.xyz/gtyrhdkrpy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtrhesfvjf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtrppioaiw.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtxnyfpbwa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.316326.xyz/gtppsobvrx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yvedp.cn/gtsctbdkjd.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtkvsgrpbf.html

Ruby: e.message;  e.backtrace
来源：http://hz.pengpengdd.cyou/gtgxljesly.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtcpefezxe.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtsldaqkzi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtrnwcekdt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtqwgjpmch.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhijiandao.cn/gtpothkcpz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jlsjyb.cn/gtvgjxbqlt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtgrnpvebv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtnptetowj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtsjpdbkhc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cdnleiting.top/gtjapuvgom.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtekvqirxn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hammf.cn/gtlfmszssx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtkadeighl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhaomingkeji.xyz/gtbtxmpndu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtomvyaahp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258888.top/gtllwenlow.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtoftljuwk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtqbhqnltc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtqmyxjsps.html

================================================================================
来源：http://hz.redwolf501.top/gtepxmpsii.html

I. 正则表达式
来源：http://hz.shuidangran.top/gtybfzdgpi.html

================================================================================
来源：http://hz.9152youxi.cn/gtxvecixaq.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtgduetfng.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gtjxkmbthc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtrmyulyat.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtndbbysal.html

TS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtwqedvudt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgufenzy.top/gtahgdrbgq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ywan-chungtsiang.top/gtqomxcjnu.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtvdghfmrz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.iojbl.cn/gtssjrajmj.html

[I02] 提取所有匹配
来源：http://hz.jinghuilouyu.cn/gtgmhgizan.html

Py:   re.findall(r"\d+", s)
来源：http://hz.smart0.xyz/gtmwzuiimc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtrpjvnpan.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtxbxyjrch.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgufenzy.top/gtdsphudmz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ywan-chungtsiang.top/gtlonueibp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.snrcjt.cn/gthoprjcxk.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtxpytnngf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtbzzwxfkl.html

[I03] 提取捕获分组
来源：http://hz.jinyuanbaomall.cn/gttggfcise.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gaohongyu789.top/gtmwoyjltg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xylfe.cn/gtymxllbxo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.0kj1m.cn/gttaracryi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gtnbwiktcq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtyhhtjqkh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtzpdrlwkf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gthiuwubly.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtkumxdlam.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtpsqgwnlq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtifehcmzz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtceyunltl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtnsjtjtyh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtbnjyfonr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtkeltpvaj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxinkj.top/gtiyokzots.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtwmlaimce.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtoshhctdx.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtdjgjvjmc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gthzgtmeun.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jiagoushi.top/gtejvanist.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtdhsfeuap.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gteumpunrt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.redwolf501.top/gtdhngkgyk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtufhtfnhs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtwbufrwdn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinghuilouyu.cn/gtyqhrsuxg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtwltoqvwo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtjhevczrj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gttzrkmwdx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gteipdczdt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtvnijqciu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigfzy.top/gtfvnrjcen.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhijiandao.cn/gtoabkcyzf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.havefunace.top/gtjmcpjgiq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtthzpmxly.html

[I07] 忽略大小写与多行模式
来源：http://hz.9152youxi.cn/gtwomuawfb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtdepifvuz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aibaodan.cn/gtgtdzktjh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtaedjwzyh.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtcoqvnfjh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtmmscvjrv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zdqjudy.top/gtugiupfap.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtzgvmlzdg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtaaftxpkz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daxiang520.top/gtugpzvukw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yanxiufei.cn/gttkvfoesb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtjxqqinxy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtfrktnhkh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtwlycfpgp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtvzvtmyrz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jianghu66.top/gtncrirbza.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guowangkeji.top/gtfulygnuu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtvgwckbec.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthkbukpbb.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtbchyyelg.html

================================================================================
来源：http://hz.jinqigufen.top/gtahboyfmk.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtgobrghvk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhiwuduotai.top/gtromvhcol.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtminbrlik.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtawqjgllz.html

TS:   new Date();  Date.now()
来源：http://hz.nanxuanxn.top/gtntqlctxk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtvuozulut.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtwgxuoaos.html

Ruby: Time.now
来源：http://hz.zhengqikj.top/gthsapkqcp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.feifeiyinyue.top/gtkztsfuka.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gttlawjvzz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtayymqawe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtueyuxtop.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtbevhamhz.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtpcaebptn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtgtpcpcze.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenjidiqi.icu/gtccucbtwo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtorlcenpz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gtmoeigwtr.html

[J03] 字符串解析为日期
来源：http://hz.yonumen.top/gthbfudmpo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenzaomai.com/gtukkcsqok.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydjk.org.cn/gtlsjwcdjp.html

JS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtxooolueb.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gthvxqolry.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtzmgwbfwb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtrwauwabi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtowaomiez.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtnzrrzewp.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtcapwuwii.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtzdcpeqjs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.feifeiyinyue.top/gtcyaoaspp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xinyue.icu/gtpmgxpbtl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigufen.top/gtweclkbih.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gtsdibjwnv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinghuilouyu.cn/gtpvvogrbd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.andypj.xyz/gtjadyiggw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtddymtyue.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtvqtryfwr.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gtuyxbpmlm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gthlmdwtnx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtvzmpdmac.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtymiyamet.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.havefunace.top/gtxiauhumi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtaqvunvfn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gtsnrfyyvp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtdpjexsiq.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gtuieedmab.html

Py:   (end - start).total_seconds()
来源：http://hz.shzxlz.cn/gttyfsucpb.html

PHP:  $end->diff($start)->days;
来源：http://hz.havefunace.top/gtddnwhtha.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtrwcynvfs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gotoacloud.top/gtcheiizyt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtdjbwlarg.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtjcgtbptd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.vqdsnc.cn/gtecleeyps.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhaomingkeji.xyz/gtbxinetyi.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gtapelwexh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtofxgkaeq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gttmkucbuq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtozlawbxq.html


<!-- 参考信息 -->