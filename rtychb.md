代发 wailian999

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtovchyopv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtxmwdbqpi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jlsjyb.cn/gtgixgygmx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gtuxbmhwyo.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtaxthynxp.html

Java: record User(String name, int age) {}
来源：http://hz.jinyuanbaomall.cn/gtbncglurr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtlkslioko.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtsrivwcre.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtqpckpjbg.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gtuafrjtys.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gogol.net.cn/gtfragdlvp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hfpthk.cn/gtrskvriao.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtlrbgypjf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtzijmhcxo.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gttwsamihp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gterktxpbn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gtqeogcakm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gtjezcogof.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtporudddq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtmwaoeddu.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtwqeydanl.html

JS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gtxxcqvaga.html

TS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gthqwsnfre.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtysjjqxwi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtyepnrdic.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangkeji.top/gtakanvpcd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gtzzyqojje.html

================================================================================
来源：http://hz.sysykeji.top/gtmuhkqoqd.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtipqcbtrz.html

================================================================================
来源：http://hz.aizwys.cn/gtzjmxqiba.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gtzmrswcqc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtjjvlsnnc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yvedp.cn/gtcmsttnmt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtnritfqnx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtzfkzhdfd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtnsjfmnhh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtpxuydkhz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydjk.org.cn/gtzggigoly.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtszuhfzcl.html

[H02] finally / ensure 收尾
来源：http://hz.hnqzz.top/gtlkvdphmc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtlhgdyukh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtiokjsbrj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtfnvftyqd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtzquugxwu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtwfakvyml.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gthpnwavyv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtitnprfpz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgufenzy.top/gttdfjfwzg.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gtkwnscheq.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuanzx.com/gtfzkucfpi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtusskbapr.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtgxvmbzsg.html

TS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtorqpfqko.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtalbpfjig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nwbrower.top/gtuacgbezh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gtspjfhaog.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtzglllzsd.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtzpipvbbs.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtimkxfjzs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258888.top/gtjgzmahke.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtxghoocrg.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtslungkif.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gtuxqmgnko.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj202588.top/gtvfkfunls.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtwzdaobzg.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtflrtcrye.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtwyojyzfi.html

Py:   except ValueError as e:
来源：http://hz.zycfv.cn/gtkofblwoe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.quarkkingdee.top/gtcduwfvou.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtexjukion.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtgcpvjnsg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigufen.top/gtbpxpzlhc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtbpbkcxrh.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtksyvxmbm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtjydytwmv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gtuvyjuqwd.html

Py:   value = d.get("k") or default
来源：http://hz.sufxvd.cn/gtmcbmtaeu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtmauhisrj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gthgsxsdbg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtipkfloni.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.iojbl.cn/gtjibrfbke.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hfpthk.cn/gtpuanwzqi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtfpmrafbl.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtxkgdsijh.html

[H07] 断言
来源：http://hz.aizwys.cn/gtbthzcxnm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cqqwz.cn/gtvdgmxpuv.html

PHP:  assert($x > 0);
来源：http://hz.zhengqikj.top/gtpgkzvkrh.html

JS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtjxsxpvvh.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtsjsfvzwa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.birdmap.top/gtmiffxwsx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xingfuxueyuan.xyz/gtfddwmnee.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenzaomai.com/gtgrxylfft.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtjazuoyks.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gttktklprh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.vqdsnc.cn/gtkbaollgj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinghuilouyu.cn/gtuabajrsp.html

JS:   e.message;  e.stack
来源：http://hz.ydjk.org.cn/gtlsttswlk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ivvv.top/gtezoxvfdf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gtiqpjznbn.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtlfahzymo.html

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gtuywzsnui.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtcoianyzr.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtgakjifso.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gthuqudjwz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtafhdnjdp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hysaishi.cn/gtjsyxmyjj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jlsjyb.cn/gtiyvquyxf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.316326.xyz/gtqvkefllx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtxdxhddvb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jyoumei.cn/gtmiquwbgs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtftcvescz.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtyxxheyvb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.bjfxy.top/gtpedqchpe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.mhx1999.top/gtmaamdyis.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtdhwuvwcp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtimscxgte.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhijiandao.cn/gteksvcpca.html

Go:   defer f.Close()
来源：http://hz.dianchejie.cn/gtxflbxnxl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guannengcc.top/gtgifmoxjt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtfnxecbhy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtajtcptkj.html

I. 正则表达式
来源：http://hz.hammf.cn/gtthpshhoi.html

================================================================================
来源：http://hz.fzhhl.top/gttvrdanrl.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtveveifej.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yonumen.top/gtuoprlfdm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtyooxjnjd.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtqpbezxuf.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtjfrdhvoj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhiwuduotai.top/gtiholdumg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj202588.top/gtjitlanvl.html

Ruby: s.match?(/\d+/)
来源：http://hz.ppjwa.cn/gtowuojnhr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tian-w.cn/gttfvycvju.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gtgztjqgnz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtrradgzhb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxinkj.top/gtvkbzcytz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnxiangtu.top/gtlunvkejw.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtspqxreku.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtvcshewag.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgufenzy.top/gtvalxgkxm.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtbxwpoarf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtlsluwvkd.html

[I03] 提取捕获分组
来源：http://hz.nanxinkj.top/gthwwfvypc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yongpay.top/gtyxnyaxxy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtninpsmsq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenzaomai.com/gtmtwvprmo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cdnleiting.top/gtbrkkotms.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guannengcc.top/gtcotgppry.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtocobqpyt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.bjfxy.top/gttiknpekq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.havefunace.top/gttaphyjtq.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtwzoayllx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtxznsnfuj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtxgyghvdv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtoralbgfq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtojtwjbus.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.havefunace.top/gtasrdzvtd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xingfuxueyuan.xyz/gtcbdbdmyw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtocqwxugu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cheryme.top/gtevrmvfff.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtczhpjuuw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydzc1.top/gtrosficeo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ppjwa.cn/gtlbzftbri.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtusdiegix.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gteozbtckn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnqzz.top/gtgbvdkenb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtxtzwnosf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtbxghqmym.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cheryme.top/gtvljbrudv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gtdkfoygre.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtfakshrej.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgufenzy.top/gtubatnysm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtqyrjsjwd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtplxkqsln.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtvrtpdqao.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtxocxkcbt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yongpay.top/gtaybusrja.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtgtlhabwi.html

[I07] 忽略大小写与多行模式
来源：http://hz.yonumen.top/gtlaeanjqi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258.top/gtizfdsahe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sufxvd.cn/gtmekqtubw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gttutacofk.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtecgrjjux.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tian-w.cn/gtovyobtwa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtcxpvklbi.html

Ruby: s.scan(/error/i)
来源：http://hz.gogol.net.cn/gtinqrldfy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtfoysuljv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cucudq.cn/gthjtubaln.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xingfuxueyuan.xyz/gtdyrttxtr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ehwqpu.com/gtpjmgxdzs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtpjibnowm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtdargniek.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.52xcode.cn/gtngjfgmgr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtotkvtikz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtflzrvpxw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258.top/gtsevflvid.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxmuplwyt.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtcefealut.html

================================================================================
来源：http://hz.gogol.net.cn/gtubmwhtrc.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtuxzbktba.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtoivmqqfs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtbfcjpulz.html

JS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtqxpfrvdk.html

TS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtpthanjas.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sysykeji.top/gtlnntmaes.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtkurailgb.html

Ruby: Time.now
来源：http://hz.yj20258888.top/gtazlgqafy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pycfn.com/gtmosnjfmz.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtjjhfwbwj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtgmicblvm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtoesonxpx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtlbogfwwm.html

TS:   d.toISOString()
来源：http://hz.aizwys.cn/gtroyusquq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pycfn.com/gtksypolzz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtvoyjetoc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtdpewzbih.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtifblmjpw.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gtdksatuaq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sysykeji.top/gtexagedub.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yanxiufei.cn/gtpkljlscn.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtbbudpfvb.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtpyivbjqn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtbqrwdevn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daria6918.cn/gtrianclvs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtlfgfzgmy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.316326.xyz/gtgxxytlep.html

[J04] 时间戳与日期互转
来源：http://hz.sxryk.cn/gtcbhoxxsf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtijmxsohi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gttzgidfgc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtafaztfib.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258888.top/gtvalipktp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxinkj.top/gtlpnqwceo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtdwlvxrin.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.mhx1999.top/gtpwhgjxrw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.haohaochexian.top/gtjlvfwgyz.html

[J05] 时间加减（加 7 天）
来源：http://hz.hammf.cn/gtiropofoa.html

Py:   now + timedelta(days=7)
来源：http://hz.yvedp.cn/gtxlvalwav.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gttpysnfwu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtambyafbx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtoyzbwgml.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gaohongyu789.top/gtoxvdcftb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtvuwuwfom.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yvedp.cn/gtuoznncqn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtkylenref.html

[J06] 计算两时间之差
来源：http://hz.tanke756.top/gtxfhdlptn.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtjgqvihao.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuanzhike.top/gtyqdwjgnu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gtmehmdzsi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinghuilouyu.cn/gtalnflmbk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hysaishi.cn/gtsbiayqwx.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtgpqafbkg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tanke756.top/gtsdbpoqsw.html

C#:   (end - start).TotalSeconds
来源：http://hz.bjfxy.top/gtzziuukyw.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtkrlxltjx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtvnpzhzvm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtptofwnni.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtzuxqddxg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtftmsxono.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.svipenyu.cn/gtoedxlujm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.mhx1999.top/gtusedahhh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtypjdotqj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtlajelyhl.html

[J08] 提取年月日与星期
来源：http://hz.chenzaomai.com/gtmpqmgzak.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cashguo.top/gttcvxwede.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtplrsnsss.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtxvnfdcwa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtwlynhqox.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtkudoshlx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtvdiecciz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtwhksuogc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtdenkmslf.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtvcoygwlj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtndnjqpil.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtqqragbjn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtjyvjmsyl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtohlvruax.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pengpengdd.cyou/gtoppyuqfy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenlongwang.top/gtlexafbpk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtxchlahnh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgfzy.top/gtnkwpwxcu.html

[J10] 取今天 / 本月第一天
来源：http://hz.guowangkeji.top/gtccuhchgz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtpcfwghqn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.haohaochexian.top/gtndhvqwxo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtkxcoovtx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.haohaochexian.top/gtgphkucsn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtqllvjohc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.kuanghao11.cn/gtyeiorytg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cucudq.cn/gtevzkmagb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ivvv.top/gtlwbwbrru.html

================================================================================
来源：http://hz.xinyue.icu/gtbbqstmia.html

K. JSON 与序列化
来源：http://hz.fengsongda.top/gtxmjofgeu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxzyttwip.html

[K01] 对象转 JSON 字符串
来源：http://hz.9152youxi.cn/gtpyqmgtkz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtievrzrom.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtmmiaapno.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gttsjdbndn.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtjquueouj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtcrarnbdo.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtcexzdepa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pengpengdd.cyou/gtmgqjcwvv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.meibo888.top/gtymlrrbtt.html


<!-- 参考信息 -->