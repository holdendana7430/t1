代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gtlattwssl.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtlvaijsgc.html

Java: public String getName() { return name; }
来源：http://hz.smart0.xyz/gtiwiuhbyu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtoixtevbm.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtnbtmgadf.html

C#:   public string Name { get; set; }
来源：http://hz.hysaishi.cn/gtcuslvcpd.html

[G12] 对象转字符串
来源：http://hz.sweek.top/gtgimzprhs.html

Py:   def __str__(self): return self.name
来源：http://hz.ppjwa.cn/gtodwjurtf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtugcvledz.html

JS:   toString() { return this.name; }
来源：http://hz.ybcxt.top/gtnjtuvzly.html

TS:   toString(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtrogpidyj.html

Java: @Override public String toString() { return name; }
来源：http://hz.xziqi.cn/gtittdpxen.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtlfsycmph.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gtmyxmjgtp.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtjnlskjmo.html

[G13] 判断对象类型
来源：http://hz.haohaochexian.top/gthalpgogz.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gtsldiiist.html

PHP:  $u instanceof User
来源：http://hz.yj202588.top/gtrljxfblx.html

JS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtnetdbqfa.html

TS:   u instanceof User
来源：http://hz.gzhubu.top/gttaevygkd.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtcaowjmvx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtzxbhheme.html

Ruby: u.is_a?(User)
来源：http://hz.hfpthk.cn/gtenrusfxb.html

C#:   u is User
来源：http://hz.xylfe.cn/gttaqujvtc.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtotdriujx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gtuwmloycv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtprngirbg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtlcilsyqu.html

TS:   type User = { name: string; age: number };
来源：http://hz.gaohongyu789.top/gtnhtomqty.html

Java: record User(String name, int age) {}
来源：http://hz.gogol.net.cn/gtxkzkoilv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fzhhl.top/gtouohpsnr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtytuhekcr.html

C#:   record User(string Name, int Age);
来源：http://hz.zycfv.cn/gtpfrwgios.html

[G15] 枚举
来源：http://hz.yj20258.top/gtxrrbnoye.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtnppavayl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuetiantiany.cn/gtptplfrzg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gtwhchzrix.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtzqbheilq.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gttwkpghjv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtgtshzjjk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cqqwz.cn/gtaeicewov.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtcwvlzmgr.html

[G16] 对象转数组 / 字典
来源：http://hz.ehwqpu.com/gtjzltlsxq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.havefunace.top/gtzsdmosfs.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtgiidopso.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtbwsryrxz.html

TS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtbaelywon.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtkafodcvh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.smart0.xyz/gtbsjqyief.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtlpwnoqsb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhongyouzk.top/gtftfifsej.html

================================================================================
来源：http://hz.0kj1m.cn/gtxhqxezzv.html

H. 异常与错误处理
来源：http://hz.xuetiantiany.cn/gtroonbvhy.html

================================================================================
来源：http://hz.sxryk.cn/gtsylbgmao.html

[H01] try / catch 基础
来源：http://hz.aizwys.cn/gtmzrdyjrh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtxzfyymqg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenjidiqi.icu/gtbssssteo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtijjwwiua.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtkieqwqdn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenlongwang.top/gtnocucjys.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnqzz.top/gtwqfrqnhh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtmzlkwxoz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ywan-chungtsiang.top/gtqcybfxxl.html

[H02] finally / ensure 收尾
来源：http://hz.sysykeji.top/gtskzojbxb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtexvptayg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtjmppiuji.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtopxbtfug.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtgiwxnckd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtuvmklbag.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtnkyonjep.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtmhhdzofp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.316326.xyz/gtkjvrgsor.html

[H03] 主动抛出异常
来源：http://hz.pycfn.com/gtlyonezts.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtivfpiptk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtvwyhubms.html

JS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtwbocmyqq.html

TS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtecjwfkvz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtmzkgitmo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtjzwcitsn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gtfjolxrmp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtcooewdgc.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtteaogevx.html

Py:   class MyError(Exception): pass
来源：http://hz.smart0.xyz/gtvptdoloi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtxtryiljj.html

JS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtqcjjahcu.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtdusefwsl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtlmoarxmk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sysykeji.top/gtxrkwhduw.html

Ruby: class MyError < StandardError; end
来源：http://hz.yonumen.top/gtntvcucjx.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gtdtilnmcq.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtuittrrry.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtgrlwpeem.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ivvv.top/gtwwlepecj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtqzeswlno.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtcplfhskl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gzhubu.top/gtcqrippjw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xingfuxueyuan.xyz/gtaeuclxkq.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtysnbzfrm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtswfixkbj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gtdisllbrv.html

Py:   value = d.get("k") or default
来源：http://hz.0kj1m.cn/gtaxhvqbuc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtpkwmubzw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtaeoekbsn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gthfjdzoud.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gthztksoli.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtvtqtueiu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dashuyun.cn/gtsdozfvrp.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuanzhike.top/gtvqgvpfpz.html

[H07] 断言
来源：http://hz.gzhubu.top/gtqfbkeoxs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gttkxkryqn.html

PHP:  assert($x > 0);
来源：http://hz.daxiang520.top/gtkwvirqhv.html

JS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtcdemwpks.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtxwzgvxrk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gttbycxfdo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gtqdmdxxnx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydjk.org.cn/gtdoisdmvv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtcdrdzlhf.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtekomloir.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ppjwa.cn/gtxqfkoxka.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.haohaochexian.top/gtercczksu.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtasvniorx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtenongany.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtkuvyybsl.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtnldgxsya.html

Ruby: e.message;  e.backtrace
来源：http://hz.dianchejie.cn/gtozqzvvpg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtxkoxqguh.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gtrjxudzaw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtfnexdpiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gogol.net.cn/gtxdctzmcm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxuanxn.top/gtmpsvkpft.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guowangkeji.top/gtxyhcvnsn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtpkthjiui.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.quarkkingdee.top/gttcvvzczd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtzftqrsej.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtomcjuqcd.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtwtphoqte.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gteglvcsev.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zdqjudy.top/gtjjxhcail.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtywnvxnki.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtbatksgia.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtzstqxcru.html

Go:   defer f.Close()
来源：http://hz.wangdashe.top/gthsollmlo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xylfe.cn/gtdjffhmrp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtjvqlidcw.html

================================================================================
来源：http://hz.nanxinkj.top/gtbclvujyx.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtzecimkfk.html

================================================================================
来源：http://hz.sysykeji.top/gtdyieuosg.html

[I01] 判断是否匹配
来源：http://hz.dashuyun.cn/gtbuzbfybh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cashguo.top/gtwthlkger.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sweek.top/gtqyrmwzri.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtnlxfyhlk.html

TS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtejroflzq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtyspfijzd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtqavgsogl.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtdkioctzr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtpyexnzsa.html

[I02] 提取所有匹配
来源：http://hz.yj20258.top/gticvsmeeq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xziqi.cn/gtppqjvlsc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gtnsmbrfyi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cashguo.top/gtsqdmmafe.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtfdwgvwka.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtagjwbdtl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtbmiaprgl.html

Ruby: s.scan(/\d+/)
来源：http://hz.xziqi.cn/gtiztgswhd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gttooncslr.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gtdkyaltzn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daria6918.cn/gtixbakyny.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gtvyzdqewf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dashuyun.cn/gtpjvznxbu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtuwzixgcy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuxming.cn/gtzxmxiowt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgufenzy.top/gtframxgax.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtavafpxdw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gtycbzfcuw.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtxuabxxuw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gttoedgdfk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtvlzwzdcl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtyeehlnwr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtsgjgieez.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtjxamqjwm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gtjqpgcgep.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtzndonpwt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daxiang520.top/gtostmoswf.html

[I05] 按正则拆分
来源：http://hz.haohaochexian.top/gtijlrwrph.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pycfn.com/gtpesgsggw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yonumen.top/gtntdwtyeg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtmvzylbqz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtrweihxww.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtnvnmcrne.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtqbjociyr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtndcvwque.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.vqdsnc.cn/gtvrrydork.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtqqbtdcum.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtmetqnurm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtcbcvmcrb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gttkhvdltp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtmdlglqxd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtvsxlmsmx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guannengcc.top/gtntwhfdfn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhiwuduotai.top/gtprorhdsx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtgjqzkfwn.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtwsjiagtk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gtxvukuzrb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtdnpyvrag.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtwnqtvpcb.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gtrcaifljl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fzhhl.top/gtwgfuhziv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gtfusriurl.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtekxuphul.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtdyciryfq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtavlehfij.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gotoacloud.top/gtsibzxhau.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuxming.cn/gtyvovqksk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtaqtecivn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtfdwpdqhp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtztbeddhu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuanzx.com/gtacwqbfhm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guannengcc.top/gtwktkeojb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtilwnoqyu.html

================================================================================
来源：http://hz.cqqwz.cn/gtircfdfmr.html

J. 日期与时间
来源：http://hz.jinghuilouyu.cn/gtukhkdsay.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrkzwbnba.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtukciajtl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtqvcnwysy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtsipkorvo.html

JS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtbayjadbm.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtezevgchz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhiwuduotai.top/gtbmtugayg.html

Go:   time.Now()
来源：http://hz.svipenyu.cn/gtoxtxsnzf.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtomkjnnwp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtaiapyote.html

[J02] 格式化输出
来源：http://hz.ivvv.top/gtdzawsctf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gthbzwicuk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtdrgrwyja.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gtlrhsdyid.html

TS:   d.toISOString()
来源：http://hz.xinyue.icu/gteebeoeji.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtablcludf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtqfkwriqs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtcccfsibk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.vqdsnc.cn/gtmosgqvxo.html

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gtottbgtyz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnxiangtu.top/gthdxvbbln.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gzhubu.top/gtbeeyjlmd.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtrljjcdek.html

TS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtbgrnnlku.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtpslaukfu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.havefunace.top/gtjnkxcakn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtcppoflij.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtjacmkrrj.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtoevhuzob.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydzc1.top/gtnulmmpqc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtmkndidji.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.feifeiyinyue.top/gtctmbhafd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.iojbl.cn/gtbtsmebkn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.mhx1999.top/gthttcgdsp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.birdmap.top/gtvgxnwgcf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtbfwtbtxb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.feifeiyinyue.top/gtlrwinpde.html

[J05] 时间加减（加 7 天）
来源：http://hz.xuanzx.com/gtmhbjzeov.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtzwbzskns.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cucudq.cn/gtraavkizo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtfpewacbm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtghcazihk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtoecalovv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gtnlgifkmf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhengqikj.top/gtoifbpzcc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.snrcjt.cn/gtkvrpxvdp.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtlgblpsqt.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtpxfralyy.html

PHP:  $end->diff($start)->days;
来源：http://hz.cashguo.top/gtveiwutjn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtkbfhgeqz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gthzjoryca.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.316326.xyz/gtszsmshsr.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtaxxsjqvj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhijiandao.cn/gtdsqcabyn.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtpucryxyu.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gthebgaffu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtbmhtsaop.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtqdsegwge.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtlhcpkcps.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtnywadcnh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtwgqbvamc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jlsjyb.cn/gtuqxcgrat.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gttznzlgdc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtihjgbpfc.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtrgwcxqtf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tianlin.xyz/gtlsjgsotm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtzfuwhcqh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtbvvtjxup.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ehwqpu.com/gtsyiljfuq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtdzrietdy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gtptpyrgxd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtbmgbcubj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gtiqevawrf.html

[J09] 时区处理
来源：http://hz.dianchejie.cn/gtlpzrltny.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtzwomlhdc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtmxokigyb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtnhmipmeh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtmfhmvcyx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhaomingkeji.xyz/gtvhbpmzww.html


<!-- 参考信息 -->