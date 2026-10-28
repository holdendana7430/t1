代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.jinyuanbaomall.cn/gtioqyftms.html

C#:   public string Name { get; set; }
来源：http://hz.xuetiantiany.cn/gtceipelen.html

[G12] 对象转字符串
来源：http://hz.chenjidiqi.icu/gtmuaoyyil.html

Py:   def __str__(self): return self.name
来源：http://hz.hnxiangtu.top/gthtleudzd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtsulxhjep.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtznjryihi.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtdghhmowr.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtxuaucgif.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gttvvepoac.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gthgdkddov.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtodduxrfa.html

[G13] 判断对象类型
来源：http://hz.jinghuilouyu.cn/gtvyoerqrw.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtjqjqzuyh.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtmfjyktaa.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtnmcpzalh.html

TS:   u instanceof User
来源：http://hz.redwolf501.top/gtyootmpbu.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtofwpvjjq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtdivbmlks.html

Ruby: u.is_a?(User)
来源：http://hz.svipenyu.cn/gtbfsmuyxo.html

C#:   u is User
来源：http://hz.hongshengwenyu.top/gtcuwoypyc.html

[G14] 数据类 / record
来源：http://hz.dianchejie.cn/gtbptcmuqw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yonumen.top/gtfmxfzooz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shuidangran.top/gtifnjvebg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtbqimxvwp.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtysylwgut.html

Java: record User(String name, int age) {}
来源：http://hz.xylfe.cn/gtuuldchnu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.52xcode.cn/gtxeogunnw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtiktxwygy.html

C#:   record User(string Name, int Age);
来源：http://hz.ybcxt.top/gtecfjnjnc.html

[G15] 枚举
来源：http://hz.ywan-chungtsiang.top/gtewvrnxyp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtplwcaswb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtkmckrfjs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtvjefhvzm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtpalwpics.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtzgupuwfr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gthizysjtb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhiwuduotai.top/gtljljmmkx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtesntchay.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtnwlricci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hywenlv.cn/gthfxvwgoe.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtsmgbqpph.html

JS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtnwofgvcg.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtbkodmbnh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangdashe.top/gtyyhysiux.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.mhx1999.top/gtndnxbrmz.html

Ruby: obj.instance_variables
来源：http://hz.jqgufenzy.top/gtbxqvurke.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daria6918.cn/gtiuatutdy.html

================================================================================
来源：http://hz.meibo888.top/gtqzcvdawj.html

H. 异常与错误处理
来源：http://hz.yuanzhike.top/gtsxmrgsgz.html

================================================================================
来源：http://hz.yj202588.top/gthydbraiw.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gtpnhoeoyg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gttldfucjh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gttdqjojmj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtzktyypoq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.9152youxi.cn/gtbwkyeeym.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtexspqljr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtdlxoookt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daxiang520.top/gtnjawpldz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinghuilouyu.cn/gtnwkacfrj.html

[H02] finally / ensure 收尾
来源：http://hz.hammf.cn/gtcfxjmzjl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.316326.xyz/gtqczpfvvw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtttawuxcs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtpkvcxiqf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtkaclnwxe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtiuhioeiw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtidkydrwn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtbsaxvolu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtacggbxsi.html

[H03] 主动抛出异常
来源：http://hz.mhx1999.top/gtxitwsqik.html

Py:   raise ValueError("错误信息")
来源：http://hz.hongshengwenyu.top/gtqmgtuzfp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtrkrylgab.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtfmvngdmc.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtxadbkwmk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtlfvzmbzu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gtjakmufkc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtmophwoqb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtxaatmwco.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gtjhqrmzys.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gtmqmcowos.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ybcxt.top/gtropwmics.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtpekowwio.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtcxztoiqa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gtlductitm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtsuhhioon.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtyeltjfzn.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigfzy.top/gtkwzmnwtq.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtkgbomffz.html

Py:   except ValueError as e:
来源：http://hz.yongpay.top/gtpwlvjjxy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gtkbbsxftg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gthtasrllr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtrtnzxium.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtlkgorbwk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gtpqrpkzgt.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtxviuhziz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhaomingkeji.xyz/gtkwsvqkvo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.bjfxy.top/gtlfjsrosm.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtzwvqzqkn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtsvwqjrsi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtzdbbclbm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtilillqus.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtuwpxvxrd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pengpengdd.cyou/gtgvsjxwsr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jiagoushi.top/gtaoenntej.html

C#:   obj?.A?.B ?? default
来源：http://hz.dashuyun.cn/gtyzqikjfq.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtbyvahkmc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtzdvcoohx.html

PHP:  assert($x > 0);
来源：http://hz.gzhubu.top/gtychrkhed.html

JS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtxhbumhmb.html

TS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtjbnvelax.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtrnfzvxrx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tanke756.top/gtcfuqnetr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtsntgdnee.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zdqjudy.top/gtdhdewzeq.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtfzcacjit.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.redwolf501.top/gtcmvfvlkd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gthbecclfh.html

JS:   e.message;  e.stack
来源：http://hz.hfpthk.cn/gtynbdjmko.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtqcnoswsa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ydzc1.top/gtafcmkmic.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtrwntrxaz.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtrngkpalm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fzhhl.top/gtaozpyqnc.html

[H09] 带错误码的异常
来源：http://hz.sufxvd.cn/gtggdeegaa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgfzy.top/gtrblbggun.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuanzx.com/gtsywjwfha.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtzgomahzj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenzaomai.com/gtbzryfgos.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shangyingyoupin.top/gtmimclrbj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gttzeyfdxa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jyoumei.cn/gtbdkmvhkg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gthetyqlmd.html

[H10] 资源自动释放
来源：http://hz.vqdsnc.cn/gtjmrahdyy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cashguo.top/gtjhylighl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gtexmtvicb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtktaerntg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtjwcxeuke.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangkeji.top/gtkresqcnd.html

Go:   defer f.Close()
来源：http://hz.jinqigfzy.top/gtvtdhpxsw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gtjrhtuksk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.9152youxi.cn/gthnjrpspc.html

================================================================================
来源：http://hz.hfpthk.cn/gtvzplxrmd.html

I. 正则表达式
来源：http://hz.shangyingyoupin.top/gtqevgczqt.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrsionyrh.html

[I01] 判断是否匹配
来源：http://hz.guowangkeji.top/gtwjkhkbju.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtvmxkjyvm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtihldzqrr.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtfvtxqleo.html

TS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtdirtscyx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtwergaqns.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtmgyvppsf.html

Ruby: s.match?(/\d+/)
来源：http://hz.cqqwz.cn/gtzhgdlbaj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtzwpzqxof.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtkfvxdwmz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtmyurficu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guowangkeji.top/gtwhzsuhld.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtgtthxpzh.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtzkmafnvw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtomwarvus.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.smart0.xyz/gtpaecawkg.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtckpuplyp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtzwhddmlx.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtzsdzxdrh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtlseliphg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dianchejie.cn/gthbmeshvd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shangyingyoupin.top/gtczczqgex.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj202588.top/gtmvpeuown.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtkbsvmdke.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gtpksryqlj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtawfhavgb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gthsogbskm.html

[I04] 正则替换
来源：http://hz.daxiang520.top/gtsdkzgtrm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gttjtqlyub.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtobvujnwa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtfgldmyil.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtchfctqhg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtmdghqiny.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangkeji.top/gtaljkdymz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtwbuojduz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gtbyaoifwb.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtghmrtxhr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtsgbomzyx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtsvmgvgtd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtxgsvlomm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtibxfvlch.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ehwqpu.com/gtwjmnovjd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj202588.top/gtmbswyczp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtyudhzrlp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gthafkszqe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.316326.xyz/gtoaryhewx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gthwsozajc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sysykeji.top/gthskxozbv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtcbinnsys.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gttqqdvvud.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtkiityomk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtbfxrebaq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenjidiqi.icu/gtyrgcwhxi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gttrfgyisk.html

[I07] 忽略大小写与多行模式
来源：http://hz.cucudq.cn/gtqisorcso.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zdqjudy.top/gtfmrqlcbp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtfsgvtpyo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuetiantiany.cn/gtwmupinny.html

TS:   /error/gim
来源：http://hz.mhx1999.top/gtehnnzqec.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.bjfxy.top/gtecplkywm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gtersoegha.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gttcoqkhys.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtxnpyuvie.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtzgxgcjis.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtvcylzrzs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yueranfly.top/gtuakdaftz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtwmlypxsv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtmdtxztun.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gzhubu.top/gtsfusyxcb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtbhmvlhrf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnxiangtu.top/gtxjqzzcaj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtoevjxhxq.html

================================================================================
来源：http://hz.smart0.xyz/gtxwsazkax.html

J. 日期与时间
来源：http://hz.zhixingplan.top/gtsdbpiehm.html

================================================================================
来源：http://hz.yonumen.top/gtregfjhyg.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gtqjfnmbwb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tian-w.cn/gtfcxdyppy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtotfvfxkk.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtykypmulf.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtudhbkxfe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhiwuduotai.top/gtwiztiqjy.html

Go:   time.Now()
来源：http://hz.jlsjyb.cn/gtkvbbwcbx.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gtpsahlclw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtwqazdism.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtlpcnxetv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtbimmfdsq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtrcsquspn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dashuyun.cn/gtfwxtvmpk.html

TS:   d.toISOString()
来源：http://hz.quarkkingdee.top/gtgsrudxjw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtrrzazisb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtpxktbrkl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtokeepqgs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxinkj.top/gteptpofyd.html

[J03] 字符串解析为日期
来源：http://hz.dianchejie.cn/gtedqxqfiw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtjpssnaze.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.andypj.xyz/gtddsooeez.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtqckhhxev.html

TS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtpyxsesax.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtjbjhucxi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtnsdsymfq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtmboeayrg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtamvxbzmm.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtxulijave.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtcyldchho.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.9152youxi.cn/gtxwyqbgwq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtphrmkkbm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtydegmzqy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtfvqubdsr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guowangkeji.top/gtsgekmczw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtjytwifuy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtnxuzfsxg.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtkseezquf.html

Py:   now + timedelta(days=7)
来源：http://hz.hfpthk.cn/gtxmiypiwm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gtaptseccl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtzdahzayl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gttaqpgajk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.9152youxi.cn/gtjgtlfkih.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jlsjyb.cn/gtwpjbyqwb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtoazbinlh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigufen.top/gtzgllpyhk.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gthxpiczmz.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigufen.top/gtfgnurywq.html

PHP:  $end->diff($start)->days;
来源：http://hz.ywan-chungtsiang.top/gtxayimigg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtvoycoill.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtpudfklhm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yongpay.top/gtxdfpigps.html

Go:   end.Sub(start).Hours()
来源：http://hz.ivvv.top/gtcylofpmx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj202588.top/gtgrqufodj.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtfkoyuwrb.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtftlhelmo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtcaxrnnyi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zdqjudy.top/gtytnyrlrh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtaealseyl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtalzhxunn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtgpekhdoy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ywan-chungtsiang.top/gtkyzfruov.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtlcoyjyhp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtlblyngni.html

[J08] 提取年月日与星期
来源：http://hz.jinqigufen.top/gtlqjmokqt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydzc1.top/gtqgorywzz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtkcjedoly.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtqwjnktww.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtgmelqvwa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tianlin.xyz/gtjghdpmth.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtyughgctk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtwgfpvdnb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shangyingyoupin.top/gtgxabiyqm.html

[J09] 时区处理
来源：http://hz.ppjwa.cn/gtylhzcksj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtdjxfubph.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtvvjxiyku.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtmooaotie.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtjviuhkka.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtziagowew.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtnqoepkej.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gtolbeeenq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtsuzhyvsg.html

[J10] 取今天 / 本月第一天
来源：http://hz.shzxlz.cn/gtbphzclrd.html


<!-- 参考信息 -->