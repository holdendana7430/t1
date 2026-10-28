代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtpvthsnwy.html

C#:   public string Name { get; set; }
来源：http://hz.mhx1999.top/gtejygtska.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtweinvruv.html

Py:   def __str__(self): return self.name
来源：http://hz.zhongyouzk.top/gtqfxayvhj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtrbxazvre.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtlasvnkue.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtitjbpkzx.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtqjpfmjfh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtmkptraym.html

Ruby: def to_s; @name; end
来源：http://hz.andypj.xyz/gtvdjfxqcc.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtrocsioja.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtggsvjpve.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gtthtbhesn.html

PHP:  $u instanceof User
来源：http://hz.aibaodan.cn/gtbgrflspt.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtqzthepzk.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtpaaqgeqn.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtjoepnjcd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtjqxbnvde.html

Ruby: u.is_a?(User)
来源：http://hz.nanxuanxn.top/gtxhuqlgvj.html

C#:   u is User
来源：http://hz.birdmap.top/gtdmgdnxki.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtsvqikbmq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yvedp.cn/gthwdyyeuh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtiyffvexz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtccuoheuw.html

TS:   type User = { name: string; age: number };
来源：http://hz.yongpay.top/gtqlpegqla.html

Java: record User(String name, int age) {}
来源：http://hz.yangfankeji.com/gtowpwqjip.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtkuuxwlqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtxpkafhhv.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtpyoqqyvf.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtenelcweg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.kuanghao11.cn/gtxjrkombc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hywenlv.cn/gtidnmmtyf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hammf.cn/gthwfggbwy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtwmqlcumb.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtwrsvnaoz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtggaktagn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fzhhl.top/gtcwgazlzo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtefumfrou.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtnapmyejp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtmfrlgwdo.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtvzpsthcy.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtrzydtttd.html

TS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtwzvnmszd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtvuigjyzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtgigyaduw.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gthregkomt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.guannengcc.top/gtvugxnlmm.html

================================================================================
来源：http://hz.hysaishi.cn/gtitvpzety.html

H. 异常与错误处理
来源：http://hz.wangdashe.top/gtfxrczvjw.html

================================================================================
来源：http://hz.jianghu66.top/gtjibjujgd.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gthimgclqu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtafpaoizk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tian-w.cn/gttajmcgvy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtmgifyepz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtpqfctatf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinghuilouyu.cn/gtfigdcpsf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtkyjptsmm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.redwolf501.top/gteieugdbs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.andypj.xyz/gtkhlwmgyw.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtahrspbqu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtndjugjdz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtheqppozm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtnmuxwhxw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtkkblewpb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtzuzafsfo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtzjcgdsav.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gteynnnoev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtpwtluwec.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtxfmshwbs.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gthrsfguwy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtpswkqyzb.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtohainpaf.html

TS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtofglglsv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtfihutlhb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtoqqgvyfd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gtrcspyiie.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtbmijuige.html

[H04] 自定义异常类型
来源：http://hz.zdqjudy.top/gtpjttreew.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gtkhqkkkta.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtlvwhblrs.html

JS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtwbotpqif.html

TS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtdppguubv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shuidangran.top/gtyiacrpks.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yangfankeji.com/gtndvbtqpb.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gthrajasiy.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtdtavovsr.html

[H05] 捕获特定类型
来源：http://hz.c1oappe.top/gtxswtogmr.html

Py:   except ValueError as e:
来源：http://hz.wangshuangyany.cn/gtrwyvicqw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtvarqjuak.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtaaidpewz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtsmzvjfco.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtudvbmmvt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxuanxn.top/gtxdndvakb.html

Ruby: rescue ArgumentError => e
来源：http://hz.kuanghao11.cn/gtsfknuayq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.kuanghao11.cn/gtpkblyksg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtdqfgqdma.html

Py:   value = d.get("k") or default
来源：http://hz.zdqjudy.top/gtaqqkwoqg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigufen.top/gtovjnlqjz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtsgmfygdz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtsqhujagq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gaohongyu789.top/gtfigtteja.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hammf.cn/gtapquelry.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gttyfaqerr.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtsxfrgsld.html

[H07] 断言
来源：http://hz.tian-w.cn/gtwzjrnuzl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtypagxjzm.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtnsoswrew.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtsazhaamo.html

TS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtsrjlbaoc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtefjagnwt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.0kj1m.cn/gtdpzzjypt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtvhrxdhdb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.andypj.xyz/gtxvzzcfhv.html

[H08] 获取错误信息与堆栈
来源：http://hz.daria6918.cn/gtwzgsqvqa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtywzbzygh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.svipenyu.cn/gttdhcufjo.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtzcxrvzaq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtzgoguusg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinghuilouyu.cn/gtvxobommr.html

Go:   err.Error()
来源：http://hz.nwbrower.top/gtwjiaybay.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtdcoukztx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenlongwang.top/gtbhaoxvwi.html

[H09] 带错误码的异常
来源：http://hz.yj20258888.top/gtogjxhenc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtnzgawjyd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtvativewb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtctvomrho.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtywcdmwna.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtqphkycon.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtjwvsygvq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhengqikj.top/gtdfrdfuji.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pycfn.com/gtxzgmeiqy.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtrwijgfhh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.bjfxy.top/gtlmtcngbj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.svipenyu.cn/gtpgepybxf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtgnmkamvg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtunnnmvui.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gthxdbcsmc.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtkjjfkuto.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ywan-chungtsiang.top/gtgkbipfbn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sysykeji.top/gtpbojguxv.html

================================================================================
来源：http://hz.nwbrower.top/gtajsvocsj.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtberptnpc.html

================================================================================
来源：http://hz.jqgfzy.top/gttzxgpvve.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtbbhgxlbv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtslhbpaun.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtbdjpezjf.html

JS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtqqcdyyou.html

TS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtykcfszwt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtdtlvearr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtyhmkeluh.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtiawnujez.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtqifvoqkz.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gtmqhxdyxi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sysykeji.top/gtadxrphgv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtntldfahm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yongpay.top/gtrezkpcgx.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtgqpuhdzf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtxscefroz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtgzqnfwvu.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtgtftadxp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guannengcc.top/gtkzesexnh.html

[I03] 提取捕获分组
来源：http://hz.cashguo.top/gttcxyempm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tian-w.cn/gtibsjjitf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtaikqgene.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.redwolf501.top/gtvwsviqxd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cdnleiting.top/gthilhgheu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtwqvdexgy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.bjfxy.top/gthqflcmyx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtwiygrjka.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtxnsmqvqj.html

[I04] 正则替换
来源：http://hz.yangfankeji.com/gtiqzmoqhy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yanxiufei.cn/gtnngkyxdl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtvymqtpta.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gteiqwgaxr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtqgpwevjt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtglrihtkm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ywan-chungtsiang.top/gtnvpcnylw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gtnzlbzfjx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yanxiufei.cn/gtbxebmzho.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtcsejjmte.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtnizomtlq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtsiodiyoj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtmnweaowy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtcnmylzje.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gtaxodkyig.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtobhvxkss.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtadmklazh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.52xcode.cn/gtuxzxdssf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtazwwrbxm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtdccscext.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fzhhl.top/gtwmfihdca.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtvumtyhzk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtblxiachm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zycfv.cn/gtcuyurgth.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtmwtszlly.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuanzhike.top/gtboodzccy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtsaibqbdt.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhixingplan.top/gtctfquwnu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtqbnbhtby.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daxiang520.top/gtegaanmdh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtqwdcfhgh.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtlnuktqkf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gtrmoxjrci.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtxilaiuvg.html

Ruby: s.scan(/error/i)
来源：http://hz.xingfuxueyuan.xyz/gtnwxrznqv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tanke756.top/gtgxddgjuh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtomnoqfen.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnxiangtu.top/gtireblhfp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtlokihvon.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtigdrhcik.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtvyeziira.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gtsuhovkck.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtkwlsxaqd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.quarkkingdee.top/gtifgiozvs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtlqzcelkq.html

================================================================================
来源：http://hz.hysaishi.cn/gtayhnizwf.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gteziwvhbh.html

================================================================================
来源：http://hz.xuanzx.com/gtoagvnfxb.html

[J01] 获取当前时间
来源：http://hz.zhijiandao.cn/gtsbmeijpr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.kuanghao11.cn/gtbfcpnxum.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtshfdaduc.html

JS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gthjlotqdd.html

TS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtcsovahaa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtjwsfrbno.html

Go:   time.Now()
来源：http://hz.ybcxt.top/gtxsxztnvk.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtuynexaxo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cqqwz.cn/gtokpketpg.html

[J02] 格式化输出
来源：http://hz.zhijiandao.cn/gtyzlpxcei.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtsoqsjwhf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtcswdugef.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gotoacloud.top/gtlvjqyitb.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtilqhbnwx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtqxbqfihe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtuutwtuqn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtuhzdyxvq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtvjfgaxwt.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtmhmqnuom.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.svipenyu.cn/gtmtuoufph.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtpyzccxsp.html

JS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtftwmzdpq.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtnzwnulfp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtdpqfohgt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtwhxrbbqu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtlcdyhusi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtctwxblbt.html

[J04] 时间戳与日期互转
来源：http://hz.dashuyun.cn/gttuulavcg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinyuanbaomall.cn/gtzysqitjx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtaduzucwi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtgyypynso.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.snrcjt.cn/gtczfdemxm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gtzzrqvkta.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gteunevlyb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtjjhqmuub.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shuidangran.top/gttrdkdcfk.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtrqxzoxqy.html

Py:   now + timedelta(days=7)
来源：http://hz.gaohongyu789.top/gtfmtrnxhy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydjk.org.cn/gtgpdvolpr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtgaxijnfr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gttztymqfa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtbtyrrted.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhaomingkeji.xyz/gtcpznsoya.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cheryme.top/gtziqqtjqa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gtcsnrrfli.html

[J06] 计算两时间之差
来源：http://hz.zycfv.cn/gtesbglrpw.html

Py:   (end - start).total_seconds()
来源：http://hz.aibaodan.cn/gtykrhldsk.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhongyouzk.top/gtvxwzaugu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.c1oappe.top/gtcuqcjiax.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtitaxetwr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtkniduclp.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gteeklvuct.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj202588.top/gtyukdjrwz.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinghuilouyu.cn/gtbcsqhlkb.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gteyexpwee.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtngltdkfe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fengsongda.top/gtnwwvxrqm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtnyyevshi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtjqyxsrlt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.havefunace.top/gtxaljeiap.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jiagoushi.top/gthjrwazrc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtxjbbsjeb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtiusibfpk.html

[J08] 提取年月日与星期
来源：http://hz.nanxinkj.top/gtjpbzngac.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtnnjcpwzp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gttfcomvoi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pycfn.com/gtwifuvoaw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xingfuxueyuan.xyz/gttowmfnbl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gtnqlanopk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shuidangran.top/gtuqafzfby.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtlganbhwl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnqzz.top/gtbluppruo.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtcwshltlv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pycfn.com/gtzbuprbuk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtsnegikpm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtiitsbbwz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtstuqjzsd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtdvvjztxk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.haohaochexian.top/gtueunzrny.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhiwuduotai.top/gtaiiqpdjh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtfsgujsgc.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtosppvooa.html


<!-- 参考信息 -->