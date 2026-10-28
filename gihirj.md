代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtitjzolhl.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtgccyjjwp.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtipftofzp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtgrjfzomc.html

JS:   get name() { return this._name; }
来源：http://hz.sweek.top/gtduotncmx.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtdcxaslkb.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtpolnutmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gteaniphsl.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtfngmtmkd.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtkedupgse.html

[G12] 对象转字符串
来源：http://hz.aizwys.cn/gtgdephabi.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gthhrjbgjl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtujrwzgur.html

JS:   toString() { return this.name; }
来源：http://hz.zdqjudy.top/gtlwnlaceu.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtytyhqmvd.html

Java: @Override public String toString() { return name; }
来源：http://hz.xinyue.icu/gtpraysdjb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtcqzzohwx.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtxsknzicp.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gthyotkwpo.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtlxatfsob.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtjmwabpix.html

PHP:  $u instanceof User
来源：http://hz.jlsjyb.cn/gtscowmvww.html

JS:   u instanceof User
来源：http://hz.smart0.xyz/gtlvrugcne.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtpvvsqmwp.html

Java: u instanceof User
来源：http://hz.nanxinkj.top/gtcanuoexg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtznrmqkpq.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtwrglytld.html

C#:   u is User
来源：http://hz.aibaodan.cn/gtoyrgynde.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtoigzyzss.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtzdtbyhbp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.feifeiyinyue.top/gtwtkxlhpv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtoniqskcz.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gttxadoyyb.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtbqqhcsoj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtemzceuff.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.snrcjt.cn/gtmrxpjaci.html

C#:   record User(string Name, int Age);
来源：http://hz.guowangkeji.top/gteyjejclo.html

[G15] 枚举
来源：http://hz.ivvv.top/gtuwfslnyv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtrpszbfbm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tian-w.cn/gtbxynwnfo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gtcjqazmua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtqmbeuurg.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gticahnaow.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuanzhike.top/gtlztwnbyd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hammf.cn/gtdsuvhekp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gteiylavgk.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtnmhjepvo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtzpkbnmbq.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258.top/gtwjcigmvc.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtfiifvvny.html

TS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtiqbsleoi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hfpthk.cn/gtwvxmmanl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtsksuaofc.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gtvixbbhqo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtgwqwusaz.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxfiyxxxb.html

H. 异常与错误处理
来源：http://hz.tian-w.cn/gtepymnxkt.html

================================================================================
来源：http://hz.yanxiufei.cn/gtogigktop.html

[H01] try / catch 基础
来源：http://hz.shzxlz.cn/gtydesxywa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ybcxt.top/gtdkuynmup.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhoulong.xyz/gtqrlnehdu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gttxnmwbli.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gotoacloud.top/gttepvawan.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nwbrower.top/gtstnuzgwk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gtjafkamzf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnqzz.top/gtmfniwuub.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtagwocnqk.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtjlveejuz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.redwolf501.top/gtvfojnmua.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtccmoipya.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtoaeztniw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtlsonthkg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtkcfmwlws.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtgfqathrf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhiwuduotai.top/gthkwtogki.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yongpay.top/gtvznqybsz.html

[H03] 主动抛出异常
来源：http://hz.gotoacloud.top/gtjcumpypv.html

Py:   raise ValueError("错误信息")
来源：http://hz.hongshengwenyu.top/gtxvjwiwld.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtekfjbixq.html

JS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtkalfvfss.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtvjgubjjc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtswpcnnfq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtylwqojgd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.havefunace.top/gtnnhcvxpi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtbbpsvrrn.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gtvhngzulh.html

Py:   class MyError(Exception): pass
来源：http://hz.hfpthk.cn/gtkugqdsxe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtrpgggrqn.html

JS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtusigfssh.html

TS:   class MyError extends Error {}
来源：http://hz.aibaodan.cn/gttzkchlng.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtecauzddt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.vqdsnc.cn/gthpswbnbx.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhijiandao.cn/gtkdpgpete.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtrpthabmy.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtegrltkhb.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtikwmdpxc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.haohaochexian.top/gtdyaisdzb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtysotlqkz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtnhzogupf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tian-w.cn/gtjnqrktmr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.svipenyu.cn/gtrbugomtz.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtrmfsjtce.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gthwwmymbx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hysaishi.cn/gtcdgcvsdt.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gttxoefecv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtidaswrzb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtpglpizne.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtyukucfyt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pycfn.com/gtjwusfuqu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtjbljkbnl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sxryk.cn/gtnwiwptqr.html

C#:   obj?.A?.B ?? default
来源：http://hz.sysykeji.top/gtxvofzqrv.html

[H07] 断言
来源：http://hz.jyoumei.cn/gtgwtcywhf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtfdwncxgf.html

PHP:  assert($x > 0);
来源：http://hz.feifeiyinyue.top/gtqackqeux.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtkjfmxkzc.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtxttvawdh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtdpewgfji.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cashguo.top/gtroalapmo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gtxgxluuis.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ivvv.top/gtvxjgcvxw.html

[H08] 获取错误信息与堆栈
来源：http://hz.hammf.cn/gtxkvikdvu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gttbgiptca.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gttkdknwxb.html

JS:   e.message;  e.stack
来源：http://hz.52xcode.cn/gtesbnoepp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtkkhfnidd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtcuipenfb.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtkfxxetzr.html

Ruby: e.message;  e.backtrace
来源：http://hz.9152youxi.cn/gtxidegrer.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sysykeji.top/gtrlncbqrl.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtvrqfrveu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hywenlv.cn/gtoexvyvhx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cdnleiting.top/gtpazsaspt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xziqi.cn/gtaghkfoaf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtukkxvofd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangtech.top/gtkjegcenh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtlmogwsxr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtruwwfvky.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gtvbptsipf.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtxbbjegox.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.quarkkingdee.top/gtextbraew.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nwbrower.top/gtnddrgbhy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtpaltloan.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gthbvglmhu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtpyqopwbs.html

Go:   defer f.Close()
来源：http://hz.wangdashe.top/gteslifkvg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtixiewjwn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtnjhvdgtw.html

================================================================================
来源：http://hz.cdnleiting.top/gtvdxwgoec.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtrdqckymv.html

================================================================================
来源：http://hz.zhixingplan.top/gtvwmrpelc.html

[I01] 判断是否匹配
来源：http://hz.guowangkeji.top/gtformpwun.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gtlwsvugmc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jlsjyb.cn/gtydtywcjv.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtqxpyejlh.html

TS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtebbepghl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtrbpulyws.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtuokerhkt.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtbqbnyxzu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtwfzbeggc.html

[I02] 提取所有匹配
来源：http://hz.yvedp.cn/gtsbdtwgri.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nwbrower.top/gttphfjjmd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtygbkckip.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenjidiqi.icu/gtvvzchsgq.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtgeoatrqq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gogol.net.cn/gtiasnvzvo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.smart0.xyz/gtbfrodomv.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtvfnlmhis.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sufxvd.cn/gttjfwncpd.html

[I03] 提取捕获分组
来源：http://hz.yanxiufei.cn/gtayfuvplr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cdnleiting.top/gtwprxtvfh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.smart0.xyz/gtycycfpnr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.316326.xyz/gtdxenakga.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jyoumei.cn/gtvwgnqmum.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.daxiang520.top/gtuifjumys.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtjwdxyqel.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hysaishi.cn/gtamfkmdaq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtqkvmwvar.html

[I04] 正则替换
来源：http://hz.ywan-chungtsiang.top/gtvjhdxbxw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinyuanbaomall.cn/gtounmykip.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtyiqvhyrg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtsjbchaqt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtfzoaqvgu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gtotjcdbkp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtqagozjse.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinyuanbaomall.cn/gtxgjhrzzs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gthnbqwkbj.html

[I05] 按正则拆分
来源：http://hz.ywan-chungtsiang.top/gtegfrwyjr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258.top/gtropgmajy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cucudq.cn/gtwzytgqon.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtchjxdecy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtgcrbeaqx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangkeji.top/gtiznfbvap.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gtuujxhqbk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtswnzjnve.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtdiehurlm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fengsongda.top/gtthhuxahe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtnryhxhey.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gthscnwear.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtexmdshqc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtefldbamk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtqenyevsv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgufenzy.top/gthbbvthdy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuanzhike.top/gtaujhcavi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtkghgfhmv.html

[I07] 忽略大小写与多行模式
来源：http://hz.pengpengdd.cyou/gtdwbqbagh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtefijneoz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtxatlfkzb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtdupnmrws.html

TS:   /error/gim
来源：http://hz.yonumen.top/gtdjxewdqk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtngrwzufg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangtech.top/gtjjwftmov.html

Ruby: s.scan(/error/i)
来源：http://hz.hongshengwenyu.top/gtxakilfag.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jlsjyb.cn/gtezoczanq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gttqtkrrdy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinqigfzy.top/gtezdvmpug.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shangyingyoupin.top/gtcwthwgbi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gthemxrqmh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtytwkxrqo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtvljhuwcb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtbyudztxv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtlpjehefr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jianghu66.top/gtxifiiadv.html

================================================================================
来源：http://hz.ehwqpu.com/gtodwjgamo.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtdmmiifgj.html

================================================================================
来源：http://hz.fzhhl.top/gtqznhyadd.html

[J01] 获取当前时间
来源：http://hz.yueranfly.top/gtjyewrpsq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtehgnggab.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtvmmwrloe.html

JS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtxrjtntri.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtoxvlgkvw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtxqqacjyw.html

Go:   time.Now()
来源：http://hz.xuanzx.com/gtbmuwjzjh.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtohivakzw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yangfankeji.com/gtxlkbuppa.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtuxfvowci.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtriaqhkhn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtzqvxwjon.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtbpxsnodt.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtypbgneup.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ppjwa.cn/gtcpzaxveo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zdqjudy.top/gtrkxhdojp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gttehgiqwd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtyzyanead.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtzqkrypig.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xylfe.cn/gtxerloxez.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtowpvfzda.html

JS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtlvvklbhg.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtsqytiice.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtmwiwteng.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtsvdzouqs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtqovnjwzm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gttieraqpn.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtsnkvgazv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hfpthk.cn/gtxdarzxwe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yueranfly.top/gtdfyuyfhj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtlqrhlywm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtgwjkxhwm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtrcwnjiru.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtuclgyhsq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yongpay.top/gtdnvdumzg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cdnleiting.top/gtqrkvhjof.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangdashe.top/gtqabjmhsw.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtjabnluzf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gttxjcwqrz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtbknsxvam.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtlhqjqhpx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtxxsulnxq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gttoyhflsh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtpwxwgzsi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daxiang520.top/gtsgvimbas.html

[J06] 计算两时间之差
来源：http://hz.yonumen.top/gtdfvthjxp.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtneqfgppz.html

PHP:  $end->diff($start)->days;
来源：http://hz.birdmap.top/gtfaqcijuy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtbggczuas.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangkeji.top/gtcyitizhb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gtuwgwxnva.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtcpxtvoup.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtaolrphil.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenlongwang.top/gtzpberdhm.html

[J07] 比较两个日期
来源：http://hz.cheryme.top/gtbpqqgyzz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtitfyotjk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gtnerbqkqo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtbzpguare.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gtkxgesumu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shangyingyoupin.top/gtwxwegzhd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ivvv.top/gtehrcnnpm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtuunyydnl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtrdnfnrdm.html

[J08] 提取年月日与星期
来源：http://hz.zhoulong.xyz/gtsegaxgdl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yvedp.cn/gtxyjhyohe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtnuyigdql.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtxflbvlph.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sweek.top/gtkejcojbg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtipjbvqqs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhoulong.xyz/gtaxtbjzbs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.andypj.xyz/gtownuffcn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gtovvmhqmw.html

[J09] 时区处理
来源：http://hz.jyoumei.cn/gtbrknplko.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtoguuitsr.html


<!-- 参考信息 -->