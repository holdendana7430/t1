代发 wailian999

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtjmtsqfqw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hywenlv.cn/gtsoshkgrz.html

Ruby: u.is_a?(User)
来源：http://hz.sxryk.cn/gtplxuamtt.html

C#:   u is User
来源：http://hz.meibo888.top/gtwgwglvik.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtruwogtcs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hongshengwenyu.top/gtdhnoffqy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtxpveyztk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtnzjafiqm.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuetiantiany.cn/gtmwrpvpjh.html

Java: record User(String name, int age) {}
来源：http://hz.nanxinkj.top/gtnngotgwq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtcowhfwvg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtnlmvwtac.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gterrxpauf.html

[G15] 枚举
来源：http://hz.jqgufenzy.top/gtvgjxzvhe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yonumen.top/gtqdjehtuv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.9152youxi.cn/gtbqfsypfz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gtgthobzzd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtobsmqlat.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhoulong.xyz/gtlwqnpztf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jiagoushi.top/gtbhemfwmm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtpnxkobek.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtefnnzuap.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtljubzaxl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtjsmuumdb.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtzgblpcxg.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtwhcdldre.html

TS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtqbxtvezo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtwklqcdse.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gttmqvacpb.html

Ruby: obj.instance_variables
来源：http://hz.ybcxt.top/gtoefmhted.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gtttukdlra.html

================================================================================
来源：http://hz.fzhhl.top/gtohgzxcrr.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtsfmpasuh.html

================================================================================
来源：http://hz.gotoacloud.top/gtmdgkaakt.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtkivsuyza.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtexgcskdo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gtmyxfgmpx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtmfiaurew.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhengqikj.top/gtfnmrdqpi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gttsjzkguf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gteonskurg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtuoaezhog.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cqqwz.cn/gtyqloeyoa.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtllivnizm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.mhx1999.top/gtmzstvytn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtnvvwshht.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gthqgekedk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtrononnfz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtigmmpvxy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sysykeji.top/gtozeprfrj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuanzx.com/gtnttxeyli.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ivvv.top/gtlredhbdr.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtphnyiaib.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtcotacnoy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtutysfvjd.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtlvedyhkc.html

TS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtsdezuaii.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtkvgvvnwx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuanzhike.top/gtprwrrads.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shangyingyoupin.top/gtflrlqdju.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtktyuwjub.html

[H04] 自定义异常类型
来源：http://hz.yj20258.top/gtubqyealf.html

Py:   class MyError(Exception): pass
来源：http://hz.gaohongyu789.top/gtkbcpfcak.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtndwnjsfa.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtoghjcbuw.html

TS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtecfdhllb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gteagwjtew.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.redwolf501.top/gtpfgqvlru.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxinkj.top/gtdctjjvkn.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gtujyhnvog.html

[H05] 捕获特定类型
来源：http://hz.meibo888.top/gttoegfxxl.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtkjaiaaao.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gtrmttxzfu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gttknlrkje.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtwnezdfjl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtkeiipogy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.52xcode.cn/gtaodyjupu.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtpvxtclox.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenjidiqi.icu/gtosyhsgvr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtyvfsymhy.html

Py:   value = d.get("k") or default
来源：http://hz.ywan-chungtsiang.top/gtebiyybxn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydzc1.top/gtfystlghd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtzhefwvms.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtvgfdvykt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtsdvomozg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ehwqpu.com/gtdpjqubyb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.smart0.xyz/gtzugylrmt.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtzlaqgxxb.html

[H07] 断言
来源：http://hz.ivvv.top/gtwqvmwunh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtnzvdvkdm.html

PHP:  assert($x > 0);
来源：http://hz.tianlin.xyz/gtvxerctql.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtrgqqrrie.html

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtfojywwpq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gtkfrbgayq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gttbqbxldn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtrwpvsgle.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gtezkqquup.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtzdrjtgyu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daxiang520.top/gtjienwqzv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtyescxjkc.html

JS:   e.message;  e.stack
来源：http://hz.shuidangran.top/gtffphqvpm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xinyue.icu/gtpqcxnnfb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtnhxyjfex.html

Go:   err.Error()
来源：http://hz.hywenlv.cn/gtqbdhrufh.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtvizwseqg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnqzz.top/gthqllcfht.html

[H09] 带错误码的异常
来源：http://hz.aizwys.cn/gtweohhaoo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.52xcode.cn/gtvvvpjshd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtubxukvmf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtcrpdktln.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.vqdsnc.cn/gtjrvnffwv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtmkjhsynm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.9152youxi.cn/gtxqwlyjah.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhongyouzk.top/gtuksrwjgo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guowangkeji.top/gtdgirjxwa.html

[H10] 资源自动释放
来源：http://hz.vqdsnc.cn/gtbnbspblh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ybcxt.top/gtvmhkdxhp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtqyfpkaip.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtdohhbzfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtpwkzczzi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigfzy.top/gtasbqjrfc.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangkeji.top/gtcgyovxas.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hysaishi.cn/gtifgszvrw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenjidiqi.icu/gtxqlgkrem.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtiwhdqfds.html

I. 正则表达式
来源：http://hz.sysykeji.top/gtqdypkgcf.html

================================================================================
来源：http://hz.hnqzz.top/gtrodjsgkd.html

[I01] 判断是否匹配
来源：http://hz.birdmap.top/gtorfvrdue.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gthhwpamsi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gtivnwaqwh.html

JS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtvxvkuwvq.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtfooimxos.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtlppvvxrn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shuidangran.top/gtafqusmea.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtzbcdjyco.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtruwjbovd.html

[I02] 提取所有匹配
来源：http://hz.cqqwz.cn/gtfuedhfil.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gotoacloud.top/gtorxncyja.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtnrftyndu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tian-w.cn/gtfjbioxpb.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gtcqgfixiv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtbdjfuzde.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pycfn.com/gtxlqjrhpm.html

Ruby: s.scan(/\d+/)
来源：http://hz.hywenlv.cn/gtqsxamemm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtbggqnjcf.html

[I03] 提取捕获分组
来源：http://hz.svipenyu.cn/gthctkjrrr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtnekpfycr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtqqfzshxf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gttnjjgwwp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zycfv.cn/gtgsvlwadn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtpfbiqosz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gtcrmznixj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtpxjmftcp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtcfpzzbhe.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtdqjodmfs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtwuvpqbem.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtewigukbi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtgqdpgbca.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtfqbfrvpi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtzdonwgto.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yueranfly.top/gteconyiad.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangtech.top/gtodrdxxft.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtirhrfptd.html

[I05] 按正则拆分
来源：http://hz.9152youxi.cn/gtoolvzkmu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuetiantiany.cn/gtchuuzdhr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gtbnubcevw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtfqemahga.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtfavrlsot.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gttnigthpa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtycmwiymt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtoinfzgom.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.52xcode.cn/gtituoqtea.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtnestwily.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtivmpnnjh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtzwuvggtj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtlhrcbubs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuetiantiany.cn/gtcssjfdiz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shangyingyoupin.top/gtumjcqlci.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.vqdsnc.cn/gtswofrnqa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.bjfxy.top/gtqggnottb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtmvxostyu.html

[I07] 忽略大小写与多行模式
来源：http://hz.0kj1m.cn/gtffguyvyp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jiagoushi.top/gteokylbon.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guowangkeji.top/gtxojoxulx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtypwvjyil.html

TS:   /error/gim
来源：http://hz.cdnleiting.top/gtccydxpwz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gteitmshkj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtittifuqi.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtodqjzbkx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtjrkkcvjb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgufenzy.top/gtearzhdwh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtoublwkqj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtgpeeaxzt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gticflunmq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtvclhnufl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gtdaqebthw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtfltxnoxi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtwmdyruyd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtukyaxvao.html

================================================================================
来源：http://hz.xuanzx.com/gtwnplurwe.html

J. 日期与时间
来源：http://hz.kuanghao11.cn/gtcjwrxwzp.html

================================================================================
来源：http://hz.yangfankeji.com/gtmdywkasu.html

[J01] 获取当前时间
来源：http://hz.hongshengwenyu.top/gtssqgfwfg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtrqacwzje.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtoekquvkl.html

JS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtixgrckel.html

TS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtqlprxjmz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cucudq.cn/gtyapscusj.html

Go:   time.Now()
来源：http://hz.cqqwz.cn/gtevirobyo.html

Ruby: Time.now
来源：http://hz.nanxinkj.top/gtynmvbadb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangdashe.top/gtqbyefndt.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtasmsfzng.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtyukaikha.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtidgozini.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxuanxn.top/gtxehpneng.html

TS:   d.toISOString()
来源：http://hz.svipenyu.cn/gtinlllpcb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtpyaakrmx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gthluixaix.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtvxllurog.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtsajgnwxb.html

[J03] 字符串解析为日期
来源：http://hz.jlsjyb.cn/gtdzstmybd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guannengcc.top/gtffahjhdd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtwxfpijkn.html

JS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtbnbbxotj.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtvhjmrivw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtarftdrdg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.316326.xyz/gtsnuyimjn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtfghjjzoy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtmogiqhkl.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtifeukvmx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtkssmuvlc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gttbscpmxx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtkidbaynl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangshuangyany.cn/gtmorupzdi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtfadjstrp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sxryk.cn/gtovfahsnk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtoajknhci.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtzydzplmz.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtgtcxgjla.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtxiecayqe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yonumen.top/gtapvrkxxw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtvactthik.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gthklpjpeb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gtwdzlyltf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gtmxlhuqth.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtydajbhdy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtmdyjuili.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtmlufknmv.html

Py:   (end - start).total_seconds()
来源：http://hz.svipenyu.cn/gtaayyaame.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtxnknumju.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtvpihytez.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtvechnhlu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtqvvhmujt.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtajbnjbxc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtmflztdja.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtmwrtscaz.html

[J07] 比较两个日期
来源：http://hz.tianlin.xyz/gtzpwmuuza.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtdwilmznt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gtrrxvusco.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtfhevvwcb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtovfvjytt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.vqdsnc.cn/gtctziiyvc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtxjpffclz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtmpbrbfbi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gteafrmgni.html

[J08] 提取年月日与星期
来源：http://hz.yuanzhike.top/gttjxpgxaa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtawmcwemr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gzhubu.top/gtgtyiacck.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.smart0.xyz/gtghzpmrcv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtrdhmpupj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtecmanjwk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtucysnypr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xziqi.cn/gtalerwrjp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gtigheqxyk.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtepshhdkk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtrqsxvcis.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhaomingkeji.xyz/gtwggutouh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtndmiopsz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtuurjhzzl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.birdmap.top/gtreflkghx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dianchejie.cn/gtauzliice.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gtexpbrwij.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daria6918.cn/gtdpoqmmfe.html

[J10] 取今天 / 本月第一天
来源：http://hz.feifeiyinyue.top/gttkfftzfj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gteyayocek.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gtqtqkjdgt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nwbrower.top/gtobhogjnm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gtaiuekuqm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zycfv.cn/gtahzyslcr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtkmexispi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtdvplrnlf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sysykeji.top/gtcqwulchi.html

================================================================================
来源：http://hz.316326.xyz/gtbgzztatl.html

K. JSON 与序列化
来源：http://hz.quarkkingdee.top/gtguadyloi.html

================================================================================
来源：http://hz.daria6918.cn/gtehaayeks.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtmjnvaysv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtcwnadsoh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtomgaohfm.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtrpozyqin.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtlrsaepks.html


<!-- 参考信息 -->