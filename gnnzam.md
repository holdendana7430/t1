代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtfkcdpoyq.html

Ruby: def self.f; end
来源：http://hz.yonumen.top/gtixpkaywj.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtbuczfxqy.html

[G09] 接口 / 抽象类
来源：http://hz.snrcjt.cn/gtxpuylheh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtrzjxznav.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gtenkvbnhv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gttlrvoktg.html

TS:   interface Shape { area(): number; }
来源：http://hz.ywan-chungtsiang.top/gtnhvqcpir.html

Java: interface Shape { double area(); }
来源：http://hz.haohaochexian.top/gtnjzdirkb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.316326.xyz/gthfuxdbhz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtejfgkuah.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtbemmudoe.html

[G10] 访问控制
来源：http://hz.birdmap.top/gtioamvame.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtrumtsypb.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtsuzmsezw.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gttucpecql.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtyzukhyqa.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtirjzbncg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtcpmhaoji.html

Ruby: public / protected / private
来源：http://hz.meibo888.top/gtkceyayjy.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtckrrzcht.html

[G11] getter / setter
来源：http://hz.zhijiandao.cn/gtxfkeregh.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtcbhsscnv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtrvfxqtyc.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtqtjnaxco.html

TS:   get name(): string { return this._name; }
来源：http://hz.yongpay.top/gtvkjzzsip.html

Java: public String getName() { return name; }
来源：http://hz.sufxvd.cn/gtqepkjhlg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtrxzbqtno.html

Ruby: attr_accessor :name
来源：http://hz.gotoacloud.top/gtxpegrtur.html

C#:   public string Name { get; set; }
来源：http://hz.cqqwz.cn/gtnmmtdepr.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtcvpbybfv.html

Py:   def __str__(self): return self.name
来源：http://hz.hammf.cn/gtvfsgsmex.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtzmzewmkp.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtzvgjomvm.html

TS:   toString(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtvkucvjgy.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuetiantiany.cn/gtjmouwefu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtwaknousp.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gthvwsixer.html

C#:   public override string ToString() => Name;
来源：http://hz.zycfv.cn/gtgnbhgcrd.html

[G13] 判断对象类型
来源：http://hz.smart0.xyz/gtqtihzuyu.html

Py:   isinstance(u, User)
来源：http://hz.shuidangran.top/gtipvezfkx.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gteysnauum.html

JS:   u instanceof User
来源：http://hz.yonumen.top/gthhndgaee.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gthexrxsfc.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtrsdxpscu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zdqjudy.top/gtentgtpqz.html

Ruby: u.is_a?(User)
来源：http://hz.gotoacloud.top/gtbzyrfebt.html

C#:   u is User
来源：http://hz.hnqzz.top/gtbyufxsaw.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtinmsseci.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gtyqxmrslg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigufen.top/gtibocfjbl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daxiang520.top/gtwooruitv.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtwqhjuouy.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtxamhdoqq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtvngtqiax.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jyoumei.cn/gtzmdsiahz.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtnlcwsfem.html

[G15] 枚举
来源：http://hz.yongpay.top/gtufjwvmoz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtwvnvliik.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhoulong.xyz/gtnrbvhqrp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtznyhnoxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtctbbvpnj.html

Java: enum Color { RED, GREEN }
来源：http://hz.jyoumei.cn/gthaitmeld.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtvdvwymde.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtviphnwnk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtwwoqezdp.html

[G16] 对象转数组 / 字典
来源：http://hz.ydjk.org.cn/gtmgldpdyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtdrfaffwz.html

PHP:  get_object_vars($obj);
来源：http://hz.hnqzz.top/gtfxeqzjaf.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtuylobpxz.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtktmgicbl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtqfauaxfp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtvuaikynj.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtykkfdlqp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtjdvgfwya.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjqdiibdo.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gthwyysqnh.html

================================================================================
来源：http://hz.daria6918.cn/gtbvejkwpo.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gttrmsterk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ywan-chungtsiang.top/gtbhwybwre.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jyoumei.cn/gtckxzfcnc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtjqpzxvhl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtmowbjrgx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gaohongyu789.top/gtjevhwarn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnxiangtu.top/gtpbtlcpyf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.52xcode.cn/gtrwfnzglp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ybcxt.top/gtviufwrmo.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtafrnkhev.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dianchejie.cn/gtwwwqiqbt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtdiuewzuv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtnqbaomhp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtfjjwrked.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtzxfksazd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtncposjbp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinghuilouyu.cn/gtkiphovff.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cdnleiting.top/gtfwjdubjf.html

[H03] 主动抛出异常
来源：http://hz.yvedp.cn/gtsrlknjle.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhiwuduotai.top/gtftnrltjt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gthbeewmss.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtifedagee.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtmeoouefg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtsbmmcydu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yvedp.cn/gtpdvhnxel.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtddkrvmef.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtyfjjucrc.html

[H04] 自定义异常类型
来源：http://hz.wangshuangyany.cn/gtynmjizod.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gtpqmoastg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtpyxexvcw.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtjaivlxct.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtghxwpmzl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtwybjlwby.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtohnvamxa.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydjk.org.cn/gtdcjjbfgx.html

C#:   class MyException : Exception {}
来源：http://hz.havefunace.top/gtlprwbqoy.html

[H05] 捕获特定类型
来源：http://hz.guannengcc.top/gtbjebjkqo.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtwnmvyuiu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtlxxddzvh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtfioaxdkt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtbjquctnn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.52xcode.cn/gtybwliduo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hongshengwenyu.top/gtgnckrviv.html

Ruby: rescue ArgumentError => e
来源：http://hz.aibaodan.cn/gtufchnwds.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ivvv.top/gtjgwylnzk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtxolkpdhf.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtdliyrffv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtzgpcwfwz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtrxabgxaa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtjqocvlql.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtondlucac.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.0kj1m.cn/gtaowhyvxh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtssqkextw.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtdpwffwom.html

[H07] 断言
来源：http://hz.jinqigfzy.top/gtoaahvkfu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gtkmgpreho.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtmowfnnqo.html

JS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtwdvplicr.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtvpgpepph.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtyckeckjc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fengsongda.top/gtsnwvsfeh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtdlbqurvs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtwgviltcv.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtrszhzkfc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtiyqfzhas.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtlrbrtdcb.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtazaxsqnb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhoulong.xyz/gtodelcxxe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtdlpxsftw.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtokrtupfw.html

Ruby: e.message;  e.backtrace
来源：http://hz.dianchejie.cn/gtldegvham.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtpzxmhmxr.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtxxjkylck.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtdhqmszpi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtgtuwmvcc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtzlbsqrzd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtucpqyvkp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.0kj1m.cn/gtoausrnwc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenjidiqi.icu/gtoxgiwsag.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtuyjavqev.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gthejslqqn.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtgvdkvecp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtqqrdzrhw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.0kj1m.cn/gthlmrkpye.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtbxxqgand.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gttefzwjzu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gtoigdwflw.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtoifbuqxm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenlongwang.top/gtcpwjzeut.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.bjfxy.top/gtfmavfxff.html

================================================================================
来源：http://hz.316326.xyz/gterfwtduq.html

I. 正则表达式
来源：http://hz.ydjk.org.cn/gtqabvzppc.html

================================================================================
来源：http://hz.dianchejie.cn/gtuctzstxt.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtayrzfpcl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tianlin.xyz/gtrsiwxwbh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jlsjyb.cn/gtflfdkwtb.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtkcvaryoo.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtmgathykl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gteixcuvlk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tian-w.cn/gtyynigowg.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtmhreuyfq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cucudq.cn/gtfkbgzizz.html

[I02] 提取所有匹配
来源：http://hz.yuxming.cn/gtycahqchy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtqmpzxyvo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtxrpvbbzp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sufxvd.cn/gtjepsvxay.html

TS:   s.match(/\d+/g)
来源：http://hz.yongpay.top/gttvapipya.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtszxbcekw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gtpdlqveks.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtmzcdjikb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtixvhuthc.html

[I03] 提取捕获分组
来源：http://hz.9152youxi.cn/gtofzkonor.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydjk.org.cn/gtymoyfapk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigufen.top/gtnxgwdpfv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtfrhrzker.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pycfn.com/gtcqfqdoch.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gtepkuwmky.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenjidiqi.icu/gtkkoxoqkg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgufenzy.top/gtuvrjqzir.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtwawsaiyj.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtzotywkaz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.redwolf501.top/gtfhelzibe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtwtwiizhb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtmbryrknw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtecofmwcr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtwgwfyoxk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtkhocnvgr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtmakmalob.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtdnmjnpre.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtsngynnww.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtipqbtohl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gtxdpenxaw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtjzjzmjuh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtrceptiss.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtahhkbotj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigfzy.top/gtpqnnblae.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtdmbdifiy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj202588.top/gtlapyuedi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj202588.top/gtslzqbgyv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtwqhbzcwe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gtlwieogrr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtenvbxmls.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtkhnoarti.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtbsjqlewf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gtjlcbpciv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xinyue.icu/gtxfietzia.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtdowwdlrz.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtlmhrjzov.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtlwltrxzo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtmaihgsky.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtiafyalts.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtvnjytmos.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinghuilouyu.cn/gtwbuvylys.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.wangshuangyany.cn/gttaxtlqqr.html

Ruby: s.scan(/error/i)
来源：http://hz.yueranfly.top/gtnhdlobkk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yongpay.top/gthcnhdhhh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tianlin.xyz/gtzkkmsbqe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gtsbyqauxc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aizwys.cn/gtfzwtagkx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtbmepzwic.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtdrqdybpg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtwegjvvmq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtqrtchrfg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtualnofqx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gttikzvmfq.html

================================================================================
来源：http://hz.guowangkeji.top/gtogxrvjec.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtddongteo.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmkxfswye.html

[J01] 获取当前时间
来源：http://hz.xuetiantiany.cn/gtlwciqgbe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jlsjyb.cn/gtulxxgifs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtemqyhatj.html

JS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtncbobztm.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gthdqyzgui.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtaacsefpq.html

Go:   time.Now()
来源：http://hz.316326.xyz/gtzouksbdr.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtovgjdgns.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.snrcjt.cn/gtwlohjdix.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtcvsbqbri.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtkmtiptsu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtwtkjesrh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtvbpueqqj.html

TS:   d.toISOString()
来源：http://hz.aizwys.cn/gtrmylsihm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtrwqcxqsd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daxiang520.top/gtswdchxwh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtijexqoqw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shangyingyoupin.top/gtrbimgzdn.html

[J03] 字符串解析为日期
来源：http://hz.shzxlz.cn/gtinpzrnxt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenzaomai.com/gtqoledvvl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gogol.net.cn/gtomowexyu.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtgmgcrvef.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtxhpmgdgf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtcxnoulww.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtztdywhlo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ivvv.top/gtxhwerzbl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtmeppdlqw.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gttvjnbzhu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yanxiufei.cn/gtyvwztxhx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hammf.cn/gtvghkisvn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtmvjqvuil.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtybqmcpju.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fzhhl.top/gtlaxgghlp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pengpengdd.cyou/gtojbptbpp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gteogvtzgi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gtlstjcmvo.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtfessrvgo.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtxmymytdz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtaposgdou.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtmorxdywi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtqbmfzhme.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.9152youxi.cn/gtibopnxnv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtqmfublzm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgfzy.top/gtvvaesdal.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinyuanbaomall.cn/gtsbzgaxxr.html

[J06] 计算两时间之差
来源：http://hz.sysykeji.top/gtmeesshxp.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtuodzirkc.html

PHP:  $end->diff($start)->days;
来源：http://hz.birdmap.top/gtybxgctbz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtcenwchae.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ppjwa.cn/gtwbdazxmg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sweek.top/gtppjoqfiz.html

Go:   end.Sub(start).Hours()
来源：http://hz.zycfv.cn/gtcxhxezdz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigfzy.top/gtemdipxrg.html

C#:   (end - start).TotalSeconds
来源：http://hz.dashuyun.cn/gtpadhjifz.html


<!-- 参考信息 -->