代发 wailian999

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtwyrjtosp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dianchejie.cn/gtlxdqyxtq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gtlmgpikzi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenjidiqi.icu/gttiztajiw.html

TS:   type User = { name: string; age: number };
来源：http://hz.ybcxt.top/gtoyqmhlsu.html

Java: record User(String name, int age) {}
来源：http://hz.kuanghao11.cn/gtfajvqwdl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhiwuduotai.top/gtsvcrxjeg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtvjnsypgn.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtiahibqxk.html

[G15] 枚举
来源：http://hz.sufxvd.cn/gtqwmurmpp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtvddkyaip.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hammf.cn/gthruwgeae.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.iojbl.cn/gtkzqwyzqa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtvhdthluu.html

Java: enum Color { RED, GREEN }
来源：http://hz.fengsongda.top/gtkhhwsfec.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fengsongda.top/gtfolutxkn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fzhhl.top/gtmtkbyuli.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtgevlnndp.html

[G16] 对象转数组 / 字典
来源：http://hz.gaohongyu789.top/gthoglanax.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtkgdnxgvh.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtpyuizyjn.html

JS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtysyvggpp.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtkbicfrme.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigfzy.top/gtmflpiagb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtctopboyr.html

Ruby: obj.instance_variables
来源：http://hz.redwolf501.top/gtdogbgrcp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.kuanghao11.cn/gtyixrxnrc.html

================================================================================
来源：http://hz.jianghu66.top/gtkskndckc.html

H. 异常与错误处理
来源：http://hz.yueranfly.top/gtirfirtgb.html

================================================================================
来源：http://hz.jinqigufen.top/gtjmuwltsh.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtohuhtgpk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuanzx.com/gtgbwzqizv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ybcxt.top/gtjnxeyhlg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtmktmvrex.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtifllnkcf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sweek.top/gtdqdxyoqb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtgabgnpqy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jlsjyb.cn/gtmxtlckei.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtlhztszgi.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtqxmznivq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtjadwmtke.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtjqnamhbn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gterkifnbl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtfcbjeduv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gttlqpshnu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtsthwrhzs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtnybqavig.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtkxgsvsgi.html

[H03] 主动抛出异常
来源：http://hz.cheryme.top/gtzgorpckg.html

Py:   raise ValueError("错误信息")
来源：http://hz.iojbl.cn/gtvnwvgeaf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtxbltvlgy.html

JS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtfwwewoky.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtinqxivet.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtsmiikexw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtmuflrrya.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtefxkueyr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtshrudvnh.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtgpyocpgx.html

Py:   class MyError(Exception): pass
来源：http://hz.hnqzz.top/gtejrcdxzv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtxtknguuf.html

JS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtserpssse.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtxivnvdhg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtsbwrhrbf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gtmmdiqrqn.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gtbemxbpfl.html

C#:   class MyException : Exception {}
来源：http://hz.zhijiandao.cn/gtrjgbgelw.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gttprpnpva.html

Py:   except ValueError as e:
来源：http://hz.gzhubu.top/gtfwxeplgi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtsaffplnk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gthprxugwa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtlpquvpuy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cqqwz.cn/gtreyedrjt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pycfn.com/gtdjdncjty.html

Ruby: rescue ArgumentError => e
来源：http://hz.tanke756.top/gtktppctbj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtswljtnhk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtgcytsofo.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtmmsotzok.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cashguo.top/gtfokfayef.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtavjdcqlo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtwvrjddzm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fengsongda.top/gtvayzygux.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gthntxgpro.html

Ruby: d&.dig(:a, :b)
来源：http://hz.snrcjt.cn/gtqezjqhlr.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtpioifiav.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtqqdohonc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gthbunkjjz.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gtiohusgld.html

JS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gthtjdjseb.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtcpuupjjh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gtizgqeeec.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.kuanghao11.cn/gtpcxpguta.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gtjsdlwwqe.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ivvv.top/gtgwwpnqcu.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtclykbwiz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgfzy.top/gtiypofiki.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.9152youxi.cn/gtcqqzywem.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtunzglhrp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtvvnjishq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtblmgwxvc.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtxlntwxiw.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gtjmijqnub.html

C#:   e.Message;  e.StackTrace
来源：http://hz.9152youxi.cn/gtnidgrnht.html

[H09] 带错误码的异常
来源：http://hz.chenzaomai.com/gtscjgusjh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cdnleiting.top/gtawdjbizw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtquycockj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtxktarmjh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gttmuqoqpi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtfxtaqtat.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gticsohlfj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtpgpmwass.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgufenzy.top/gtpsxksgkb.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtwfdggafg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.bjfxy.top/gtcvnzpkam.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtkyicxhwj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtrmbsfjai.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtcykspogu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtvgrzlhhb.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtqumrhrjh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gtjmeqqcvx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtlivomljc.html

================================================================================
来源：http://hz.ehwqpu.com/gttofgcrko.html

I. 正则表达式
来源：http://hz.yj202588.top/gtucmjqkqn.html

================================================================================
来源：http://hz.cashguo.top/gtbxvyakgv.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtjzyefrob.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtxwhxwiwk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtvdsirmka.html

JS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtiilttjwb.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtuhqvpwet.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sufxvd.cn/gtrcuzpbzb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxuanxn.top/gtnfiapsow.html

Ruby: s.match?(/\d+/)
来源：http://hz.sweek.top/gtboxzgsrb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuxming.cn/gtffimqlvt.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtjasjgwtk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtizlgvhtx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guannengcc.top/gttuhcyore.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtffhwigol.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtopdszlsb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtcdufzxuv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtrvotugnr.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtwajcwuhe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ppjwa.cn/gtyahkfjjp.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtsnofsxdr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtndhozovn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtodbsxzxh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhoulong.xyz/gtobhszsws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ehwqpu.com/gtqncnlqwg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtqrlpduqr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangshuangyany.cn/gtkwaqybqb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtzobvkhko.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shanyushiyangkeji.top/gthntpivbb.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gtohjdvvgg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gtewlvsyzd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtkrffxdsr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtdxitwnwz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtebtxuodv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shangyingyoupin.top/gtdckisfkq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtdzurgddf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zycfv.cn/gtceiidfzj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yonumen.top/gtvtbjpylf.html

[I05] 按正则拆分
来源：http://hz.yj20258.top/gtvwckflcr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ehwqpu.com/gtquygmjlh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.svipenyu.cn/gtlbsimajz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtphnsbjnu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtaudpmxxw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gtibvbrath.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtwlaojobn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtmzjwkhuu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangkeji.top/gtjimildoa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinyuanbaomall.cn/gtulklizou.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtuzawoapx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ppjwa.cn/gtpshszwgx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtejgbbatm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtfdpcinfs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gtmurzmlmc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgufenzy.top/gthbbndegt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtodxgtlsc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gthjukwnkq.html

[I07] 忽略大小写与多行模式
来源：http://hz.ppjwa.cn/gtsqqyiybo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtczbghoyq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hammf.cn/gtdflesmsr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hongshengwenyu.top/gtzyxgphkl.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtisrcinru.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtqoacdvmh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtguroestw.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gtprwvcwam.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zdqjudy.top/gteivgyavw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tanke756.top/gtyikdzthn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.meibo888.top/gtdejotqov.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.quarkkingdee.top/gtxnetitky.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtzdkbgwli.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtcrzawesw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtmiwtvved.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtteiqcixe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jianghu66.top/gtmchhkfzq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gttmtyqqkv.html

================================================================================
来源：http://hz.yj20258.top/gtrzaiusuc.html

J. 日期与时间
来源：http://hz.cqqwz.cn/gtlsofamvw.html

================================================================================
来源：http://hz.nwbrower.top/gtizrcugsk.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtxsnshzhl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgfzy.top/gtdrokcotz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtgphmhezi.html

JS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtlgtaonkf.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtkrwvjatw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gthhswaqko.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gtbzxhqapf.html

Ruby: Time.now
来源：http://hz.zhoulong.xyz/gthtacsict.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtvrkgyote.html

[J02] 格式化输出
来源：http://hz.jinqigufen.top/gtirixvopa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtauxddost.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtxxcfhycb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zdqjudy.top/gtkqjsfbkz.html

TS:   d.toISOString()
来源：http://hz.jianghu66.top/gtszsoauol.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydzc1.top/gtucrntcro.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gthifvwske.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtkcwagjxv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj20258888.top/gtbhnfyccv.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtyjqxfnpy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ybcxt.top/gtkmqpkysl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtzmecnklg.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtipdcrdse.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtuicieydo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtozyfquor.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtsuqhmvnn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtmllepruc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtzvbsywly.html

[J04] 时间戳与日期互转
来源：http://hz.0kj1m.cn/gtkqoqiffx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtbauzipzq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sweek.top/gtbfgiozuq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtpnkzvvux.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtqaeneimp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gthawwmnse.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gtptkuwrpl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgufenzy.top/gtjprpllhz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ehwqpu.com/gtaleubqpy.html

[J05] 时间加减（加 7 天）
来源：http://hz.bjfxy.top/gtteavtgyx.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gtmlmfigop.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtbbvdnbpa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtxvebgvqa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtascqfvhm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigufen.top/gtodfrbafn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtrfpovvjj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gthymwnqat.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gaohongyu789.top/gtrujlgdrn.html

[J06] 计算两时间之差
来源：http://hz.quarkkingdee.top/gthhbwsrve.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtwlsdfqim.html

PHP:  $end->diff($start)->days;
来源：http://hz.guannengcc.top/gtpdznrngo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtptpsjgzj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangdashe.top/gtzolkpsjg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhijiandao.cn/gtimbzqfdb.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtaazkdjoq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gtdslndees.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinghuilouyu.cn/gtzicrsgyr.html

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtowdjrxeo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtqzlxnalh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtsmvefhzx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtzsgmxbhq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtzisbcjbl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtcoumnrxg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.vqdsnc.cn/gtsznaxzta.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtilomttyd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtxcwicfcp.html

[J08] 提取年月日与星期
来源：http://hz.zhoulong.xyz/gttnhxrdzv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtkadjxmvw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtrtzvskjz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtmmzqndog.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gthtxodcvl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pycfn.com/gttefwuheg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hywenlv.cn/gttwawmidh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtdawcydeg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yonumen.top/gtpxuygjyg.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtifetdmkm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtmloeyqij.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhaomingkeji.xyz/gtwgydkjyq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtfwyjphcz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gttkhhxxuz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hfpthk.cn/gtucguucey.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtmhyrnibl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.pengpengdd.cyou/gtncuiifga.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.52xcode.cn/gtrqtoyqnx.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtrqapmknt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtwtllsihy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangtech.top/gtpizworzo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtzngpnmvc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gtditpxwas.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydzc1.top/gtjyztbnff.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gaohongyu789.top/gtuhjskitn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gtpzekujhm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.vqdsnc.cn/gtpjdbmhip.html

================================================================================
来源：http://hz.redwolf501.top/gtcsvaucsc.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtlzwjkhiw.html

================================================================================
来源：http://hz.zdqjudy.top/gtnkdnkqam.html

[K01] 对象转 JSON 字符串
来源：http://hz.meibo888.top/gtcqqycbgo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtllibyxkv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gthcyadefe.html

JS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtkxcvfatu.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtemxjxjdr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtbksaeueo.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtecdhctht.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtnuscdnrm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtrhprllvh.html


<!-- 参考信息 -->