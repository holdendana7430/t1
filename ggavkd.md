代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtxckyxshq.html

JS:   toString() { return this.name; }
来源：http://hz.gotoacloud.top/gtpdmyxkfh.html

TS:   toString(): string { return this.name; }
来源：http://hz.fengsongda.top/gtbpjpapgu.html

Java: @Override public String toString() { return name; }
来源：http://hz.xinyue.icu/gtfajgeqwc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtgcgvcruf.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtorvtdxwi.html

C#:   public override string ToString() => Name;
来源：http://hz.jinyuanbaomall.cn/gttvubupmj.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtyvlslvrn.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtocjvjeuw.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtabvwklzx.html

JS:   u instanceof User
来源：http://hz.c1oappe.top/gtcymiopxo.html

TS:   u instanceof User
来源：http://hz.9152youxi.cn/gtrylyjvir.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtdixfxrlb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtzqqcqkoq.html

Ruby: u.is_a?(User)
来源：http://hz.yangfankeji.com/gtmtqwultk.html

C#:   u is User
来源：http://hz.yueranfly.top/gtecjymboz.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtwggzibmb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hywenlv.cn/gtqklqfadx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtphygxpgd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gtvoxzpmtq.html

TS:   type User = { name: string; age: number };
来源：http://hz.birdmap.top/gtcnovymhl.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtqjlhryca.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xylfe.cn/gtquispefo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hongshengwenyu.top/gtijjpspqr.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gtdqlozuss.html

[G15] 枚举
来源：http://hz.gaohongyu789.top/gtuiuabhri.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gthopxvpot.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gttnaltzmp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gtkcmfxcoz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtsmuzumos.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangkeji.top/gtcryvddmx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtqohgfmco.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtoqkesllm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gthxqlbbbn.html

[G16] 对象转数组 / 字典
来源：http://hz.zhixingplan.top/gtneqmqcbf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuanzx.com/gtjqpgowcb.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gteraljprp.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gteeaszzph.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtduigacoi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtwenlueeo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtfvnsgssu.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gtnbbhtnap.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtqeqtalsa.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtcncedghx.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtvvxfpcfk.html

================================================================================
来源：http://hz.quarkkingdee.top/gtenrsxcem.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gthdxhkova.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gtbmzgbyjb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cqqwz.cn/gtibxixwuz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtsazwbwsd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtwuthosui.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtsqwmewrw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtnjhaabez.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtdcxbmuru.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gogol.net.cn/gtigazcahi.html

[H02] finally / ensure 收尾
来源：http://hz.meibo888.top/gtohawgovf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtxwodhjxw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtrxejwigu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gthldqdyqs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gttmamyvle.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtlaezvyuq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gtjstqbpff.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gtvjtxjfej.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtsroskxnw.html

[H03] 主动抛出异常
来源：http://hz.jinqigufen.top/gttkfukfiy.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtviurjxcl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gthkbwhkto.html

JS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtsxgqbcfr.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtyfwgccmk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtsllghpnj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtacquuuxm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cqqwz.cn/gtzkhtlmnn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zycfv.cn/gttuaxxktk.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtzepklkdo.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gtsdlpjhyq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gthedaphuc.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtajizeorv.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtqnjdgyst.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtyzdhfuax.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pycfn.com/gtzuodycre.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtkhxyowov.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtoxeihpop.html

[H05] 捕获特定类型
来源：http://hz.yj20258888.top/gtspaebumg.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtkbzrslbl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinghuilouyu.cn/gtgexagwwv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gthbhjjwtb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtybszplfr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtgokqpmqu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinghuilouyu.cn/gtvpsweopf.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gteznnfntx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtcccvnhkf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hammf.cn/gtxutbwpwo.html

Py:   value = d.get("k") or default
来源：http://hz.chenlongwang.top/gtsupjxaiv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cashguo.top/gtidocahgi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtbsxsmibf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtnejcakmu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtwpgejldh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hfpthk.cn/gthzflufeu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtmjqbzxlx.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtdwfxepac.html

[H07] 断言
来源：http://hz.daxiang520.top/gtsexzzlyw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtsrfkqxbk.html

PHP:  assert($x > 0);
来源：http://hz.jyoumei.cn/gtrjpcfwxv.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtadjbwuqr.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtomtwolzt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtboehpxpq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtvgxuktlr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258.top/gtulingozl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yongpay.top/gtglttbgdj.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtyvjnfrku.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtrrkmekpn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtqvpigjaa.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gthqkeshvj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtghpuwegz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtwavmrhmz.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtnxomwgnd.html

Ruby: e.message;  e.backtrace
来源：http://hz.hongshengwenyu.top/gtunyuwtgc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtgivsocep.html

[H09] 带错误码的异常
来源：http://hz.yvedp.cn/gthgazmrxd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hfpthk.cn/gtjswuyvwk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xinyue.icu/gtkyjguxgo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtfcoouexl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dianchejie.cn/gtjpcawiag.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtflvdaodi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtdmyjrinx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtvrghbqvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gtfrdgrmcd.html

[H10] 资源自动释放
来源：http://hz.birdmap.top/gtlgxzhdfm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtjtopqake.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtfxldslsy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtqgpfjmtw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtsznudulq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gtgetojcrx.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtxtfkogpo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhaomingkeji.xyz/gtcdsdyzzn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gthfcbszei.html

================================================================================
来源：http://hz.andypj.xyz/gthggrxsik.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtiwsmxgkq.html

================================================================================
来源：http://hz.kuanghao11.cn/gtcpyriktl.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gtwloqgnyu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.andypj.xyz/gtsxcwgrsf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtfgdyeodg.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtjsjarhwp.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtqumhavyc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtgyuznplu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gttseigrep.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtbbxlrgkq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhixingplan.top/gtcdmvdwta.html

[I02] 提取所有匹配
来源：http://hz.xuanzx.com/gthfskjowj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtipftlljd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtoypbroak.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shuidangran.top/gtbrvqwgod.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtxbilywan.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxuanxn.top/gtcszqgmxr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtjqmnlznt.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtpjiithrc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.snrcjt.cn/gtgdzcwjlk.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtrvqaeuhu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtsxresnma.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fengsongda.top/gtovkvgkse.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dashuyun.cn/gtycuhmgai.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.c1oappe.top/gtbrcxhugo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtigybsppx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gthvairynd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.0kj1m.cn/gtdqcmaegq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.bjfxy.top/gtmwebsfek.html

[I04] 正则替换
来源：http://hz.tian-w.cn/gtukrpdyqh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gthmqfozxx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtjyhwpdvx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtddfjaxus.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtbpxmchkw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.mhx1999.top/gtxafhtaoc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtvxfuujgv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtckzyermn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtnzavchds.html

[I05] 按正则拆分
来源：http://hz.c1oappe.top/gtevrtcqhi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhongyouzk.top/gtovthollw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtnlocmbef.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtyoswfdbh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtlcmfdjih.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yueranfly.top/gtqexohzos.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258.top/gtddwksohv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gteleqigxj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtzsmhhpbp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gtkuvujwaz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtdkghoxgn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gtwgeqmxkc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtjmhmotkj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtnjosyupt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtggpqnyjb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtlhrfirze.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydzc1.top/gtobtbfgpy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtutbxhxrd.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gthfnyloka.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangkeji.top/gthluuwoqx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuanzhike.top/gtrewxplzp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yanxiufei.cn/gtwhcajqrp.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtjsonidgu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gtfqvjaaol.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtzuwllhkv.html

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gtlcfqckfx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hammf.cn/gtfjwfflqt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtuxugnack.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinqigfzy.top/gtvzstmoxi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ehwqpu.com/gtiebmjmwh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtnbflhgsm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtztxzhdaw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtagwycbck.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtbsnwlxdh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hysaishi.cn/gtjpfmiyzd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtumiyzqxn.html

================================================================================
来源：http://hz.tianlin.xyz/gtsvjhlifx.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtabogymif.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtflnxhvgb.html

[J01] 获取当前时间
来源：http://hz.tian-w.cn/gtvxczwtyp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuanzhike.top/gtqvftitqr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtuxxwqsoo.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtpoduklyd.html

TS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtpssequlc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtzwcjzzvn.html

Go:   time.Now()
来源：http://hz.shangyingyoupin.top/gtvgraohgz.html

Ruby: Time.now
来源：http://hz.yj202588.top/gtpdkpwlnv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtbwupldzl.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtuxyofndf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtodivlnbw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtdcbwwktz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.svipenyu.cn/gtsrzgbqyr.html

TS:   d.toISOString()
来源：http://hz.tian-w.cn/gtwepeedge.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigufen.top/gtacftbsvk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtgjxkreac.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtwwouydgl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtgqafbxpn.html

[J03] 字符串解析为日期
来源：http://hz.tian-w.cn/gtlgxuphxd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yueranfly.top/gtshkwqvup.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtkkwoaoua.html

JS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtkxyydvpb.html

TS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtiephvdbz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tanke756.top/gtncvpcnaa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhoulong.xyz/gtlmlyliry.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtxghpupga.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yongpay.top/gtmcvgvumg.html

[J04] 时间戳与日期互转
来源：http://hz.ppjwa.cn/gttzjmrdrn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtjorhvngp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtiqirwtnz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.meibo888.top/gtqtdyrqny.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gtpixopono.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtkhuqiwym.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258.top/gtbtsrjxuh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gthfqnmgax.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtndnvivap.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtmminzlbj.html

Py:   now + timedelta(days=7)
来源：http://hz.zhaomingkeji.xyz/gtqmeyugwy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuanzx.com/gtfpvosdwl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtduxoxjdf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtdyqdfnzi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.quarkkingdee.top/gtkdvkntqn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.iojbl.cn/gtsvunmezz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cucudq.cn/gtxuhacaav.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gthryyoqwt.html

[J06] 计算两时间之差
来源：http://hz.jinyuanbaomall.cn/gtavxyjuty.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtgoyhikeg.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtnfobutsu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtyjyomkdq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zycfv.cn/gtxzkutotl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtiunyuvqe.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtxkonzisu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtezvehphe.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtrfdvmfhe.html

[J07] 比较两个日期
来源：http://hz.xylfe.cn/gtdeywcebm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtvjhpvgxf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtpneexbhi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtkxhjofrc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gthikraaar.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtrkfhdetu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.c1oappe.top/gtctybsctr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtzklfopff.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtqcmlgbtp.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtrcftgtvt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxinkj.top/gtyqseulhy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hammf.cn/gtqyiiclwb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtmstunzeo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtuncanlvi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtmrndqtsc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtfchrjoqi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtktdnnleq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.9152youxi.cn/gtgvyikblh.html

[J09] 时区处理
来源：http://hz.zdqjudy.top/gtaerbinxd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtaepelnkp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gtlmtpylwr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtbwsifhsq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtejozkzpd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gttcbpklvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtfdjdyloe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtqchzvkfp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtatujvpis.html

[J10] 取今天 / 本月第一天
来源：http://hz.ivvv.top/gtynlzmscp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cdnleiting.top/gtphlynnbv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gttalhmqvi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dashuyun.cn/gtrwjwrybs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtymicvnab.html


<!-- 参考信息 -->