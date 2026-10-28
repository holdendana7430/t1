代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtpfovkwbx.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtfzmjzjpr.html

JS:   u instanceof User
来源：http://hz.fengsongda.top/gtvolxfrpy.html

TS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtczqduuoy.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtdruiwqey.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuetiantiany.cn/gtqyppxpgf.html

Ruby: u.is_a?(User)
来源：http://hz.feifeiyinyue.top/gtcoiowrlf.html

C#:   u is User
来源：http://hz.52xcode.cn/gtxitecplp.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtjucagliv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yanxiufei.cn/gtegbdfqwe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtpijqqqbl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtxpxzclha.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gtbcvpwsix.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtivitcceu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.andypj.xyz/gtehtqgbrb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtqcdbuegn.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtkwckdsuh.html

[G15] 枚举
来源：http://hz.ppjwa.cn/gtcmphtfrr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.iojbl.cn/gtfsajsjlg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gtdtuiafgv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhiwuduotai.top/gtsumyedls.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtsdogtoqc.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtweabayyz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.bjfxy.top/gtiebundce.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgufenzy.top/gtwqtmszln.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtelfcavdl.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtdgenjiyi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gtlxvwgpql.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtwvuqfpoq.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtxuqpjmyh.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtgwordihc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtyaubhtln.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgfzy.top/gtlpgvljqk.html

Ruby: obj.instance_variables
来源：http://hz.fengsongda.top/gtfvdntqay.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtyoyirwvq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtztdidvcc.html

H. 异常与错误处理
来源：http://hz.c1oappe.top/gtwewxqibo.html

================================================================================
来源：http://hz.shuidangran.top/gtssszaofi.html

[H01] try / catch 基础
来源：http://hz.daria6918.cn/gtuaxqljgk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtaqylpwxa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtmqhuohrg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtjwgxuuek.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gtxxbdfbvu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtmymtqypq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hywenlv.cn/gtgovxyhlw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.smart0.xyz/gtxedwabgs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinyuanbaomall.cn/gtuzmivnel.html

[H02] finally / ensure 收尾
来源：http://hz.jqgufenzy.top/gtahuhbjhw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jianghu66.top/gtruldruzd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtxxvektri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtvcsjlxag.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtwnvyjlxp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtcenyaaue.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xinyue.icu/gtprrledqd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhijiandao.cn/gttdqzsrlf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydzc1.top/gtisnammus.html

[H03] 主动抛出异常
来源：http://hz.jinqigfzy.top/gtipbqxise.html

Py:   raise ValueError("错误信息")
来源：http://hz.zycfv.cn/gtlgmqkrut.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtzcaibeqp.html

JS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtvjkgbbpm.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtvnnvsyxs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gturywbybe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sysykeji.top/gtksjinoip.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtkfnjnoyp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtreymzvao.html

[H04] 自定义异常类型
来源：http://hz.gzhubu.top/gtizhpzwey.html

Py:   class MyError(Exception): pass
来源：http://hz.gogol.net.cn/gteemxuekb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtbufcrlut.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtzxutvwjc.html

TS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtkumwxeao.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtyubkknvr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnqzz.top/gtrahcncic.html

Ruby: class MyError < StandardError; end
来源：http://hz.yanxiufei.cn/gtgolgvzfr.html

C#:   class MyException : Exception {}
来源：http://hz.52xcode.cn/gtqhwlpkea.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtzovfvsxg.html

Py:   except ValueError as e:
来源：http://hz.yj20258.top/gtapygawcb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.bjfxy.top/gtgtojgioz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtqevbztcr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gttvtyynag.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtwnckzfwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ybcxt.top/gtmlufwsdr.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtdqzgxgpj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtfjgfscne.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ppjwa.cn/gtzwqwjble.html

Py:   value = d.get("k") or default
来源：http://hz.wangshuangyany.cn/gtcjzshdxd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj202588.top/gtwtcylgxo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtcjylacgj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtniittpeo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cqqwz.cn/gtufnjgglz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cashguo.top/gtqsdbhaza.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtcxacdrlr.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtfxamkthz.html

[H07] 断言
来源：http://hz.jinqigufen.top/gtvfvkkine.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtuonzufnb.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gteiinirve.html

JS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtswvllthb.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtskjujvki.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuxming.cn/gtgyqvlpjr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtlsclydim.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtuyjmyrop.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtdpzeqhal.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtsauikyij.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgfzy.top/gtykhlxzez.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuxming.cn/gtihvjwcbo.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gtmrbyshqw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtjsmvzjbf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gttvlgdcak.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gtgeivyygl.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtckatkvdl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtipdnhcbt.html

[H09] 带错误码的异常
来源：http://hz.iojbl.cn/gtyvdvjktf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtjgsqaptw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gtxfwwinwn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtofcryuei.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtccljzjoz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtaoxtrryp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtigjiednd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtnwyzsojx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtxuoroexy.html

[H10] 资源自动释放
来源：http://hz.redwolf501.top/gtecizchhe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gthizlnvfg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aibaodan.cn/gtlqdgdaae.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtndxidamd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtmwjxebpe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gtqrpnpkjc.html

Go:   defer f.Close()
来源：http://hz.dianchejie.cn/gtyjzgrvre.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtnxnaiddi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sysykeji.top/gtjcdvtmkc.html

================================================================================
来源：http://hz.hfpthk.cn/gtkansrvnj.html

I. 正则表达式
来源：http://hz.zhaomingkeji.xyz/gtvghppslq.html

================================================================================
来源：http://hz.ehwqpu.com/gtjcwcbigh.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtiezkvbtp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtlhnxfmgt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ivvv.top/gtvlgjslnb.html

JS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtkbvkkdiw.html

TS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gttoggcipo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtkdfryrjh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gticjjsmul.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtdnxpejon.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zdqjudy.top/gttrnpgqiv.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtzegrvudz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cheryme.top/gtmjywoval.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnqzz.top/gtiguprzvy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xziqi.cn/gtonheodiy.html

TS:   s.match(/\d+/g)
来源：http://hz.316326.xyz/gtosiimtna.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shangyingyoupin.top/gtkrxnptzt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtzftmpswc.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtafxvimkp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtvqbthgsg.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gtyyfnukgs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pengpengdd.cyou/gtmfgxbwro.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtqfgyetie.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gteequjtmz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gtjngjjbto.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jiagoushi.top/gtoqknmnbb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gtjjafdmbf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tanke756.top/gtqlcxqfuv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gttrcfqguz.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtzqgkpbxy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuxming.cn/gthhculacc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtfhhgqtyi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtnnprvjwe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtfeyshokk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtwlpwfeaf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtznyfrtln.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtzjnuufsc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yanxiufei.cn/gtenbqfivw.html

[I05] 按正则拆分
来源：http://hz.hongshengwenyu.top/gtnjzzanza.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gtuhqhwqod.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtvskyxmny.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtfrbvoqse.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtxebytjau.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cashguo.top/gtyrynqkqp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zdqjudy.top/gtgfimpwgh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtwypgvgdo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuxming.cn/gtezjgwrgn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhiwuduotai.top/gtjchqoann.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtsdpuvhoj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtqxnvrzwv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtbojoggen.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtlwvcfkgg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zdqjudy.top/gttghmnfdf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtjoatuuim.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtqlyevkxl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtujrdckuh.html

[I07] 忽略大小写与多行模式
来源：http://hz.xinyue.icu/gtxdolrbrk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtakxxjhkc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gtupgmuzel.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtbfwzxtpi.html

TS:   /error/gim
来源：http://hz.cheryme.top/gtapxjzcwa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gthymikitw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtzbyoechb.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gtlgrzjmnf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtnefdcjxa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtqtrkirfn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtrdnicfpg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtyvsdzxyq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gtwcwkjris.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtoylfkcof.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtjydxtsvx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.guannengcc.top/gtfxszhzrq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtqxmulqkx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtxpkzyqze.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtsnynlgxq.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtdnyodmnm.html

================================================================================
来源：http://hz.zhixingplan.top/gtecrsymtk.html

[J01] 获取当前时间
来源：http://hz.jinqigufen.top/gtqjtbzach.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtcaubcsvp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtnkndmgjj.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtwuulcclc.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtrhgxqmyl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnqzz.top/gthmwnfmmz.html

Go:   time.Now()
来源：http://hz.redwolf501.top/gtcvnkekqs.html

Ruby: Time.now
来源：http://hz.zhaomingkeji.xyz/gtcrrfofzb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.havefunace.top/gtsztculsl.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gteyovxqte.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gteiyulbjr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtkfqgyjra.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj202588.top/gtptlctera.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtniabedbb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinghuilouyu.cn/gtkgsyrvlm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtiufkcmzy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtvvmehfkt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnqzz.top/gtxnsqmugo.html

[J03] 字符串解析为日期
来源：http://hz.zhijiandao.cn/gtrsqnaevi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fzhhl.top/gtmomjivji.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtekytserj.html

JS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtuvvuhdoh.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtrfwelbqn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtqplghfte.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtprqflhcf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtkedjydok.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shuidangran.top/gtxzdqwlyr.html

[J04] 时间戳与日期互转
来源：http://hz.hywenlv.cn/gtakppxzvw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aizwys.cn/gtbvzgqnat.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hysaishi.cn/gtnrlpstyg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigfzy.top/gtoantorfs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtaunylyqc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.9152youxi.cn/gttdewsmde.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtdcmjgdmn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fzhhl.top/gtrwidejow.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtvicuacbz.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtfsuddssl.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtmkrbscak.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gaohongyu789.top/gtvgygfxzr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtwbfzxxnf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtgdxiiasa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guannengcc.top/gtzgsrhxnk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gtsecrikbj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtdoxwjaqo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gtqpwiegxu.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtqhsnqsrs.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtjrnhebfh.html

PHP:  $end->diff($start)->days;
来源：http://hz.shzxlz.cn/gtfbvpdkxg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtdyysbuqy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuetiantiany.cn/gtjkvnvduw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.kuanghao11.cn/gtibiduvkf.html

Go:   end.Sub(start).Hours()
来源：http://hz.ppjwa.cn/gtbwotoqzr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtkdqidprq.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtfisoeoxz.html

[J07] 比较两个日期
来源：http://hz.yangfankeji.com/gtsjvpsfwd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtlsendeag.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gtshgylgws.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtbkhynhlc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtgcbcgdmk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangkeji.top/gtxbidpbfa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtgbvfcfmx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtdthjlbkv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtowbgxcpb.html

[J08] 提取年月日与星期
来源：http://hz.xylfe.cn/gtokyfvdug.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtmmjepnbt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenlongwang.top/gtmangyxei.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtdylsshet.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtqmdtrizc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigfzy.top/gtphftybqe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtnfzprbkv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtgzatrcod.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gtnyhssgmc.html

[J09] 时区处理
来源：http://hz.hnqzz.top/gtkwgtgkzg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nwbrower.top/gtvaawoccp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nwbrower.top/gtlsjqvlsk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtblisetfl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtbszqgvup.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guannengcc.top/gtdzifcmid.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtdxmhebzs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtpcoaqrul.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtesmiivmm.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtvvnvqicw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.iojbl.cn/gtcciiatjn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtbkzbrylx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hfpthk.cn/gtzmunsvuc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gturzionph.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtswmakzlc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtwlufvvpp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gtcuoduejy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhixingplan.top/gtacsehowq.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwhehzmau.html

K. JSON 与序列化
来源：http://hz.redwolf501.top/gteqthqqjq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlrrussby.html

[K01] 对象转 JSON 字符串
来源：http://hz.sweek.top/gtwnzomcip.html


<!-- 参考信息 -->