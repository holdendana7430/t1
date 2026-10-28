代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtgpvoibgw.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gtxpukbqbv.html

Py:   @property 与 @x.setter
来源：http://hz.jyoumei.cn/gtobmplrlv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtdurhkahe.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtwewgkrjy.html

TS:   get name(): string { return this._name; }
来源：http://hz.hysaishi.cn/gtmzaoykcd.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gtjntlgmcx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtdhjysdgc.html

Ruby: attr_accessor :name
来源：http://hz.zhijiandao.cn/gttpezoenu.html

C#:   public string Name { get; set; }
来源：http://hz.iojbl.cn/gtshimdtlc.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtnlfcebxx.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtjrstjeaq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtbqtvtkmh.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtwrtanbvg.html

TS:   toString(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtrreuaklb.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtwhqyvtrp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daxiang520.top/gtsyrqrukn.html

Ruby: def to_s; @name; end
来源：http://hz.smart0.xyz/gtuwxdmvts.html

C#:   public override string ToString() => Name;
来源：http://hz.gzhubu.top/gtsmtlrpkc.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gthorvmyiw.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtcdqbbqze.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gteaxbfohx.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtnzajmolk.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gtiiwnsvbw.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gtyifyfuvm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtosrofdpw.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtgdpvmhqb.html

C#:   u is User
来源：http://hz.ppjwa.cn/gtangrmxnw.html

[G14] 数据类 / record
来源：http://hz.ydzc1.top/gtbpokmfkx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuetiantiany.cn/gtkxaoveux.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.52xcode.cn/gthqshlogn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtilefdivs.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtzfrtpxni.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigfzy.top/gtsxrxgjbj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtuwkfurwk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gtlvnfrtye.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtyzdwsgby.html

[G15] 枚举
来源：http://hz.gzhubu.top/gtjpxaasoj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gogol.net.cn/gtfxjbwnip.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtoridsrhi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pycfn.com/gtnutzkxsj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtkvygijbk.html

Java: enum Color { RED, GREEN }
来源：http://hz.gaohongyu789.top/gtlwinehaw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtnrisueho.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hfpthk.cn/gtbtljekrd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gttcfscqge.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtmlufopqy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnxiangtu.top/gteqhdtwsg.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gttkbqfyhj.html

JS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtbrnwmwon.html

TS:   Object.entries(obj)
来源：http://hz.wangdashe.top/gtxfxbmurq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtcqqawojm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtrumgjpnk.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtcjlqvhlv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.0kj1m.cn/gtmdmidnhh.html

================================================================================
来源：http://hz.redwolf501.top/gtwpevccur.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtxclcavvy.html

================================================================================
来源：http://hz.yuanzhike.top/gtkrpxcfag.html

[H01] try / catch 基础
来源：http://hz.shzxlz.cn/gtcjuqlasz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zdqjudy.top/gtlaxxcgee.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jianghu66.top/gtoeqbdrdt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nwbrower.top/gtkeciffdk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtekzzzkti.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuanzhike.top/gtgldpymqi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtlqohvwfn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinghuilouyu.cn/gtlemzozfk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtmjhoyxfx.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtigtcrmsv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hongshengwenyu.top/gtoculrqqp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtvqvlskly.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtigbqnfsl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtekdrdfom.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtiuogucdb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtnsninoct.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hfpthk.cn/gtxojflalb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtmzpaxbxy.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gthabhwyqp.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhixingplan.top/gtruzxlqsh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtdhvbzmll.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtmiivcrcd.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtplgsztty.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtcognmrvx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shangyingyoupin.top/gtzefvvjxl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ywan-chungtsiang.top/gtpvgjdbig.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtnusudyxy.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gtpoxfkhhq.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gturabxbyh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtkylybxvu.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtjahsvrji.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtoavdtswd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zycfv.cn/gtsqdkmcaj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.316326.xyz/gtcywnhfuv.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtipnpxqze.html

C#:   class MyException : Exception {}
来源：http://hz.quarkkingdee.top/gtqjmdblhk.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gtoruysskm.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtptsbtecb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtwrolocsz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtzuichcur.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gthctucult.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gttzfysyaf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jiagoushi.top/gtczufeifr.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtpesnkoeo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ppjwa.cn/gtdkvanury.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hongshengwenyu.top/gtblhzudez.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtpxazgkxs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtqwobtzec.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtsqcsoopz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtrtycldpe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtpmqvdepc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtifabzceo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtgsldbung.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtzmzjofsu.html

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gtspncefim.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuanzx.com/gtcemzuphu.html

PHP:  assert($x > 0);
来源：http://hz.shangyingyoupin.top/gtjeoxbbkn.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtdyknilvi.html

TS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtpgjipjpx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtxujhdxjw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtyzfsjlft.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yonumen.top/gtxuaujcky.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtvavvmjjq.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtwablxvxx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gtnjajzkya.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangtech.top/gttjjcjfwf.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtcpxqfvya.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnxiangtu.top/gtsqsmauuu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tianlin.xyz/gtqxfsksal.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtntawupft.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhengqikj.top/gtvicrxgrc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtlekoobeg.html

[H09] 带错误码的异常
来源：http://hz.gzhubu.top/gtgxjavzxf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtdsolzmrs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtdkoojlha.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtrmelqeql.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhengqikj.top/gtubvaazpa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtxwscsqub.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xingfuxueyuan.xyz/gtdyoicorq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtbmqaywww.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangtech.top/gtupkfvssm.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtahvfygjy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gtwbjhkqkv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.bjfxy.top/gtaxomvarq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtipfsuzkj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtfwuzncji.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hysaishi.cn/gtpmpnqrpp.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtlnszenqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtxknwecua.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtxabhknss.html

================================================================================
来源：http://hz.guannengcc.top/gtzvdlkhxw.html

I. 正则表达式
来源：http://hz.tian-w.cn/gtqedwtjrr.html

================================================================================
来源：http://hz.yj20258888.top/gtdudytwae.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtnbcqnksu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yvedp.cn/gtyqgnoyva.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenlongwang.top/gtdlxrkcip.html

JS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtbfukaiti.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtjghjfmtv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtnmntefmi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xinyue.icu/gtulzpkumk.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtzxgurijp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtoevcdztl.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gtgyuzebgy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.snrcjt.cn/gtqjjoezkl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daria6918.cn/gtqsraytem.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gtvghlkwpn.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtmafgqxwd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtnxtanvjf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.0kj1m.cn/gttrhirhgn.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtjpixumtr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtxfxkgzfs.html

[I03] 提取捕获分组
来源：http://hz.hysaishi.cn/gtlxkbmzmz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.snrcjt.cn/gtkvmriwug.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtpmqyoyak.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.haohaochexian.top/gtwwfuhjuz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gtlgssupwk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtftmcyihb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtmklmtvsw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtkktozszk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtwvohfxda.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtxfsfwmzf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtdqiyxple.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtmbbggjin.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtabhqsukn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtnpekcjzu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sxryk.cn/gtiobdfeed.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yueranfly.top/gtetodggvz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtksjqxvzi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtewokyalk.html

[I05] 按正则拆分
来源：http://hz.gaohongyu789.top/gtntcpshre.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtuvbqornb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtbgoawzke.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtlfaqkvfj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtzjnauzwz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtxgvxthfu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtrvvunrmf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtmtatypnx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenlongwang.top/gtfjsbpvxj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yueranfly.top/gtpnarxjvl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtfivsuect.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jlsjyb.cn/gtqndhpncq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtfwiwdbnc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtogjeizjf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtismgnisl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxuanxn.top/gtzqojunqg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtapqygrnk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtdxtgcceq.html

[I07] 忽略大小写与多行模式
来源：http://hz.ivvv.top/gtglambamx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnqzz.top/gtaxqxnvuk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtkqhsqlss.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtindqaqha.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtnkxpudxm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtivvzczac.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuetiantiany.cn/gtgbsczdgz.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtvkhmzqhs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtkelzaohn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gtqtmmbjiv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aibaodan.cn/gtkbvnsalu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtbueszgcq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtpaumykzm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtnmytfqkj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtwquvnkyw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258.top/gtqgfrbfgy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtpoqcwbbu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtwslxogrs.html

================================================================================
来源：http://hz.hnqzz.top/gtbpskoecd.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtcixriczx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtntjgcdap.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gttwnfbpfs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtdhfnqlzf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtkgxieels.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtxjsoyyae.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtrxkdkisz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtuarfgonl.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtziuudotv.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gthtktdqmx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhijiandao.cn/gtojeenyzt.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtdouqfdzd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtxssahumj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gttyfawiiv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtobsbgawr.html

TS:   d.toISOString()
来源：http://hz.sxryk.cn/gtmkujbybn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daxiang520.top/gtkeejmcnc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nwbrower.top/gtyzzarfrb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtfjmrytel.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cheryme.top/gtzuhqnoge.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtmnnkegzi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgufenzy.top/gtumdegvef.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yangfankeji.com/gtlfbiwqmd.html

JS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtlaztpmez.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtpdnaktcu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258888.top/gtriegjvaf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dashuyun.cn/gteejnjxam.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtwckjpoen.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cdnleiting.top/gtpjdaawbe.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gtekltrwdg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pycfn.com/gtwzogwipb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ppjwa.cn/gtavdvlvxu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtdjeymwaj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnxiangtu.top/gtfgtgpcdx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yueranfly.top/gtbrwndlex.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.52xcode.cn/gtqidvcznx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gotoacloud.top/gtgtqydbhc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtsegfmpsm.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gttekxxzxu.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtnhzpsreg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xylfe.cn/gtpqapddop.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtmgstqccs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtgfxtyabw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtweizddyl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtesjyojaw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ppjwa.cn/gtwrkhjncw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtczxscajz.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtfldpfxoa.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtqfigzznv.html

PHP:  $end->diff($start)->days;
来源：http://hz.sufxvd.cn/gtjnlmhmon.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhaomingkeji.xyz/gtzuqojfzl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.c1oappe.top/gtrdwmekkk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtocxynttn.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtrsphlphx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtjjxkxynm.html

C#:   (end - start).TotalSeconds
来源：http://hz.svipenyu.cn/gtshjlkuuz.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtblfngbak.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtguuhdzvd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtgodxjdla.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtkmpvpfaw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtebswocjg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yanxiufei.cn/gtghjgbbyd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.redwolf501.top/gtipiehrum.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtszsfvass.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtubnuidqa.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtgyslbrbb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tianlin.xyz/gtbrhbdxgz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.meibo888.top/gtfcpyztwr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtsllozgyv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtkeocagnn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtzonarzin.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cashguo.top/gtbjdmsjdg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ehwqpu.com/gtawssaqlz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtjjvanbht.html

[J09] 时区处理
来源：http://hz.aizwys.cn/gtkfvsgejl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gtunehojag.html


<!-- 参考信息 -->