代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.wangshuangyany.cn/gtezhcpvdd.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtjcuuepuw.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gtnyqiawsd.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtypzpvfra.html

Java: u instanceof User
来源：http://hz.guowangkeji.top/gthcvrpyzn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guannengcc.top/gtgarbegta.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gtbutvzsxl.html

C#:   u is User
来源：http://hz.9152youxi.cn/gtwdealpqg.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtxkbqcwkd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gtmowwittj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtfwwiwuee.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hammf.cn/gtczaypbmw.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtjsxqkofr.html

Java: record User(String name, int age) {}
来源：http://hz.zhongyouzk.top/gtyztgxdxd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydzc1.top/gtfniqzwry.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gtfcraivsk.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtheevofjn.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gtfbmzrztu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtmpnknvnu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gthsskfsvk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtbtmsqpnk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gttjmrqrvd.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gtlirdxosu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgfzy.top/gtufbmvbbf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guannengcc.top/gtlquemvet.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtxpkmpxbo.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gteosycoek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ybcxt.top/gtrbqknqda.html

PHP:  get_object_vars($obj);
来源：http://hz.jiagoushi.top/gtteycrjzs.html

JS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtityyvukq.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtttldnsmu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gthsmnapvi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gotoacloud.top/gtfopdyuqz.html

Ruby: obj.instance_variables
来源：http://hz.wangshuangyany.cn/gtkbriblsi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.birdmap.top/gtvaafzaye.html

================================================================================
来源：http://hz.ybcxt.top/gtledrzrax.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gteghfwnri.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnuarzika.html

[H01] try / catch 基础
来源：http://hz.jiagoushi.top/gtvqjfypqp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtkhfinzzk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtrlrrsyrl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtouqfcnev.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gttouwekgp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gzhubu.top/gtihfrvucg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtgcsfmgdn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.316326.xyz/gtoahxqbec.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gtypciymyr.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtokljborm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtaesesdgp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gteantscxd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtrzmcyqpq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtgnpofmwq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtmoczmfxt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gttfrjarll.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.c1oappe.top/gtuyswzncq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yonumen.top/gtibehjyvb.html

[H03] 主动抛出异常
来源：http://hz.hysaishi.cn/gtkfzroaog.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigfzy.top/gtbsgfjxrx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtsllenwku.html

JS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtxgfbxkde.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gteurcrfks.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.havefunace.top/gtvibzorgj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtslapnmfb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gtnhepeitr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gteqqztpek.html

[H04] 自定义异常类型
来源：http://hz.gogol.net.cn/gtdjqurwvc.html

Py:   class MyError(Exception): pass
来源：http://hz.pengpengdd.cyou/gtfrqldxje.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtmqsonkmv.html

JS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtaclvqcpq.html

TS:   class MyError extends Error {}
来源：http://hz.jianghu66.top/gtayzevkus.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yvedp.cn/gtyqzlfmkv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sxryk.cn/gtvjvwlroy.html

Ruby: class MyError < StandardError; end
来源：http://hz.jianghu66.top/gtuajldyuw.html

C#:   class MyException : Exception {}
来源：http://hz.jqgufenzy.top/gthyvruapf.html

[H05] 捕获特定类型
来源：http://hz.cucudq.cn/gtuzoreiib.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gtmndwkuhz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.iojbl.cn/gtjsleiipn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtmspenxxj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtexlqvzhn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gttkiricxy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gtwhzoomvr.html

Ruby: rescue ArgumentError => e
来源：http://hz.kuanghao11.cn/gtqqqsgiki.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtdeoccwsz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtctsfrahq.html

Py:   value = d.get("k") or default
来源：http://hz.52xcode.cn/gtviflujnb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtuiuikwhj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtipxiglcb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtkrubhnpo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shzxlz.cn/gtlzxizgfj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gtqkxysgxc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zycfv.cn/gtndxmvlfk.html

C#:   obj?.A?.B ?? default
来源：http://hz.hongshengwenyu.top/gthdxigtld.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtdkhuhhkg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtknavbquq.html

PHP:  assert($x > 0);
来源：http://hz.vqdsnc.cn/gtdndrjcic.html

JS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtvhyktqms.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtdyqlctck.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhaomingkeji.xyz/gtlaubecyg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sxryk.cn/gtgxsyqycg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.9152youxi.cn/gtldbjpqsr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gtbnywhyzh.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtpjhpfnig.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtjfwmxong.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtxkjhwhpf.html

JS:   e.message;  e.stack
来源：http://hz.yongpay.top/gtkhpzzmzp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtbgquzgqo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhengqikj.top/gtlmabelby.html

Go:   err.Error()
来源：http://hz.yj202588.top/gtsadfyxkm.html

Ruby: e.message;  e.backtrace
来源：http://hz.xziqi.cn/gtkzdxukjx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenlongwang.top/gtzxjewjvx.html

[H09] 带错误码的异常
来源：http://hz.jianghu66.top/gtyucxjsue.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtusiilzyx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258.top/gtlwvqiqov.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zycfv.cn/gtjezqfjkn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtbslwcfzx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.feifeiyinyue.top/gttphneaqe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangkeji.top/gtkchnsecn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cqqwz.cn/gtbwgvbnvw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tianlin.xyz/gthmqnxalr.html

[H10] 资源自动释放
来源：http://hz.pycfn.com/gtrhlybevh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gtwgayterc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yanxiufei.cn/gttkefwmes.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtgeljlzba.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtcygmfoke.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fengsongda.top/gtjlxqgdzz.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gtiuxhplse.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtseptlsua.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gtgrqdfaxt.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfttpqgia.html

I. 正则表达式
来源：http://hz.hnxiangtu.top/gtpojecxyg.html

================================================================================
来源：http://hz.snrcjt.cn/gtixzlbyrp.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gtshihewrr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtbvzjfbce.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtxxkdzaqa.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtnofexzlo.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gttqfyjlyw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ybcxt.top/gtqdlrtcmn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gthzprznxi.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtfwncyjjs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gteldpvqbz.html

[I02] 提取所有匹配
来源：http://hz.xuanzx.com/gtknepzonl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtncmpsibr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtxhbxwbkl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gtzzsiilmn.html

TS:   s.match(/\d+/g)
来源：http://hz.wangshuangyany.cn/gthoemperk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tian-w.cn/gtgwvdwkgr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxinkj.top/gtrjmfvxll.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtglqhavcm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtjutsavoo.html

[I03] 提取捕获分组
来源：http://hz.yj202588.top/gtygmnvwio.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zdqjudy.top/gtpccdnoah.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ybcxt.top/gtgxyjyblq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shzxlz.cn/gthcsgpukz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuxming.cn/gtkitzgsto.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gtnrxxbeug.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtqbdusabh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tianlin.xyz/gtawlgbxwx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtfnxahvel.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gttzuvqpig.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gthydbrddn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtxcceipbt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gttomuotnf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtjeefpkov.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtkemiphas.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangdashe.top/gtttciktyz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhixingplan.top/gtqwecwqte.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gtjumvkiuc.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gtmkskkztw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydzc1.top/gthokhaxbm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtigcezpxb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtonompyzp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtrbtzkttw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gtsnjquzwn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenjidiqi.icu/gtkzxmtvio.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtgyfzcjvf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nwbrower.top/gtpqxcbmvs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtovejqtpw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtnyrjqtsb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.kuanghao11.cn/gtohtyaapp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtxezfjmhm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtfigtrmjm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtifxghqes.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj202588.top/gtdvmwssbh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtatgubbid.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtcnxxvixv.html

[I07] 忽略大小写与多行模式
来源：http://hz.sxryk.cn/gteovckzed.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydjk.org.cn/gtwnsuicpf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangdashe.top/gtoltiiddl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtegquiqgl.html

TS:   /error/gim
来源：http://hz.yonumen.top/gtkgpddkzm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.feifeiyinyue.top/gtmtunhaol.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtchhqtqai.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtqnybnepu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtbnlsbnrh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gttebxrrve.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtwqrfjtgq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dashuyun.cn/gtfjrasodt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gteablckdm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtxfatwbmn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xziqi.cn/gttmxokwrv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.meibo888.top/gtxkvbiluy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yanxiufei.cn/gtnlqvqpzq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zycfv.cn/gtkbahhhdn.html

================================================================================
来源：http://hz.0kj1m.cn/gtpitmucaz.html

J. 日期与时间
来源：http://hz.xuanzx.com/gtqakjqiuf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwuoprkac.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtmgkdxjbh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cdnleiting.top/gtxexbpzos.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtmcyrfmhx.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtfyriedol.html

TS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtnbwbswll.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jyoumei.cn/gtnmxvzfvc.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gtlquygbdc.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtkijnmflm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtfurprnxi.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtxqdqjxig.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtovkgcmrj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtzmudofkc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtugmyvqpc.html

TS:   d.toISOString()
来源：http://hz.kuanghao11.cn/gtcadoaptn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuetiantiany.cn/gtlwxmsgai.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinyuanbaomall.cn/gtfiswllrq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtbtphlfln.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtumzhulzs.html

[J03] 字符串解析为日期
来源：http://hz.daxiang520.top/gtplshcerr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtvoyohjwx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtkjllfybn.html

JS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtoyjzakos.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtqhwukyuw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtfdmtknwf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtnkykcaqg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtkxmzcgwo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xylfe.cn/gtzpaqmego.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtyipwavlj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydzc1.top/gtgxvdpgar.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.svipenyu.cn/gttfkgwcoj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.wangdashe.top/gtggwqukaz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gttzgprydp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxinkj.top/gtefrcyvdk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtrseaghxs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzhubu.top/gtubdwhqlv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gtusmcthqo.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gtjyokxxzv.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtxxdtbwoz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aizwys.cn/gtjunzynrj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtmrrryurf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtymsnpbqf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gteshmrpym.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zdqjudy.top/gtmgyfvfoj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtndsrsrtn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gthyblmyxe.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtoyvodxrc.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gthnzlyooy.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtfvtxqjsv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jyoumei.cn/gtcbqihoac.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtvysfihbn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtroumbqqk.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhengqikj.top/gtmgnzlcsr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gtirtrcybg.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtbyqlkwqi.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gticxnvamc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtfveggtlq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtgzbkrbas.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtvgcttdwd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtkxrowybl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtxbfhsmpx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gthmtymjot.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtxbjqmvmh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtgmambgcq.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtweplymvt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gtgnfgcqgq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gtaqfhygzg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtbajbjssz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtqulepkws.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtcyzvtidx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtwzhjgqzn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinyuanbaomall.cn/gtelqsfgup.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.52xcode.cn/gtytgfpgyk.html

[J09] 时区处理
来源：http://hz.xylfe.cn/gtfaaafqcd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtxaqqihsb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gtsquolczr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtwknedepk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gteatenune.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtljmjrsnc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sxryk.cn/gtealdwqnv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtjxlhbeqt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtpdcgcilh.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtebmnbgly.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gtagcwicpm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.meibo888.top/gtrsugkjvx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.316326.xyz/gtejadricw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtgvgztbcr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtjwyruupm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtuocsdrss.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtycwlygxf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shanyushiyangtech.top/gtjgwtjlcr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gteqwcmces.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gthytcjmpi.html

================================================================================
来源：http://hz.iojbl.cn/gtblibixoz.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtbffdnsbq.html


<!-- 参考信息 -->