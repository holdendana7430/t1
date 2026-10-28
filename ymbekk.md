代发 wailian999

Java: u instanceof User
来源：http://hz.shangyingyoupin.top/gtkairyisg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtkmlalglw.html

Ruby: u.is_a?(User)
来源：http://hz.guannengcc.top/gtxccilskz.html

C#:   u is User
来源：http://hz.shanyushiyangtech.top/gttqnlpqff.html

[G14] 数据类 / record
来源：http://hz.jqgufenzy.top/gthecywqgg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtagjresza.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gttioemzpp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtmpdravhy.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtdqfxfmly.html

Java: record User(String name, int age) {}
来源：http://hz.aibaodan.cn/gtptnnwubs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtfbbhkqzc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gthfkksdjb.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgufenzy.top/gtfewttjet.html

[G15] 枚举
来源：http://hz.yuxming.cn/gtucwfmgjb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.smart0.xyz/gtqiygpmdi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtafhvhozp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xylfe.cn/gtwubbrunh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtkmwvhiqd.html

Java: enum Color { RED, GREEN }
来源：http://hz.daxiang520.top/gtgqctrhkc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtlkpqalls.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtkmopkkuq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtddxojxoa.html

[G16] 对象转数组 / 字典
来源：http://hz.pycfn.com/gtygexjemd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtsdikdnqm.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtlruuseqt.html

JS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gtxbzikfns.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtwruxzfip.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gotoacloud.top/gtzuefwwbv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtfcyxjabo.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtwbqhqxnv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtbgngrhvo.html

================================================================================
来源：http://hz.ivvv.top/gtvkgirkbo.html

H. 异常与错误处理
来源：http://hz.birdmap.top/gtnjapfgge.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtejzfutfq.html

[H01] try / catch 基础
来源：http://hz.dianchejie.cn/gtvpudpudk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gttbwwiapb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cucudq.cn/gtzkpqvdhd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtvllndnkg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtrbvwdxqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtkrxtqrua.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtrjhztxvq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aibaodan.cn/gtsdsfsasn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtouoczabj.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gtvylpsmvh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtmnmsjiss.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtllozfgop.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtneldxhji.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtasbvsnlm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtwucjtkyq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuanzx.com/gttieqwpbw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gtploxphfk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daxiang520.top/gtvfqjqage.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gtfmzxixem.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtnacaxebo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtzdlarzzg.html

JS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtbuhzjhcl.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtvioazvoz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtlyqjnlti.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigufen.top/gtdnebnimn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigufen.top/gtnejorige.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gtzfctqimg.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gtueiparhr.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gtieuflipg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtccegqcbj.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtxmoaxsnc.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtpuolzkpz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtqeepvddq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtgwnysmkb.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gtkujsrojw.html

C#:   class MyException : Exception {}
来源：http://hz.ywan-chungtsiang.top/gtdcxfofrm.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtkwnzzacu.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtoitdoego.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtafygbdhr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtitgfmnto.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtmexhvvfp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtbfulzfvb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtkzjoffos.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtytzrdzca.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zycfv.cn/gtkotxjxua.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtozsgyosj.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gtbaijxhri.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gthjafjbkv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtctbicwed.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtlbbgvoyh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtwnfmehwt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtmfkojvez.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zycfv.cn/gtaofurulc.html

C#:   obj?.A?.B ?? default
来源：http://hz.hongshengwenyu.top/gtuzwqthpq.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtmlcojmmu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gthaehifpt.html

PHP:  assert($x > 0);
来源：http://hz.316326.xyz/gtfvnluxmt.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtjdogmqim.html

TS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtwpezyyoz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtxxswyqek.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtmjfxrcrl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hywenlv.cn/gtfsmvchlz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtbjphzcsa.html

[H08] 获取错误信息与堆栈
来源：http://hz.c1oappe.top/gtjooofwok.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtywcqdbzs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gttwkakaff.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtbcabcgky.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtakbomhor.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yanxiufei.cn/gtxhjmvzln.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtvjcvqfsg.html

Ruby: e.message;  e.backtrace
来源：http://hz.cashguo.top/gtkzodavkb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pengpengdd.cyou/gtaamrudfc.html

[H09] 带错误码的异常
来源：http://hz.yangfankeji.com/gtwtpoawbi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtqezutalb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ybcxt.top/gtdquxxxfd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtmvgdjynx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cheryme.top/gtuoyqoywq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtvzzdhewp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gtblcydhmr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hongshengwenyu.top/gtfwbdemqa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dashuyun.cn/gtuixrdpet.html

[H10] 资源自动释放
来源：http://hz.ivvv.top/gtusizlrkm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.0kj1m.cn/gtdtbdqnfb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtgyrdeypn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtxzseooak.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtkjqcmobv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtfwaaeacq.html

Go:   defer f.Close()
来源：http://hz.jiagoushi.top/gtkrumzpru.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aibaodan.cn/gtewnlxlai.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtxmdeeviv.html

================================================================================
来源：http://hz.cqqwz.cn/gthrlhsdrg.html

I. 正则表达式
来源：http://hz.meibo888.top/gtgnuwaqlp.html

================================================================================
来源：http://hz.jianghu66.top/gtoirxbidq.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gtfxfnkskx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sysykeji.top/gtakuraolw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shuidangran.top/gtbtfmqwfi.html

JS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtxickrtsm.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtfeoaucvd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtnkqazash.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aibaodan.cn/gtrozuhlzi.html

Ruby: s.match?(/\d+/)
来源：http://hz.xinyue.icu/gtbgbrinsx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtvvludhhs.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtexktxoqo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tian-w.cn/gtirqawcdf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtdpunpcfh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtfausuvfm.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtlbqyexhd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cucudq.cn/gtemgwvics.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cheryme.top/gtgfshzcyk.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtyhqoybnn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nwbrower.top/gtekmbwche.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gthtaqzphb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hysaishi.cn/gtgpkyqieu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtuhmdmucr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guowangkeji.top/gtmicokvyf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtamdvmngw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hywenlv.cn/gtnjnqodys.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gzhubu.top/gtcnzfelpk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.meibo888.top/gtzbyqkuau.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtjsuixjto.html

[I04] 正则替换
来源：http://hz.yonumen.top/gtxzckrunb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gtygbioxas.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtuylqvnpk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtekamnelm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtelaskgfg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zdqjudy.top/gtdzsyxfhd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuetiantiany.cn/gtbethxgxs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gtfyrpbieh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtdmgpjnwd.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtnnijtogb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zdqjudy.top/gttdjxemxg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.svipenyu.cn/gthkogooac.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtjaximcka.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtwhviemuw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangtech.top/gtqlcaxpoa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtizmltsiq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gthwitvfiv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtdqmpnvnh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtwwcbeeqs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtafgjstgx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtwpzikpui.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtvjeeildc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtgylnorlz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtmvuxdyzw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yangfankeji.com/gtzmrhodfq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yvedp.cn/gtczkvwcqm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtlskrjlfa.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhaomingkeji.xyz/gtefzuzzhv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtqmtobooz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtqcpuanjk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtuzbfrltd.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtihrvejvc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.bjfxy.top/gtatbvkllk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtfrrqhygz.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gthdwyjknn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gtoaxpbfca.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ivvv.top/gtqddmsbva.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daria6918.cn/gtivaykrzo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jianghu66.top/gtpvgcnroy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtbtojrkbq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtprukkfvf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xinyue.icu/gtukkrngjw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtfazqczzz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.snrcjt.cn/gtnafjfuxz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gthpjzjwil.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtktgqgczp.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtebcwktym.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbpsbipos.html

[J01] 获取当前时间
来源：http://hz.sufxvd.cn/gtdwgmiugw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhiwuduotai.top/gtlxzftlku.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gttdzbfpju.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtcfxilnre.html

TS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtjozptipg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtcvysgytb.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtankqhnor.html

Ruby: Time.now
来源：http://hz.pycfn.com/gtshzzhwpr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtfkunseqx.html

[J02] 格式化输出
来源：http://hz.dashuyun.cn/gthvgoetsn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtkbwveoxq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtlpvtgvwr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fengsongda.top/gtoveusxwe.html

TS:   d.toISOString()
来源：http://hz.birdmap.top/gtyuwwtleq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guowangkeji.top/gtawosuipt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtmkvzcecz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gthvksfnno.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hongshengwenyu.top/gthogpltvx.html

[J03] 字符串解析为日期
来源：http://hz.nanxinkj.top/gtijwveohw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gtimsymvfs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxinkj.top/gtdzqafnsk.html

JS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtwioopglg.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtgfnhxfyb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtnfoeopbv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtzgxpdqck.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtptbwkbdm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtnztxocue.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtcroasuyu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gtmainmtwi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtwpoeaijb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.snrcjt.cn/gtlxfqcfvs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.snrcjt.cn/gtcfjceldf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtaibxpluf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtuxqpawek.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtfqcuxlrb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtpgjdjmfg.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtdmwswwbp.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtzgicfsuz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtlzijpgnu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtmffrcjpn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtldpoyznt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.smart0.xyz/gtzsmfkbqz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtuwapqugl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangkeji.top/gtaixkinub.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtmokwquyw.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gtuouwymft.html

Py:   (end - start).total_seconds()
来源：http://hz.quarkkingdee.top/gtivtwjscu.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtkhecnksq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtvdmuxofq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhengqikj.top/gtnfqhufwu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtpsjcbhzf.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtwnzjkryx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtfxsshoow.html

C#:   (end - start).TotalSeconds
来源：http://hz.quarkkingdee.top/gtfqgkpzuy.html

[J07] 比较两个日期
来源：http://hz.vqdsnc.cn/gtfvppfmwg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtouykhnrg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtjmiodrzq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtpbfbpuws.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtepjrmnsc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtkqgpaacr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ppjwa.cn/gtnxbbppxr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtrrkwxlum.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtzfbhsahs.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtbhtjdhvy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gtqcklxmzs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtqizwsbqj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtyingejob.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtkehjueco.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gtclnwavrz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tanke756.top/gtjugjumzr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xziqi.cn/gtpvqoifwu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtjypdlyod.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtkawpouye.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tanke756.top/gthigthfku.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtgpsyoqiv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtsolpnros.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtcdfgwybj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtiutxhtga.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtzxnurstp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtajsavfju.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnxiangtu.top/gtslyqtkyy.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigufen.top/gtivhcixmr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtsgpbtjue.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtcwpmohyd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tian-w.cn/gtglutaqak.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinyuanbaomall.cn/gtxhwpzrxf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtabvtxqjz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinghuilouyu.cn/gtqnjvklzy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtdhlrjkzd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtbbkveuyy.html

================================================================================
来源：http://hz.jqgfzy.top/gtuwuvkvta.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtcztopcxw.html

================================================================================
来源：http://hz.sysykeji.top/gtweugveez.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtehdstqnf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtzpcdbmgs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtbemkqubu.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtinmrmmnb.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gteuvocjtn.html


<!-- 参考信息 -->