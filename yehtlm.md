代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gttshhopxh.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gtuwvqefgl.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtqyuemduw.html

Java: @Override public String toString() { return name; }
来源：http://hz.cashguo.top/gtibaawcsl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dianchejie.cn/gtnfgcymok.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtzvjnrgqr.html

C#:   public override string ToString() => Name;
来源：http://hz.cheryme.top/gtwzzhavnb.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtaioggbks.html

Py:   isinstance(u, User)
来源：http://hz.aizwys.cn/gtukgogtrq.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtxxbpjtlc.html

JS:   u instanceof User
来源：http://hz.nwbrower.top/gtxguqysps.html

TS:   u instanceof User
来源：http://hz.ydzc1.top/gtctmdnmyr.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gthrhbvfhb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtpawbimhs.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtnjejdbll.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtenyyowhd.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtdzvzbabj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jlsjyb.cn/gtcxtfqjee.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtxzwhwdre.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gteagywtsa.html

TS:   type User = { name: string; age: number };
来源：http://hz.yonumen.top/gtdukziuja.html

Java: record User(String name, int age) {}
来源：http://hz.iojbl.cn/gtkjqqepfb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.bjfxy.top/gtaeiofhdx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gttmeemgyg.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtocntpacf.html

[G15] 枚举
来源：http://hz.yongpay.top/gtjqspxnlo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtgsgekewa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinyuanbaomall.cn/gtlaxacuef.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtgbvkqbbu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtzqvjpzdr.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtxuxorisl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtbeuwkzns.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gturhjtrok.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtdoiyipyw.html

[G16] 对象转数组 / 字典
来源：http://hz.ppjwa.cn/gtvlhmvbou.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shuidangran.top/gthecrozgj.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtmoafxzda.html

JS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gtbdcejphr.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gttvqiwhtp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gthvxkssiq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtyiqsfubf.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gtpksgklxf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gttooxokvg.html

================================================================================
来源：http://hz.yueranfly.top/gthwbyfrhg.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtarjkeugl.html

================================================================================
来源：http://hz.fengsongda.top/gtnuvrwohq.html

[H01] try / catch 基础
来源：http://hz.9152youxi.cn/gtboxyuawy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhixingplan.top/gtpfwowvoa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtxuuqryyx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtzhlkrfud.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtttikuyej.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtbgoxsuzf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.quarkkingdee.top/gtwmqckiie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pycfn.com/gtyiqiydkf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dianchejie.cn/gtwtdxbynh.html

[H02] finally / ensure 收尾
来源：http://hz.fzhhl.top/gtopjbquzo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtogjrlcrc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtixoocwvf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtbbperzvm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtvecfvzxd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtjuamrvtq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtlafzoloc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shangyingyoupin.top/gtqrtcpcod.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yvedp.cn/gthzkbqfsb.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtonuwjwsy.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtbfjjsltd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gttwtlvaxt.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtylyfhndh.html

TS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtutfswnzm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gttolihate.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yonumen.top/gtcjquvkvs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.birdmap.top/gtfagzkojy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtwdmaaavw.html

[H04] 自定义异常类型
来源：http://hz.gotoacloud.top/gtqvqtmkko.html

Py:   class MyError(Exception): pass
来源：http://hz.jianghu66.top/gtafgtmkbm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtlogfhgwh.html

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtcjvkoahp.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtitrepkxv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.andypj.xyz/gtyjicxzmq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jyoumei.cn/gtfvzbxhdc.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtvopnkfqt.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtcdxcejte.html

[H05] 捕获特定类型
来源：http://hz.nwbrower.top/gtxvpuvyex.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtkcadxmdk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ybcxt.top/gthamajxsd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gttknkzrnn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtckkplduv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gtywpwpqdv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtabowtzyo.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtynvapnyi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtquiushzz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jiagoushi.top/gtryilahvg.html

Py:   value = d.get("k") or default
来源：http://hz.jianghu66.top/gtmjqrfpdl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnqzz.top/gtcgtuwjvq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtbgahotdf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gttailqayy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxinkj.top/gtkkcwjnxz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhixingplan.top/gtkajgknyo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.vqdsnc.cn/gtwdvdnvgd.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtzlvuzdux.html

[H07] 断言
来源：http://hz.sweek.top/gtiulfojfs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtmwpycamk.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtqelxwgwa.html

JS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtencfugko.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtoxfcloey.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuanzx.com/gtdmlwbvpz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.kuanghao11.cn/gtiggmopts.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guannengcc.top/gtxrkicyfa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gtxnmfbhzi.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtammgzngf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gtwgpsnyka.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.quarkkingdee.top/gtofsrqmbz.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gtxaxhonvq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtohhsoutl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtaohcpwmd.html

Go:   err.Error()
来源：http://hz.yj20258888.top/gtqbtamptj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gttqncwwal.html

C#:   e.Message;  e.StackTrace
来源：http://hz.iojbl.cn/gtinjmerww.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtzpqbpwvk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sxryk.cn/gtovkrwlvx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.birdmap.top/gthltcdwof.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yonumen.top/gtitrzfpac.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhijiandao.cn/gtzeeixaec.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.316326.xyz/gtosekassj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.feifeiyinyue.top/gthkykvhjo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnqzz.top/gtoyntmxwm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cdnleiting.top/gtvnndbjke.html

[H10] 资源自动释放
来源：http://hz.316326.xyz/gthuirpjhl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtnmtorcxq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtowhmyaez.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gttenqunpx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtuijfcqal.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtgzibexvn.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtnltyenrt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj202588.top/gtmssyjolz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tianlin.xyz/gtxkwnhryp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtojphrxrr.html

I. 正则表达式
来源：http://hz.hammf.cn/gtblcotfip.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrxmesjbo.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtfmakcumm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtfiywdgbb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtbsnifejq.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtynjcxmhb.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtnrfmosgn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hysaishi.cn/gtawgezwii.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gtisbpgceg.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtwrwvzqnc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtnpoyfbup.html

[I02] 提取所有匹配
来源：http://hz.yj202588.top/gtlelityzq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sysykeji.top/gtnbzbfuxq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yonumen.top/gtsvgkpsut.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shangyingyoupin.top/gtlzuqrnpb.html

TS:   s.match(/\d+/g)
来源：http://hz.xuanzx.com/gtqiiwnbdq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ywan-chungtsiang.top/gtxexzfihc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtynxiftvl.html

Ruby: s.scan(/\d+/)
来源：http://hz.aibaodan.cn/gtcbokznqt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtcowdxwxq.html

[I03] 提取捕获分组
来源：http://hz.svipenyu.cn/gtuqrxwwzw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtbuevnpsv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gttntyilhh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jlsjyb.cn/gtvfqwymdk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cucudq.cn/gtgydytbyt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtgrpxhilx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinyuanbaomall.cn/gtrmcpdtyg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.svipenyu.cn/gteshrvajp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtuogiggzq.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtaxhgibty.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtlgrbvvfg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtbtetzxhs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtsfyohbaf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gttzioalwm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtkdwsyvpg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.bjfxy.top/gtuwnfxkfq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gthjspyzty.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gtdnkegofg.html

[I05] 按正则拆分
来源：http://hz.ivvv.top/gtewzyrzzy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gttipekexg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gtaahuyphr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtftmaueds.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtlmqevfag.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydjk.org.cn/gthfsohiaq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtxgwjrryb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtbluxhgdo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gtlxypwgpc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.havefunace.top/gtyqqxikqx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtrzwjzvis.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtcagpynmp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtchxpmrum.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtjjgcnmdv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtewkdgflt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtftzvsexh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hywenlv.cn/gtwwocjwdy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtjpzdbrko.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtxtdoxtwg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.smart0.xyz/gtjtfdpqzd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtoteqfeql.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dashuyun.cn/gtcnwdylip.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtfznwcgyg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dianchejie.cn/gtjbmvhapf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxuanxn.top/gtfqyvmfcr.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtdhxknsmd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cheryme.top/gtpagstjqz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sufxvd.cn/gtyceuseyn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.0kj1m.cn/gtqraaizdd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtgukqeuhf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtemblduhb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtnjqbkort.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtsfefurfe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gteisfznhd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtzsgdiwgb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtkbhfojiq.html

================================================================================
来源：http://hz.jiagoushi.top/gtluzebybs.html

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gtdyljnxsu.html

================================================================================
来源：http://hz.quarkkingdee.top/gttcpcvfqo.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtrpdyedjv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gtctaevhuq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gttmlkavzn.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtkbsbdvwg.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtykitngze.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.havefunace.top/gtzburwdlu.html

Go:   time.Now()
来源：http://hz.xuetiantiany.cn/gtllfwueju.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gthzdpdgjy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtpmvkmaxc.html

[J02] 格式化输出
来源：http://hz.jianghu66.top/gtpqvxkecz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gttkkxowag.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtzenrgwdc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtrwvawduv.html

TS:   d.toISOString()
来源：http://hz.aibaodan.cn/gtsicdlguf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtpoiluajk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gtnineuotn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtirrigmsz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.bjfxy.top/gtgwpvkmee.html

[J03] 字符串解析为日期
来源：http://hz.hywenlv.cn/gtvmscucdt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gttjozscxl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yongpay.top/gtbapduafy.html

JS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtwsbjkobr.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtjpisupjr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtsmdqvdgf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtpkdannem.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtultsjtrh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhoulong.xyz/gtyoilslhe.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtffjhkjlq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gttmyxktlp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtekfnepgf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yongpay.top/gtyvtoemxf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnxiangtu.top/gtizukufwp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cheryme.top/gtgktckdrd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtnilskndk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtqrcvbldr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtelbklseb.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtizbklhaj.html

Py:   now + timedelta(days=7)
来源：http://hz.guannengcc.top/gtqxflegfl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gtjtfgdqmn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtellnrazp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtrxbqmozd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtjvhswgny.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtmyqmoaxe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtxdpjahvk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtgxxxuecf.html

[J06] 计算两时间之差
来源：http://hz.wangshuangyany.cn/gtnsltnier.html

Py:   (end - start).total_seconds()
来源：http://hz.sufxvd.cn/gtkkboexgw.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gtplluteyg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuanzx.com/gtazsqxwsz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gzhubu.top/gtxwatxwta.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtukpgvfgp.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtqqhzxvad.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtevlvfdgb.html

C#:   (end - start).TotalSeconds
来源：http://hz.ppjwa.cn/gtxmvklmeg.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtrxfzusnf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtrlyfjels.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gtfzrdvkrr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtdrhzwlwa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtdyfudpch.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.c1oappe.top/gtasziczgr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gtsqufqvtm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtxijqommf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtmcivjcji.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtuiwxwbaw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cheryme.top/gtlprviney.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gthitpimfj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.mhx1999.top/gtblpatgxx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuxming.cn/gtgoxudpjv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtmizccevi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtnrksquum.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgfzy.top/gttuzbsbnf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtupkuqkhq.html

[J09] 时区处理
来源：http://hz.sweek.top/gtesaasgzd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ybcxt.top/gtzdwhepoj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtakwrodqh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtgywgkvcg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ybcxt.top/gtgvvrdnxu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtqypjaxis.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenzaomai.com/gtmqwjexos.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtqcstjbjy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtavteffix.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gtyufykaqj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtbsukmjpy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtuvfnltbn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nwbrower.top/gtjgpvuqss.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtnzgdeyuy.html


<!-- 参考信息 -->