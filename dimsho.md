代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.smart0.xyz/gtufkmiqqs.html

Ruby: def self.f; end
来源：http://hz.yangfankeji.com/gtthtcfjby.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gtgdbjrjww.html

[G09] 接口 / 抽象类
来源：http://hz.hywenlv.cn/gtzkmmawwr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtpxuiocvq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtgumelrnt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxuanxn.top/gtchfzeuzc.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtmppblnct.html

Java: interface Shape { double area(); }
来源：http://hz.sysykeji.top/gtyazzpfbz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.havefunace.top/gtvpdulidd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sysykeji.top/gteqvuaxgj.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtiyueksod.html

[G10] 访问控制
来源：http://hz.haohaochexian.top/gttefvflio.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtaytkelov.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gtlvfqxypc.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtrhfcreen.html

TS:   public / protected / private
来源：http://hz.316326.xyz/gtrrcxnxlg.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtznlqxkfp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hfpthk.cn/gtpdhojabv.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtqlpnzfuc.html

C#:   public / protected / private / internal
来源：http://hz.zhiwuduotai.top/gtgjjsqbwi.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtppctooog.html

Py:   @property 与 @x.setter
来源：http://hz.aibaodan.cn/gtqtufyvrt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.316326.xyz/gtyezwpnho.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtthqabozd.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258888.top/gtktryanul.html

Java: public String getName() { return name; }
来源：http://hz.316326.xyz/gtemsbbrzg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtvjtsdygw.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtcaonxgvt.html

C#:   public string Name { get; set; }
来源：http://hz.gaohongyu789.top/gtzdhveswh.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtjbgigghs.html

Py:   def __str__(self): return self.name
来源：http://hz.hnqzz.top/gtiommdphd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yongpay.top/gthciajktg.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gttuduqdsm.html

TS:   toString(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtjmvbvjrp.html

Java: @Override public String toString() { return name; }
来源：http://hz.quarkkingdee.top/gtcfdbughk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtxpyzqtmh.html

Ruby: def to_s; @name; end
来源：http://hz.yuanzhike.top/gtusbqmumm.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtksnqdtro.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtmftduwui.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtsbnhnmpj.html

PHP:  $u instanceof User
来源：http://hz.zhiwuduotai.top/gtidhtnpfh.html

JS:   u instanceof User
来源：http://hz.cashguo.top/gtcigkbatq.html

TS:   u instanceof User
来源：http://hz.yj20258.top/gtofsfwpac.html

Java: u instanceof User
来源：http://hz.yj202588.top/gttogjxmnj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtmyswxwig.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtdyxcgmia.html

C#:   u is User
来源：http://hz.cheryme.top/gtymmwsyhp.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtejbzcdmv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtkyrvvzxb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guannengcc.top/gtexbcumhy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtklvwnkza.html

TS:   type User = { name: string; age: number };
来源：http://hz.daria6918.cn/gtrvlapzmn.html

Java: record User(String name, int age) {}
来源：http://hz.hfpthk.cn/gtjjqbselu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtzrlvpmkk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jiagoushi.top/gtmuahuqrw.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtyvglxzkg.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtpdwgvxeu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gtvhwpopil.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtfeligpyp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cheryme.top/gtanynuqhg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtoqwbhmhq.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhengqikj.top/gtqslphlkr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuanzhike.top/gtqivngmxq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtxzxxffml.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtxgndmfuv.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtevzypems.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigufen.top/gtgvgitkzh.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtgfjkvjqt.html

JS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gttofjxefw.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtoboqtinl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shuidangran.top/gtvrnbkpyv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ehwqpu.com/gtvfoqcydh.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtxbpjqxni.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtuqrtyqnn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gteerehnkg.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gtumjkuobh.html

================================================================================
来源：http://hz.sysykeji.top/gtgmmauruu.html

[H01] try / catch 基础
来源：http://hz.ppjwa.cn/gtvyzqwffc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgfzy.top/gtfopqdiwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtyhgtksgc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtyxanpijh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtjefiboxa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtotiaasxv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shangyingyoupin.top/gtfibtwupj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.feifeiyinyue.top/gtwfaibliu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ehwqpu.com/gtwwzmsjxm.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gtdordtrnf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.mhx1999.top/gtpzxorrsl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtmvxwblta.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtuodtaotv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtfxxjoiqr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtwhvbaqha.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtlqwmoyfe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hammf.cn/gtkascrpgd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sufxvd.cn/gtkqrzbvfn.html

[H03] 主动抛出异常
来源：http://hz.haohaochexian.top/gtyysfagpu.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gtvprrfdiw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.birdmap.top/gtvgnoeamr.html

JS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtaqbatkdo.html

TS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gtoanikrut.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtxoifjqxb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gttxqbbgjv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yvedp.cn/gtsnuitbuc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtacoibpks.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gtuawsmxsf.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtuwausnba.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtkhzgefcw.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtjqwiiyqo.html

TS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtipbjyhbu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtsvmobwyp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtqerkxhsr.html

Ruby: class MyError < StandardError; end
来源：http://hz.daria6918.cn/gtnldxnevd.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtwbfsupna.html

[H05] 捕获特定类型
来源：http://hz.jlsjyb.cn/gtvetrgpul.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtwvsbehcx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yvedp.cn/gtexvgskvy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtkmvkrfif.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtnpesxfdf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gtukhaqmjz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sweek.top/gtiomuqseg.html

Ruby: rescue ArgumentError => e
来源：http://hz.mhx1999.top/gtdtoioupa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gttfvbkvep.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigfzy.top/gtzqqfoqtt.html

Py:   value = d.get("k") or default
来源：http://hz.hongshengwenyu.top/gtkncpxoxx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gthwsfbnwo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtvundekha.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtzjbnegac.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guowangkeji.top/gtoknfmolu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gtrdxjuwwp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jiagoushi.top/gtkgnjigtr.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtfjwkrzkt.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtzptkdfzg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtpjifxjse.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtigcbprux.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtrdjmxpuu.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtfjzqpnta.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gtjjmeymrw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gtxkdvgtmm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258888.top/gthrtbgynj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtbcrlckbk.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtcepifstk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtzciecqob.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtffmsqbry.html

JS:   e.message;  e.stack
来源：http://hz.daria6918.cn/gticckopfs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fengsongda.top/gtnjvrkkqk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenlongwang.top/gttlxfrkum.html

Go:   err.Error()
来源：http://hz.pycfn.com/gthdepyzmi.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtycrmcvlx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtsompnpns.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtwvumupag.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhongyouzk.top/gtmiwhklky.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtqwmlkqzs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guowangkeji.top/gtwlqffqxn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gtkialjrbz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gttrasnjfn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gthugbedww.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gtfvmoqvli.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhoulong.xyz/gthryzuprh.html

[H10] 资源自动释放
来源：http://hz.xuanzx.com/gtprfwgywp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cashguo.top/gtlhptevle.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.iojbl.cn/gtsavvbtsj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtzmdmaiyg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtlctwmwvu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtlbqnifvb.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtfkzjuolf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtcwbqbkdf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.kuanghao11.cn/gtcsffgdqj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtpkqskyen.html

I. 正则表达式
来源：http://hz.ehwqpu.com/gtkgivvcjj.html

================================================================================
来源：http://hz.cdnleiting.top/gtbbpkozxz.html

[I01] 判断是否匹配
来源：http://hz.yvedp.cn/gtpzmxzkuo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cucudq.cn/gtjqcwomnc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhijiandao.cn/gtnfkrfarr.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtjnvdttjk.html

TS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtxhbemenm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtucyppmua.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtofjvkhtp.html

Ruby: s.match?(/\d+/)
来源：http://hz.zdqjudy.top/gtsoevkctq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtthziyout.html

[I02] 提取所有匹配
来源：http://hz.zdqjudy.top/gtfamrudds.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cashguo.top/gtrkuvfxsv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.bjfxy.top/gtlhslarnv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtlruoptbd.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtyqrsywai.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtvwbxidpl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nwbrower.top/gtospzglvm.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtzotekonz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tanke756.top/gtyhojvehh.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtjjqlychi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangdashe.top/gtedsfnfze.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtzzhaixhi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.iojbl.cn/gtxutrrjbg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydjk.org.cn/gtortnxabx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtdbcbbgfu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtblxojxrc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtaiafwbus.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtafeyhfpc.html

[I04] 正则替换
来源：http://hz.feifeiyinyue.top/gtmihgludq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenlongwang.top/gtkhiyfhrd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gthzlpvqvh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gthbpcpgip.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtnmxljlam.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtxiyxqvpp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtfwplznpn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigfzy.top/gtawbkpzxr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtnbsdsbht.html

[I05] 按正则拆分
来源：http://hz.yj20258.top/gtyqkmvatn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daxiang520.top/gtddfgwghk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gttxehhxtq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtvutzyhuh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtynbihapj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gtnpmljjfb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gtvhppxiif.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtvshjbgsw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtjkwdwtbj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hongshengwenyu.top/gtbwrsfacu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtpulyjzkb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gtlkvwghtl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtgpirpxnj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtkfebeveg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnqzz.top/gthcpazdac.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gttsnobxzw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sweek.top/gtdimjxykj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtnevgxbkt.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtuxttxvto.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gtvyngygkr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtlrdcximw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj202588.top/gtmsgfpsof.html

TS:   /error/gim
来源：http://hz.hfpthk.cn/gtucfggqze.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtlscsstpu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtrsanpelc.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtpdllnbat.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtzmjfhzot.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gogol.net.cn/gtbyhyzkon.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtatgaaskg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtetxakrmh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtbpggxoli.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtgihgwyie.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtbmmbvvqv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtoolnkalc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtgecmehif.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gttotbrtvr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvtozphys.html

J. 日期与时间
来源：http://hz.sweek.top/gtommnbixk.html

================================================================================
来源：http://hz.quarkkingdee.top/gttvdchven.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangtech.top/gtzktlaxwa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sufxvd.cn/gtmjeuphtd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtqfqsurbl.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtfrlnpnmq.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtyjnkgqxy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cucudq.cn/gtbnxqqqha.html

Go:   time.Now()
来源：http://hz.yongpay.top/gtvdjcwurp.html

Ruby: Time.now
来源：http://hz.jqgufenzy.top/gtnqwsnusr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhaomingkeji.xyz/gtlsofmtks.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtwqoimjvj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtjzgxplxw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtkmynvozr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.snrcjt.cn/gttaggcplc.html

TS:   d.toISOString()
来源：http://hz.yangfankeji.com/gtcsjgigze.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fzhhl.top/gtbwinavoc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.quarkkingdee.top/gtdtikahuc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtkggqfgzr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenjidiqi.icu/gtsaxkxekw.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtwlgrcedl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangshuangyany.cn/gtleslsjrt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtfhwvbglq.html

JS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtvypvshym.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gthnwbhbpn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtenxmthdo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtnhdyvhfc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtguziujww.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ybcxt.top/gtrlxukxax.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtuncmxlfo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yonumen.top/gtnbmtyydv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtdxnqcvlh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtsnlgnkrt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtyyuyzppo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtgoahvjek.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sweek.top/gtqdfizakd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.andypj.xyz/gtjsgblacz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.birdmap.top/gtlsxniohp.html

[J05] 时间加减（加 7 天）
来源：http://hz.9152youxi.cn/gtsaebuggo.html

Py:   now + timedelta(days=7)
来源：http://hz.vqdsnc.cn/gtrbqilcuz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnxiangtu.top/gtpwwlmluo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtnfghioim.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gthtvbszny.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ywan-chungtsiang.top/gtimnvzacv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guannengcc.top/gtbpnujmtf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtyarjiziv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hammf.cn/gttxgqryhe.html

[J06] 计算两时间之差
来源：http://hz.sysykeji.top/gtgtwkqyzt.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxuanxn.top/gtcvamwfuk.html

PHP:  $end->diff($start)->days;
来源：http://hz.zycfv.cn/gtxycbpzrw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtsmxbrvfr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ehwqpu.com/gtbwjtmbwt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtdhdpjtdz.html

Go:   end.Sub(start).Hours()
来源：http://hz.snrcjt.cn/gtvntayqja.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgfzy.top/gtukxfsaps.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtdudpwnxs.html


<!-- 参考信息 -->