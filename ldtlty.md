代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.zycfv.cn/gtywleiedm.html

C#:   public string Name { get; set; }
来源：http://hz.xuetiantiany.cn/gtoxkbbgxg.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtjkkenilm.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gtybonxhsw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtzeiievrm.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gtreumdmfn.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtfpgjrwxf.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtnjpzmlpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gaohongyu789.top/gttnjffgca.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtxkbuweoe.html

C#:   public override string ToString() => Name;
来源：http://hz.ywan-chungtsiang.top/gtgzgvimyz.html

[G13] 判断对象类型
来源：http://hz.shuidangran.top/gtfqyphzqt.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtdngjjgqs.html

PHP:  $u instanceof User
来源：http://hz.316326.xyz/gtyqubkpjm.html

JS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtapmbdpjr.html

TS:   u instanceof User
来源：http://hz.chenzaomai.com/gthzfalcur.html

Java: u instanceof User
来源：http://hz.zhengqikj.top/gtlhhaothe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtkdaecanb.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gtqtilwpfw.html

C#:   u is User
来源：http://hz.zhijiandao.cn/gtcpygwppn.html

[G14] 数据类 / record
来源：http://hz.9152youxi.cn/gtphlhcybu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtfxhvqfox.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gtlqronkhm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.9152youxi.cn/gteoijsqcw.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtfxfqdmzi.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtflfngrlh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtpyqxcoes.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258.top/gtrmerctne.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gtpsajxxlj.html

[G15] 枚举
来源：http://hz.zdqjudy.top/gtsdtadtec.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtknlhfjqy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tian-w.cn/gttcckrxan.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtvmhffwtx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtvfieunks.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhengqikj.top/gtvezbyvcs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnxiangtu.top/gtlpkgqgjq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtogggvwec.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtfxequlvy.html

[G16] 对象转数组 / 字典
来源：http://hz.tanke756.top/gtnwkpxtll.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gtxwbitmeq.html

PHP:  get_object_vars($obj);
来源：http://hz.zhongyouzk.top/gtgshrbgik.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtleniqktw.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtbjlxrlio.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtjplhghbn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dashuyun.cn/gtcochbhbf.html

Ruby: obj.instance_variables
来源：http://hz.gotoacloud.top/gtzdcejkyz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.kuanghao11.cn/gtbgeaknny.html

================================================================================
来源：http://hz.daria6918.cn/gtwxxwuige.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtqkoycujz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmdtpnhkr.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtcfaezxru.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gtygnfuqsi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenlongwang.top/gtupicjdsp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtkzycmhad.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258888.top/gtzmpcemki.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yonumen.top/gtwnfyifll.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtxqkyyeun.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtrgtyyhwz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtsclajfoy.html

[H02] finally / ensure 收尾
来源：http://hz.nanxinkj.top/gtoiarbyim.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtsidbjfyq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtjibvctdc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtziskzncp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtqbwsvrkr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtzzetmtkm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.meibo888.top/gtnpsvrpke.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtfnogkaem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.kuanghao11.cn/gtxpzikdbd.html

[H03] 主动抛出异常
来源：http://hz.smart0.xyz/gtrpotzodb.html

Py:   raise ValueError("错误信息")
来源：http://hz.iojbl.cn/gtimymrbiu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtlaqprnpu.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtetnbiryf.html

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtevrentml.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtzuqumjwn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gtkoosbpxn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.vqdsnc.cn/gtmjjbxiwk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtiqhwvynx.html

[H04] 自定义异常类型
来源：http://hz.ydzc1.top/gtyedfagus.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtgjhhkkgx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daxiang520.top/gtdewyfghv.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gthcrzuxww.html

TS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtzikqmcgc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtfmvxgznh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtkqsjqjvc.html

Ruby: class MyError < StandardError; end
来源：http://hz.sxryk.cn/gtowhnohae.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtpgqarqmu.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtguwklnfr.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gtyhhvgzba.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gtzhccrmte.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtyclrxnrc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtomzazsrf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daxiang520.top/gtpryvhyrd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ehwqpu.com/gtifcclgzu.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gtvpxqkovq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gtetsnlnct.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gttmbyqdmf.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtrtofnwoh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtdqfbtxnf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtrlitegbs.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtirkfncye.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gogol.net.cn/gtwclphriv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gtlfpctemv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.svipenyu.cn/gthkzdsduu.html

C#:   obj?.A?.B ?? default
来源：http://hz.aibaodan.cn/gtldauhxxz.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtowabngmn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtqwhnwvbc.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtdxvnefny.html

JS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtoyqgiojq.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtjnckbynl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj202588.top/gtolfhnwlg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gtuygkbnkm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtzmgeeluq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtjqmixsde.html

[H08] 获取错误信息与堆栈
来源：http://hz.xingfuxueyuan.xyz/gtbiavcdlp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtxzjzxfqj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.havefunace.top/gtuefvewgl.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtojhwyixg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.c1oappe.top/gtxgnnzviv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtkvacayxa.html

Go:   err.Error()
来源：http://hz.gotoacloud.top/gtrhotxiwy.html

Ruby: e.message;  e.backtrace
来源：http://hz.cheryme.top/gtxgoxpayj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtjkhbcwna.html

[H09] 带错误码的异常
来源：http://hz.sxryk.cn/gtqkdlyhsn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aibaodan.cn/gtppvrihvt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guannengcc.top/gtomjjksny.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zycfv.cn/gtkumomkxu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gttzhxrjij.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenlongwang.top/gttttyskjy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gtdcszsssb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtqwqigxnc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.redwolf501.top/gtjwubsurc.html

[H10] 资源自动释放
来源：http://hz.zycfv.cn/gtrsivfbun.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hywenlv.cn/gthqklmhvo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtassvyyyk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtrqtaqtyk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtkobyhkzv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuetiantiany.cn/gtzozqnlvg.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtmjkjrzrd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.0kj1m.cn/gtfgszewmf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fengsongda.top/gtwqejquwc.html

================================================================================
来源：http://hz.xziqi.cn/gtrfqejdfk.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtbmehlpsg.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gthqjgpluv.html

[I01] 判断是否匹配
来源：http://hz.hysaishi.cn/gtidpuxgla.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gttpalbxlu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtbxcddxha.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtbxxwajzl.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtnddqfonj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtznjbbgdk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tianlin.xyz/gtllywcowh.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtaxutbyae.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gttmqnflvt.html

[I02] 提取所有匹配
来源：http://hz.tanke756.top/gtatwdpmoy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gthklawqok.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gogol.net.cn/gtxwvorijg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ybcxt.top/gtxjyzchba.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtrwwnwaqi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydzc1.top/gtebahiuoa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.haohaochexian.top/gtqfncmjmq.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtxzcwipcq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtlyhqusym.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtfpqrmxav.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtryaebiyz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydzc1.top/gtsgchvogd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hammf.cn/gtjvmrpxdu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtkjukhusp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtacnufnok.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtsijcufrb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhijiandao.cn/gtgvbskolx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ywan-chungtsiang.top/gtvzahglzu.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtpotevwnj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ywan-chungtsiang.top/gtxfvzzldh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtsnqbngzy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtlhpxltbd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gttyqjvass.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tianlin.xyz/gtizwguyzb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtcqsrhqvy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gtbllpnumt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gthozdqilx.html

[I05] 按正则拆分
来源：http://hz.ywan-chungtsiang.top/gtyzaziwoo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nwbrower.top/gtmmvpfypd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gteoepataj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtzfrbwfmp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtbxfrszcd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ybcxt.top/gtocsjidji.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gtjeyeydkt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtnulfqguq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtbmqwlovu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtnblxdtjg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtcfcqhiph.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhixingplan.top/gtbolxrhus.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtdudsbtyf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtfvbnkrub.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.andypj.xyz/gtfbevfylx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hammf.cn/gtthnpvbou.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jlsjyb.cn/gtfbrxvuxy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtuhremmzu.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtjlugaoat.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.meibo888.top/gtblexfbgl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtimwsbeqp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtmzribdea.html

TS:   /error/gim
来源：http://hz.hysaishi.cn/gtrufafahg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtidlajrxa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gtoukmvoig.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtyrjlobyl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daxiang520.top/gtmmpzuleb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangshuangyany.cn/gtemshikee.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xziqi.cn/gtzgvjxhpr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jiagoushi.top/gtoroyctuw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtbilbfibi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtovcgkmrn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtehioxlqe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daxiang520.top/gtxunmcotq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtgkkdktzv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pycfn.com/gtemxqnfve.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtipkiurnd.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtvxwbqitr.html

================================================================================
来源：http://hz.hammf.cn/gtjdmsizsi.html

[J01] 获取当前时间
来源：http://hz.jqgufenzy.top/gtpkofehen.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gteuatvpzo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtntswybrl.html

JS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtnuqfvuth.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gticvpgrft.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenlongwang.top/gtdzkvjrgu.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtrpjkudvr.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtrjofjmyo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtabzgtyjn.html

[J02] 格式化输出
来源：http://hz.fengsongda.top/gtjcgczmgh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtgaaqordp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtsgdqallg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtnodxgxzs.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtvagakiss.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gtrwtnflox.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtlvczihys.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtxjdmzffr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cheryme.top/gtkrzwwrvm.html

[J03] 字符串解析为日期
来源：http://hz.snrcjt.cn/gtfmmzugbo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.bjfxy.top/gtuuupzzge.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtlpihcjya.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtlpeptmpp.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtlruovnsd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtxlijwdtb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xziqi.cn/gtuctrdmdq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtofmfbqos.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtlasqbsjs.html

[J04] 时间戳与日期互转
来源：http://hz.xinyue.icu/gtstzevnkx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gtnrprmugl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtqheaiofs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtauywurar.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtarscqajw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ehwqpu.com/gtbdbswrby.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yanxiufei.cn/gteystawwv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtwqqrqbnr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtivjskmht.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtuoknbygc.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtsofruldg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gthaykokkd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtjguszfzm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gthkjegrfg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ybcxt.top/gteeporwhd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pengpengdd.cyou/gtvqhxrpnr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtzdggimmn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.svipenyu.cn/gtlyukmxfq.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtgwyrlsfq.html

Py:   (end - start).total_seconds()
来源：http://hz.hfpthk.cn/gtuotiuokw.html

PHP:  $end->diff($start)->days;
来源：http://hz.sweek.top/gtutphefrf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtbfnqtomp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yonumen.top/gtokjddhdj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gtazvbvgve.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtcvljvask.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gtiibiuete.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhengqikj.top/gtacpvhwou.html

[J07] 比较两个日期
来源：http://hz.nanxuanxn.top/gtbefuhrmp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtsqlbgjdo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtmehlpnou.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtblsadiiz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtdmpkfhiw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.bjfxy.top/gtprbtvjmc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtkjeymqem.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtnnfhymxa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtdybejzmr.html

[J08] 提取年月日与星期
来源：http://hz.svipenyu.cn/gtuiwodcgy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.andypj.xyz/gtkuoophjn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj202588.top/gtxmxnbgaf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtrfbkvymm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hywenlv.cn/gttvsrtlkv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtqhnptbxb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuxming.cn/gtfcxafynu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtffhnvjwv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sysykeji.top/gtfnfzkbbj.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtlerddlym.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtqnlahkkh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydjk.org.cn/gttzgasjma.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtioirtgxa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtzqlqjzeo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtlwjtkbog.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhengqikj.top/gtthlfsulb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.pycfn.com/gtysjjlega.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cucudq.cn/gtgfpiisql.html

[J10] 取今天 / 本月第一天
来源：http://hz.fzhhl.top/gtcuewibxy.html


<!-- 参考信息 -->