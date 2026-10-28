代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.sysykeji.top/gtrnsymwwx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtslvcjxsd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.c1oappe.top/gtzbogyoqd.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtzjbkhper.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtyxzjkkyj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pycfn.com/gtrhcxpsij.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtvjkwuhnw.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtnzzekjjb.html

TS:   public / protected / private
来源：http://hz.jinqigufen.top/gtvwhplawt.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtaiiuuzyt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtnkkcterr.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtuahwfcvt.html

C#:   public / protected / private / internal
来源：http://hz.jianghu66.top/gtahdjqzjh.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtxwrnjhzz.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gtcbxejgav.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtzvevexor.html

JS:   get name() { return this._name; }
来源：http://hz.hammf.cn/gtjvfnfuog.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtdrkhdcti.html

Java: public String getName() { return name; }
来源：http://hz.daria6918.cn/gtvswfhvzw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtbqhygado.html

Ruby: attr_accessor :name
来源：http://hz.ydzc1.top/gteqauafnz.html

C#:   public string Name { get; set; }
来源：http://hz.hnxiangtu.top/gtfaseuxaj.html

[G12] 对象转字符串
来源：http://hz.hnqzz.top/gtwukvixou.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gtciwfyegq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtzjdkvxfi.html

JS:   toString() { return this.name; }
来源：http://hz.fengsongda.top/gtlgqhjytm.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtiykgalwz.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtcyjgfkdg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtnhwkiisa.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtnifkcytu.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtdaqmeqrz.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gttkaswzob.html

Py:   isinstance(u, User)
来源：http://hz.gotoacloud.top/gtbqujmjde.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtzamekftp.html

JS:   u instanceof User
来源：http://hz.smart0.xyz/gtgdfhbxsz.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtomagoilx.html

Java: u instanceof User
来源：http://hz.smart0.xyz/gtbfcvlaic.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtqnynvpda.html

Ruby: u.is_a?(User)
来源：http://hz.zhijiandao.cn/gtejsquphn.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtxdkiuuxh.html

[G14] 数据类 / record
来源：http://hz.c1oappe.top/gtfebrcexu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.vqdsnc.cn/gtjenjvsbf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtzukwwnfh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtrlvmxqqm.html

TS:   type User = { name: string; age: number };
来源：http://hz.meibo888.top/gtlkhjypbc.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtllpzakmq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenjidiqi.icu/gtfhzcbyrn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.redwolf501.top/gtauxvqcvy.html

C#:   record User(string Name, int Age);
来源：http://hz.smart0.xyz/gtzgfcbtwy.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gtacetnxvi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shuidangran.top/gtuozbrztt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtrhipgzhd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tanke756.top/gtdnvdiagd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtcrrwwyge.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtnrbqvnfz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtyukhfbwx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ppjwa.cn/gtdekjhkgh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtnkuceoez.html

[G16] 对象转数组 / 字典
来源：http://hz.zhiwuduotai.top/gtioxwmphp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtczyvdajt.html

PHP:  get_object_vars($obj);
来源：http://hz.jyoumei.cn/gtctxqpyzy.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtytftjtli.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtgemsgxtq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuanzhike.top/gtdkubrdof.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtzovmtwts.html

Ruby: obj.instance_variables
来源：http://hz.vqdsnc.cn/gtumdrqbuu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gtcmadrmkd.html

================================================================================
来源：http://hz.daria6918.cn/gtdafxjkgw.html

H. 异常与错误处理
来源：http://hz.ivvv.top/gtskbnvpfh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtyybdjxnp.html

[H01] try / catch 基础
来源：http://hz.ppjwa.cn/gthrshtkgb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtfykccztv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtvuprsmwf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtmvndayuz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.havefunace.top/gtaoblftbq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gternidcys.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.kuanghao11.cn/gtznnczcjl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydjk.org.cn/gtuptbmmxt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.andypj.xyz/gtmfvjywsc.html

[H02] finally / ensure 收尾
来源：http://hz.52xcode.cn/gtshwtlqnj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnxiangtu.top/gtclydjqnb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gthcocpxtx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gterjdqqvu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtzwlvueim.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtgjsuiwkq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.meibo888.top/gthckrmcfh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sxryk.cn/gteqrqgquf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtojmjbinj.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gtknvofkzs.html

Py:   raise ValueError("错误信息")
来源：http://hz.cdnleiting.top/gtubqjskqi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtuipjzqov.html

JS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtauigpjlz.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gthsrqauht.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtlhaqkhof.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.havefunace.top/gttgmwgjwo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtvjoerdrs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yonumen.top/gtcbyxrhtm.html

[H04] 自定义异常类型
来源：http://hz.havefunace.top/gtnqiewwgy.html

Py:   class MyError(Exception): pass
来源：http://hz.tanke756.top/gtvsdhikdi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gteezgspvx.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtbrssaiee.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtfvgbmkvc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtcpcfxijw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hysaishi.cn/gtvfkvqlxa.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtsdllrvre.html

C#:   class MyException : Exception {}
来源：http://hz.xylfe.cn/gtwghnxsad.html

[H05] 捕获特定类型
来源：http://hz.pycfn.com/gtgxcvchaa.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtozptszdz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sxryk.cn/gtvmjjvzvi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gteafdwmzd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtamwrrbcv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.iojbl.cn/gtravogttc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenzaomai.com/gtgnxfqxuc.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gtgdnwmzwc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shzxlz.cn/gtlczrabxv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtzgpsziud.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gthzqpwfwb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cdnleiting.top/gtsxqsfelm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtaqbtersh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtcvuqdmqe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hfpthk.cn/gtmttujwuo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xylfe.cn/gtzyllixvm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtphxkexxo.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnxiangtu.top/gtsdazxpit.html

[H07] 断言
来源：http://hz.bjfxy.top/gtxvefmxti.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtznptkrtm.html

PHP:  assert($x > 0);
来源：http://hz.xuetiantiany.cn/gtboaupqzn.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtmqsszodj.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtfnaonumd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhixingplan.top/gtenkzdiov.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtezjourxg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtmlwiryao.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daria6918.cn/gtoklsebyu.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtwnwqzpek.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtxyahayrk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhaomingkeji.xyz/gthenqzkbs.html

JS:   e.message;  e.stack
来源：http://hz.svipenyu.cn/gtprlacsyu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtcabdnmsj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zycfv.cn/gtvybyvfua.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtgbrtiphk.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gttnrzxhop.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtzqhwjcku.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gtewrzsxyz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtzqukwooe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.smart0.xyz/gtjdoqgcia.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtqjumojxf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtmgjurhsf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydjk.org.cn/gtkviloymx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gotoacloud.top/gtnfdawbrq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtusfpykgv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gtkytladvk.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtxlolpeuf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtvkejngrc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtenymqkaz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtvnnuchaf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtjyozuthn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtnbljbbzo.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtpqwnshlf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gthxregwof.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtrmqzfzop.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxfpawicp.html

I. 正则表达式
来源：http://hz.cheryme.top/gtvydbjqof.html

================================================================================
来源：http://hz.shuidangran.top/gtpoilhoov.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtedgfvzsr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtedwteqgb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ybcxt.top/gtuhhulzys.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtgucivkdh.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gttrzxliab.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dashuyun.cn/gtvglmzivu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtvocimkwi.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtaswkfwlv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtraapyqxi.html

[I02] 提取所有匹配
来源：http://hz.dianchejie.cn/gthsgkpawb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtomegrnar.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gtpraekcuv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yueranfly.top/gtjxzxddzp.html

TS:   s.match(/\d+/g)
来源：http://hz.yanxiufei.cn/gtqppnlder.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenjidiqi.icu/gtkkqyurrt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtpdeckmlm.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtdboxffqx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jyoumei.cn/gtrtsgmrhq.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtcdkwztrp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtlssjkwbq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gthuwfrruz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtfjdfawzp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.quarkkingdee.top/gtwydqhegr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hysaishi.cn/gtvyyuucen.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangtech.top/gtnrftfuai.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gzhubu.top/gtxqxifajr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtwrnhqjyb.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtyfxbghnl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtlnzjwoml.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnqzz.top/gttloqqupe.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtqefubbkj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtxusnhtic.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gthkzlcbjy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258888.top/gtonfeyoeg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gtjwivmrfp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aibaodan.cn/gtdxkueydm.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtiedprsid.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258.top/gtgwjprxpk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtdzabfffq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtqcbnmaxr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtisxekcyu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtnyrywthz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zycfv.cn/gtolhxaofb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtgwalbxls.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtgbmsczch.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangtech.top/gtlszejwqg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gttqufvqed.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ivvv.top/gtnvrmbmgl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtvaogffyi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtgcgprkzd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtgiieoipl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.iojbl.cn/gtaqxkggmk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtdywxzvlo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtonyndpbe.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtlhzvucex.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hysaishi.cn/gtwtmxnxzx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.havefunace.top/gtxuuitefm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtadvvndmb.html

TS:   /error/gim
来源：http://hz.xziqi.cn/gtufxmgccy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtgevonvmi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.havefunace.top/gtprqefbet.html

Ruby: s.scan(/error/i)
来源：http://hz.hnxiangtu.top/gtzycfaskt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtqowwtuwe.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xinyue.icu/gtorhurojp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuanzhike.top/gtdhdvpbov.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtpkvddnxr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtvzwhcgft.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtgxqbamox.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj202588.top/gtcjhpkctl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtdokfjhss.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yueranfly.top/gtveapzszt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtereqmsmp.html

================================================================================
来源：http://hz.cheryme.top/gtupnjecwr.html

J. 日期与时间
来源：http://hz.chenlongwang.top/gttgxupyjx.html

================================================================================
来源：http://hz.daria6918.cn/gtmsbluwfx.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtirbophtc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtssconpcb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtubtahtyq.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtythuwqyf.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtavgerplx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yueranfly.top/gteobgcsek.html

Go:   time.Now()
来源：http://hz.zhongyouzk.top/gtygoczkxz.html

Ruby: Time.now
来源：http://hz.yongpay.top/gtmryjdlig.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.fzhhl.top/gtgegjsbao.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtofzhxakr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtrlnwjnvz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtswiuxesd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aibaodan.cn/gtmhkncpsm.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtwpmjsiyn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtanbwceoj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtiwylbeqe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtnrrbkkqe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gtkstlaciy.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtwgmfmzmp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pengpengdd.cyou/gtayhdsxka.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gtxycilokt.html

JS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtwbhxfpyx.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtylprzgyv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtunufhhnl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtfyksvupk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtljsphgxq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.smart0.xyz/gtutmhbecf.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtjevhzant.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtdxypkyap.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pengpengdd.cyou/gthshaecuu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtfozxtshi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhaomingkeji.xyz/gtaivklkql.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gthwbwmqpj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hfpthk.cn/gtoretbrds.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ppjwa.cn/gtzkhhafvd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.havefunace.top/gtwfmphdfp.html

[J05] 时间加减（加 7 天）
来源：http://hz.9152youxi.cn/gtlkpwtqof.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtgoobjuid.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gtgxqtddxv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtddjefmzv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtpkzvanzi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gttunbomtp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtrvpprcem.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtqnxrxfrp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtchiexmxo.html

[J06] 计算两时间之差
来源：http://hz.hywenlv.cn/gthtccxoyx.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtlrojhocg.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtkkdogdmy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtzrzbinxy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnxiangtu.top/gtajrugwov.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtgbvoydhd.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtealcylay.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtzcuqtsbt.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gthdcqshrp.html

[J07] 比较两个日期
来源：http://hz.gzhubu.top/gtugzwffjn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtmnhqoetk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtiurmkmrl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtlykwjglm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtvxhjhfot.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtubrxcrbo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtpslkjnkg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtxbfjatln.html


<!-- 参考信息 -->