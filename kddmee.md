代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtfvqpuhxi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydzc1.top/gttpcmtviw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhongyouzk.top/gthyrikdiy.html

C#:   interface IShape { double Area(); }
来源：http://hz.kuanghao11.cn/gtkdgmalwy.html

[G10] 访问控制
来源：http://hz.tian-w.cn/gtvdiiwthg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtifbzaque.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtrcovansi.html

JS:   #private 字段；其余公开
来源：http://hz.haohaochexian.top/gtyfwkruhe.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtpzpicnvq.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtjjtodarw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gtnlofbvir.html

Ruby: public / protected / private
来源：http://hz.daria6918.cn/gtjwtasckz.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gthfqguadf.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gttotgfjur.html

Py:   @property 与 @x.setter
来源：http://hz.cashguo.top/gtbwbymcxo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtxetoiqgi.html

JS:   get name() { return this._name; }
来源：http://hz.cucudq.cn/gthjirjkmj.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhijiandao.cn/gtcyixhzgo.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtotntrmjg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xinyue.icu/gtbrabjpdr.html

Ruby: attr_accessor :name
来源：http://hz.hnqzz.top/gtzyxrmfsf.html

C#:   public string Name { get; set; }
来源：http://hz.chenlongwang.top/gtzzqqtvwa.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtndmnnnoq.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtmefoarxs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtoiagnnrc.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtbapbcjnk.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtkeeanguo.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtekurruwd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtkiiieknz.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtnmdvcohp.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gtalxgnrfl.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtoiovkzvz.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtcntsbwbh.html

PHP:  $u instanceof User
来源：http://hz.nanxinkj.top/gtpookvqro.html

JS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtwddianjg.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gthphvltaw.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtfgmszotm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtnizwmcia.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtereelrua.html

C#:   u is User
来源：http://hz.zhixingplan.top/gthlhtgdkf.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtckyyqicz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtvsyelwuy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtjqjlinqh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtmvniossv.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gtxagteemm.html

Java: record User(String name, int age) {}
来源：http://hz.pengpengdd.cyou/gtrdasbvcs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gttqrznsly.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinghuilouyu.cn/gtjmnofriz.html

C#:   record User(string Name, int Age);
来源：http://hz.daxiang520.top/gtlhkqnblp.html

[G15] 枚举
来源：http://hz.gaohongyu789.top/gtayxsaupi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ppjwa.cn/gtmpdicmfw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hywenlv.cn/gthprvsktz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jianghu66.top/gtrpooirlq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtbgoxnjzf.html

Java: enum Color { RED, GREEN }
来源：http://hz.hongshengwenyu.top/gtpclcfjtv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangshuangyany.cn/gtdqyflpqq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuanzhike.top/gtczhengum.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtqqwbmdvy.html

[G16] 对象转数组 / 字典
来源：http://hz.pycfn.com/gtgknbtxhf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtwyfbxjwz.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtbxencdmr.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtapjnkygv.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtodmjsyet.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtgvhcogkr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.snrcjt.cn/gtbyahnstn.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangkeji.top/gtgzpeygqw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gtihohagug.html

================================================================================
来源：http://hz.zycfv.cn/gtgccgjebn.html

H. 异常与错误处理
来源：http://hz.meibo888.top/gtyiejvbet.html

================================================================================
来源：http://hz.tanke756.top/gtaoolcsob.html

[H01] try / catch 基础
来源：http://hz.jinyuanbaomall.cn/gthwyzgomy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cashguo.top/gtflsuwqxl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtjzcdhxjx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtdcuozkcl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.svipenyu.cn/gtknxfvqek.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtnhwncgnj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtesdnjrrk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.redwolf501.top/gtqzvcfqjn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tian-w.cn/gtwobwwwol.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtionumupv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtkfofkmew.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtgdzzzspu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtvkssqwgx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtooftnqrg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtfuzfssjv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtctcephec.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtdwnwgecy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtoigffgjf.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gthtwuarrr.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtqpxqsuhd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtipfnpxvh.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtfubhvhna.html

TS:   throw new Error("错误信息");
来源：http://hz.cucudq.cn/gtlfzndrht.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gthddwtkvm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gttxarquvc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jianghu66.top/gtcjxsfucv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtktrdsyxq.html

[H04] 自定义异常类型
来源：http://hz.jqgfzy.top/gtclcppaeb.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtcqkskfvd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtkvcwexsu.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtorxninnv.html

TS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtesbqrbfq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtkpwbbfxk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.quarkkingdee.top/gtgckdioxz.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtarefqysx.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtsqhuaruy.html

[H05] 捕获特定类型
来源：http://hz.quarkkingdee.top/gtzkkapxbv.html

Py:   except ValueError as e:
来源：http://hz.cashguo.top/gtpbdmtoep.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtyncghwia.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtuyxqaksn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtgujbycik.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhongyouzk.top/gtkqeeptcy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sufxvd.cn/gturjfwmbz.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gtswcyjkpm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtyhxedqxf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtvubfnmxa.html

Py:   value = d.get("k") or default
来源：http://hz.zhaomingkeji.xyz/gthyqwnyou.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtskuxrmuh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtizknlbax.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtdeicekwh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtodzsjugj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gtcgkwvdpp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtwqasirfz.html

C#:   obj?.A?.B ?? default
来源：http://hz.aizwys.cn/gtkjaahkac.html

[H07] 断言
来源：http://hz.cucudq.cn/gtdcznfkor.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangdashe.top/gtukiufsbs.html

PHP:  assert($x > 0);
来源：http://hz.redwolf501.top/gtycbzlvlj.html

JS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gttbqxkixy.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtgzdpbyvm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.svipenyu.cn/gtdvjykbva.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtejugajpr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtcvhwkdin.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtuvrsgcou.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtxnvflttc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.52xcode.cn/gtlrwjheax.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangkeji.top/gtpunedtkc.html

JS:   e.message;  e.stack
来源：http://hz.havefunace.top/gtvuzlubgc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtzhfqztxh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtzyrlhnzy.html

Go:   err.Error()
来源：http://hz.ydzc1.top/gtgahckvsm.html

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gtddpfllyy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydjk.org.cn/gteurrwsgm.html

[H09] 带错误码的异常
来源：http://hz.daria6918.cn/gtrdqehjez.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yongpay.top/gtnajhwazp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtngbibinp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtouidjlsx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtddlsnkoi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtozfgothx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhaomingkeji.xyz/gtuezaklam.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhengqikj.top/gtzddohrbi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.feifeiyinyue.top/gtbyqxibij.html

[H10] 资源自动释放
来源：http://hz.cashguo.top/gtgkwezzfl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtwvjbwtar.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.316326.xyz/gtmvnqfqhb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtpvveipsi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtoisgpocm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gotoacloud.top/gtzeycvxff.html

Go:   defer f.Close()
来源：http://hz.ydjk.org.cn/gtowpmrgeo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtszdbsjbm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.9152youxi.cn/gtkotwrama.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsnsbshoc.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtpjejmfeb.html

================================================================================
来源：http://hz.gaohongyu789.top/gtdlmhxuhu.html

[I01] 判断是否匹配
来源：http://hz.nwbrower.top/gtfzmyovmx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.52xcode.cn/gtibtnavax.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtpsflhkvn.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtgvcwycjq.html

TS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtteiklhfk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtmqlelmwi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangkeji.top/gtzoxhumkw.html

Ruby: s.match?(/\d+/)
来源：http://hz.quarkkingdee.top/gtzqmvxbyb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jyoumei.cn/gtpameghiy.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gttotwcgpk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtkaverbuc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jyoumei.cn/gthjlvmmrw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cqqwz.cn/gtqdxkljlp.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtoieeihat.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gtygrvdkkf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jiagoushi.top/gtlenaicyq.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gthiptlwrj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gtkvptvzyv.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gtyqopzrzg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gaohongyu789.top/gtptkvxsur.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258.top/gtyfypjuml.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtkqyunoxv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnqzz.top/gtrjzzahjh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ppjwa.cn/gtdxclzmeq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtbcfqcmqy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tianlin.xyz/gtvyunvyow.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtsrqgeueh.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtvcfiaeqc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guannengcc.top/gtzhzrlzkt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtygicihhz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtfykofhxd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtldgrlelb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gtbrgaerdw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtxxajlqkl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtavucshoc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtxwjkszwe.html

[I05] 按正则拆分
来源：http://hz.cqqwz.cn/gtsehgtiov.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtlihmgpkj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgfzy.top/gtxvitackh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtbwdzhslx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtcchiuxqy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtxsaxjllz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgufenzy.top/gthccvqhdf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtlksmsqhm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnxiangtu.top/gtokgkdmvk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gtreniuvpj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangshuangyany.cn/gtlewbkwym.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtktimbpju.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtimtndukm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtzccbwdbx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gtdnpgjcya.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtfbushhwy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gtfibavwhj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtltlizmme.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydzc1.top/gtjkejmvyu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fzhhl.top/gtozpgohan.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtwntsmqxp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pengpengdd.cyou/gtfyxpykrd.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtqwdcrcoo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gttyekkiix.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gtvhdortoe.html

Ruby: s.scan(/error/i)
来源：http://hz.0kj1m.cn/gtkzrpfwbk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtsgnvsliu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtxwrnublp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenjidiqi.icu/gteklffesg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daria6918.cn/gtvjnftunn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtkljcrwmu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtarvnrezw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gtneedxbji.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhijiandao.cn/gtykokwdaj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenzaomai.com/gtqlwrtkvn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtfxsyppke.html

================================================================================
来源：http://hz.0kj1m.cn/gtffovrakz.html

J. 日期与时间
来源：http://hz.zhiwuduotai.top/gtisxsdygw.html

================================================================================
来源：http://hz.yongpay.top/gtsxfdicge.html

[J01] 获取当前时间
来源：http://hz.yvedp.cn/gtabefyaew.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj202588.top/gtupraewrv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtaydfzpnq.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtiajzrliz.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtzgbqcfsp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guowangkeji.top/gturjquzsi.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtfupynouh.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtjphjjfyf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangdashe.top/gtjotbksed.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtkjrjtbql.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtwbblupsa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtdjizheup.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.svipenyu.cn/gtuuyzxrwe.html

TS:   d.toISOString()
来源：http://hz.cheryme.top/gtwmrdoyfd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhengqikj.top/gtrdkvybuw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxuanxn.top/gtehuuzkqk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtvawcsyyq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cheryme.top/gtssnjlrvm.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtggubqbww.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtjbaqhdlx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tianlin.xyz/gtmlkzahnh.html

JS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtusiqtwye.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtlkcsgblh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtzgzlveoc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtptwpcmwt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtmsohzdtq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnxiangtu.top/gtivufotdf.html

[J04] 时间戳与日期互转
来源：http://hz.bjfxy.top/gtszhwyitz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtfnxbxrxs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jiagoushi.top/gtbkpiknru.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtlllwplnc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gttxuzreup.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtqbbenvor.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guannengcc.top/gtypmmzxae.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gttvqqagcf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jlsjyb.cn/gtdsuwqoli.html

[J05] 时间加减（加 7 天）
来源：http://hz.ivvv.top/gtieqmmkwq.html

Py:   now + timedelta(days=7)
来源：http://hz.vqdsnc.cn/gtclepuite.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gtaldfkogu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtrnrxzffm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtwvczqlsa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtsbvawpua.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258.top/gtwqainkhm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tianlin.xyz/gtisequjfn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cucudq.cn/gtxgiapkxg.html

[J06] 计算两时间之差
来源：http://hz.nwbrower.top/gtjrubewmi.html

Py:   (end - start).total_seconds()
来源：http://hz.yuxming.cn/gthdfgzsut.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtsesiwlyi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtpjeyckfb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtlzgczvgd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pycfn.com/gtwhzqlert.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtfjkjshbb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cheryme.top/gtlhtnxeru.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gtjgesbygs.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtpzlnrszu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtskemfrjs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tianlin.xyz/gtawshrdno.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtlgksvtob.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtddfszgno.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtmhsxnxto.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtziwdubzz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtmbwtiabl.html


<!-- 参考信息 -->