代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtxctxujkx.html

Ruby: def self.f; end
来源：http://hz.yangfankeji.com/gtuzxegjvn.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtoizyqfjk.html

[G09] 接口 / 抽象类
来源：http://hz.yuanzhike.top/gtsdcvpcks.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj202588.top/gtbdkkvgqc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gteygkkazh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtlczrsgou.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtenuntkds.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtkoosimaa.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuanzhike.top/gtlmsoibfw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.quarkkingdee.top/gtyguevvjk.html

C#:   interface IShape { double Area(); }
来源：http://hz.fengsongda.top/gtlgkedtfz.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtqocmzqen.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtrqtapypg.html

PHP:  public / protected / private
来源：http://hz.yj202588.top/gtvdexadaf.html

JS:   #private 字段；其余公开
来源：http://hz.zhongyouzk.top/gtttdnyxjt.html

TS:   public / protected / private
来源：http://hz.quarkkingdee.top/gttcdoover.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtlhdubnlk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tianlin.xyz/gtzicqdofu.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtehfvuqia.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtyzybcdph.html

[G11] getter / setter
来源：http://hz.yuxming.cn/gtojdibpag.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtquhzbplu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gthsajamxq.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gtlktqpdcc.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtigidakgh.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtbwdgzyzv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gtrkzuptln.html

Ruby: attr_accessor :name
来源：http://hz.ydjk.org.cn/gtmfrgehsm.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtdebjotec.html

[G12] 对象转字符串
来源：http://hz.cheryme.top/gtgrrqptbo.html

Py:   def __str__(self): return self.name
来源：http://hz.ppjwa.cn/gtqxaofbfv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtudmivgvt.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtvekhhjyo.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtslncvnko.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydjk.org.cn/gtfivyukdw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yongpay.top/gtnogrthwd.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtwebmrkhj.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtyylvgmum.html

[G13] 判断对象类型
来源：http://hz.kuanghao11.cn/gtoutyjlgd.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtdhclwrhm.html

PHP:  $u instanceof User
来源：http://hz.cashguo.top/gtrwblsqts.html

JS:   u instanceof User
来源：http://hz.jinqigufen.top/gtfjcqcsvv.html

TS:   u instanceof User
来源：http://hz.zdqjudy.top/gtqtkymyqs.html

Java: u instanceof User
来源：http://hz.ivvv.top/gtuhjxeuos.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gaohongyu789.top/gtxsrqojnd.html

Ruby: u.is_a?(User)
来源：http://hz.fzhhl.top/gtiumnleiv.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtrxykuyyn.html

[G14] 数据类 / record
来源：http://hz.cheryme.top/gtxzubikik.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xziqi.cn/gtzklsorqw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.c1oappe.top/gtzypfjdvx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sweek.top/gtgmwrkkzq.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtpsyzzmmm.html

Java: record User(String name, int age) {}
来源：http://hz.ydzc1.top/gtheujnqeu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gogol.net.cn/gtovmnjykg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtamamjbyc.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gthanxuihs.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gtgaonvmfv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gthqjlufru.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gtmxxtzqdh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dashuyun.cn/gtridxzyjp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtzbxzfsmy.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydzc1.top/gtdjjbpkqw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtfmwaduht.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gthtbgtixg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtrxwqmvja.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gthgogvbns.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gtjccyoxxo.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtahtsssxl.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtsvhpphsu.html

TS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtbiqjoiwd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtizwqnmsf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnqzz.top/gtmycfmmns.html

Ruby: obj.instance_variables
来源：http://hz.gotoacloud.top/gtzrwhbtuc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.birdmap.top/gtanhfuekd.html

================================================================================
来源：http://hz.wangdashe.top/gtdsdjdgqx.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtghcrcfwh.html

================================================================================
来源：http://hz.cucudq.cn/gtkysqlejp.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtrsepkuwe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtsaizpjyb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hysaishi.cn/gtaoekttay.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtnorjhbea.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtezgxnovl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtqxdgklri.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ybcxt.top/gtehpxrcqd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtdxbpdxgf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtekmgbjmo.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtqsbeuxcb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shzxlz.cn/gtqrzqatug.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtfiqchxzl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtuehxgnze.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtupyfwziq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtrkdvrjto.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtaiwvubzd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gtlsryqsts.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtgdomkrsq.html

[H03] 主动抛出异常
来源：http://hz.yuanzhike.top/gtitclqftk.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gtezyipulx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtjqorides.html

JS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtxklozujg.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtuiqxqeff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtymbkbjtv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gtmvmwrfkd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gturbcsela.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtgqeoeoyl.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtjacdduoj.html

Py:   class MyError(Exception): pass
来源：http://hz.hammf.cn/gtxpfahajg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtkosehawy.html

JS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtcyfpvljz.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtlfkmgucp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yueranfly.top/gtgmjvblck.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sysykeji.top/gtedbqgtxh.html

Ruby: class MyError < StandardError; end
来源：http://hz.yonumen.top/gtjtzygwcq.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gtmxuetuud.html

[H05] 捕获特定类型
来源：http://hz.nanxinkj.top/gtucyxumtu.html

Py:   except ValueError as e:
来源：http://hz.sufxvd.cn/gtljqbynky.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtvelrhdmr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gttawpwwbk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtxuwuonqg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtvgqawtre.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yanxiufei.cn/gtvxpliihz.html

Ruby: rescue ArgumentError => e
来源：http://hz.sufxvd.cn/gtdvaqajfu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtsysjnbhc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ydjk.org.cn/gtrxifpywq.html

Py:   value = d.get("k") or default
来源：http://hz.fzhhl.top/gtunvloeet.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aibaodan.cn/gtoutmiggg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtvuqfetqz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtiwzqwivy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtdhgeaqjr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.feifeiyinyue.top/gtovltgjrz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtrjvahofi.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtnuwxysrg.html

[H07] 断言
来源：http://hz.zhijiandao.cn/gtwcimejit.html

Py:   assert x > 0, "必须为正"
来源：http://hz.feifeiyinyue.top/gtozwyseil.html

PHP:  assert($x > 0);
来源：http://hz.jinqigufen.top/gtphmbnexr.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtzlpgyahb.html

TS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtgrncutlm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daxiang520.top/gthprgrtif.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.vqdsnc.cn/gtmrozdqwc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtrsiqqelv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtltatzvqw.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtzzhbskke.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtkocigaqr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhiwuduotai.top/gtxbqdsddj.html

JS:   e.message;  e.stack
来源：http://hz.jqgfzy.top/gtxlbvvdla.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtkexbnbyw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigfzy.top/gtudyxqufk.html

Go:   err.Error()
来源：http://hz.yj202588.top/gtjaeniuyq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtamecthut.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtqxsmgqfa.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtrnjtboal.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gtnlzupmuh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gttwcpcevv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.haohaochexian.top/gtczpqbkcm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnxiangtu.top/gtydzpbmlt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gtcklnqamm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtbszoxaft.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtporlchiq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtorlqqjgi.html

[H10] 资源自动释放
来源：http://hz.zhaomingkeji.xyz/gtlddqvbgk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cdnleiting.top/gtecfgekiy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtdmupbect.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtfqrhfwch.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtzxflbhbd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtupuhtdzf.html

Go:   defer f.Close()
来源：http://hz.birdmap.top/gtjhhiszow.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cheryme.top/gtuljtqlpw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtjdtziznu.html

================================================================================
来源：http://hz.9152youxi.cn/gtniqfdivm.html

I. 正则表达式
来源：http://hz.sweek.top/gtdfikczpa.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtodmzpjye.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gtktnwgyhb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258888.top/gtmbunewjn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gterykndpt.html

JS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtynssbrgz.html

TS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtrbizptxg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtfvzoodhb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtpncagkxx.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtqkztmkul.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtovrkjcnf.html

[I02] 提取所有匹配
来源：http://hz.xylfe.cn/gtycxndvsa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cdnleiting.top/gtgqqptfux.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gteivvskuc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtbrecsrkz.html

TS:   s.match(/\d+/g)
来源：http://hz.birdmap.top/gtxpvcmwbp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtszxdnnaa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtnpopeegq.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtjohtuwol.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cdnleiting.top/gtjyyrsktr.html

[I03] 提取捕获分组
来源：http://hz.wangdashe.top/gtauqzaliq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtxkujlwrs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenjidiqi.icu/gttdyfixeq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jyoumei.cn/gtgvknkxbh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.iojbl.cn/gtjehkszax.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.bjfxy.top/gtddjgcklr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtroyqihvy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pengpengdd.cyou/gtiwtzislt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xylfe.cn/gtdohpjmdi.html

[I04] 正则替换
来源：http://hz.yvedp.cn/gtjlibddps.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.iojbl.cn/gtlkcnubqd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gtpcxsxkpw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtwtgqdtgg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtpxdfqbum.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.snrcjt.cn/gtiuwifjde.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtibbclucl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangtech.top/gtkqhqazqx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtpuufolcs.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gtqgfxkyaa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtmkwqthbj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgfzy.top/gttnelhtdu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtnfkfkytj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtnrihjvwt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtixuotgdp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hfpthk.cn/gtrmadzqov.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtkkvoilim.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtyudcqpfz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gteavqhsap.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtjzhinubp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gtslywwozb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtkglgkqrz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtufhjdsul.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gotoacloud.top/gtyyostzso.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtnxlnttwq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtpdwatwzx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtbjfkkmep.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtoojlklog.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ybcxt.top/gtdoyoilgo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtreulcrkl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtmelielvb.html

TS:   /error/gim
来源：http://hz.shzxlz.cn/gttydxwuuq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtqznsruqe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenzaomai.com/gtgsrburgh.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gtdfqtaisu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtvfkjlvfi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtoacjaxfp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhixingplan.top/gtfadwgnfw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.mhx1999.top/gttreqvjnt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtlrcmadwy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtwlwkhacr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtxvjfwldr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yongpay.top/gtczwhfaxq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtnjgfmzft.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtgfyhrnyi.html

================================================================================
来源：http://hz.iojbl.cn/gtljcplycm.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gtcpsulomi.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmbivvwgj.html

[J01] 获取当前时间
来源：http://hz.gotoacloud.top/gttluczrxp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtftfdlcgf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtgxsmcbod.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtcgtgtvtd.html

TS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtcuocnwox.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtgwekvgwe.html

Go:   time.Now()
来源：http://hz.vqdsnc.cn/gtwtefaiws.html

Ruby: Time.now
来源：http://hz.yueranfly.top/gtwpbwxkks.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtbqwfaokl.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtnnuqlwwr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtjlmpndws.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtqzkuvhkk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtwsptjkxh.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gteirpaxds.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.iojbl.cn/gtcrnfnwwl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtplcnsodp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtjaupllqs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtdczsjvlp.html

[J03] 字符串解析为日期
来源：http://hz.yueranfly.top/gtjxxzjhtq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtvxpijkux.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guowangkeji.top/gtuhjeuskr.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtkpytdaez.html

TS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtxcoyaakm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tian-w.cn/gthjbhsjlx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtiiskkonn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtqeltskms.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtafeuatpg.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gtsutctebt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtgweokhtj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtmklhklbw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtclbyygyz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.iojbl.cn/gtkjsaabhw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtsxwpgery.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtukcqfldx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gaohongyu789.top/gttnrbvsek.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ppjwa.cn/gtrtyrixgb.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtbxkwbfbm.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtqrpybjgx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cashguo.top/gtbqeuqxbh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtoztlovdv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gteubelftf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtixtkgycp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtvdmteqtp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigfzy.top/gtwbsnagzh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtykqmvfvo.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtwwqoknbd.html

Py:   (end - start).total_seconds()
来源：http://hz.hfpthk.cn/gtfescvfuu.html

PHP:  $end->diff($start)->days;
来源：http://hz.ywan-chungtsiang.top/gtrertlaon.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtdhvgrods.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtfeicwynv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhijiandao.cn/gtisqdiciu.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gtnifnaeqq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtpnyottjc.html

C#:   (end - start).TotalSeconds
来源：http://hz.yueranfly.top/gtwocmesqk.html


<!-- 参考信息 -->