代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtflgilimt.html

JS:   toString() { return this.name; }
来源：http://hz.jiagoushi.top/gtrqxkuobp.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtgadeaqtn.html

Java: @Override public String toString() { return name; }
来源：http://hz.quarkkingdee.top/gtpxkjdgxf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtngkoqjwe.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangkeji.top/gtwgcrirrn.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtrmistguy.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtekfkfvvb.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtvlmuzcnb.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtuplnvnpe.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gtshopgvei.html

TS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtnrrebnni.html

Java: u instanceof User
来源：http://hz.c1oappe.top/gtibfnjjet.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtwztauudg.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtgvkrbpvt.html

C#:   u is User
来源：http://hz.xylfe.cn/gtopukbteb.html

[G14] 数据类 / record
来源：http://hz.jinqigfzy.top/gtfaxfmrsd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pycfn.com/gtdoevawzm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.svipenyu.cn/gtjscyahtx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtvllfnedu.html

TS:   type User = { name: string; age: number };
来源：http://hz.tian-w.cn/gtmkpivakp.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtogvokjth.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hongshengwenyu.top/gttzqpixee.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtbdsbeknr.html

C#:   record User(string Name, int Age);
来源：http://hz.hnqzz.top/gtwkunzlks.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtyqhkfpoq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gteiujhfua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtbgkmpqxh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtjenkktjg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtewfpzxyr.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gteiopuagx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtmcsnxolt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jlsjyb.cn/gttkohtwvh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtqosegcxo.html

[G16] 对象转数组 / 字典
来源：http://hz.ehwqpu.com/gtsksaibgd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtvdaspjsi.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtprnvtupl.html

JS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtpnbjrkdg.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtsgdzluto.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtccqilzyt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtdjzfeghy.html

Ruby: obj.instance_variables
来源：http://hz.zhijiandao.cn/gtmcdwnmmf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jlsjyb.cn/gtyruxcanf.html

================================================================================
来源：http://hz.guannengcc.top/gtjdbrrszt.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtmhscfxcq.html

================================================================================
来源：http://hz.fzhhl.top/gtyyagthyg.html

[H01] try / catch 基础
来源：http://hz.chenlongwang.top/gttouasjas.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shuidangran.top/gtiwceirmh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtiylrzlez.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gttvetsolg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtgzizokox.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.vqdsnc.cn/gtmsccffko.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtpcwiuqqe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cqqwz.cn/gtuzofthcz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.c1oappe.top/gtlviufsxj.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gthgtxoboo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtdyfirycl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtminzlsrv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gteabxxsdg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtadggywbn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gthwrezrpd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gtfnvebwxz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtcxvjeczy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.c1oappe.top/gtvhhgpnom.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtcuvpmtgz.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtystfjson.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtezueptuw.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtiqtwthxq.html

TS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtwffxhowj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtturohjds.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtdmsgbbbt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgufenzy.top/gtcomkyupp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtopjhaafr.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtwvzlvpjc.html

Py:   class MyError(Exception): pass
来源：http://hz.hysaishi.cn/gtwtcfyzui.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtuwtnffyv.html

JS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtcznnbdwj.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtecqrzztu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guannengcc.top/gtxlbvitya.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtyhanujwp.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtuguojfrc.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtacnnqmxd.html

[H05] 捕获特定类型
来源：http://hz.chenzaomai.com/gtduxyyfsv.html

Py:   except ValueError as e:
来源：http://hz.hywenlv.cn/gtgflbqnxb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tianlin.xyz/gtkcextinj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtkkdchloi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtupiayxjz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgfzy.top/gtgwwtcifw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuanzhike.top/gtinevltqp.html

Ruby: rescue ArgumentError => e
来源：http://hz.shangyingyoupin.top/gtaompdsko.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtkozwhrpd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtvdznmgjz.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gttrfhxqtk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuanzx.com/gtxznwxvcp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtuennnruk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtpztvklkq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.iojbl.cn/gtfjgblujq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtfjtieesd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gtkpyvkhcq.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gtkknszeso.html

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gtipdwgohz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shuidangran.top/gtmugmofqq.html

PHP:  assert($x > 0);
来源：http://hz.zycfv.cn/gtjdfyoeoo.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtkkeqhrol.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtsqqkfwbi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtqiuzixvt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gttmkprkkd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtfncggkax.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hfpthk.cn/gtckyahlqb.html

[H08] 获取错误信息与堆栈
来源：http://hz.pengpengdd.cyou/gtpfvvabva.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenzaomai.com/gtrdqdwfys.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtlusvtnqs.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtaiiqeoet.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtzfswhynh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangdashe.top/gtnkqsoknp.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gtovbvmosp.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhixingplan.top/gtxvnqiipi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtlourukzj.html

[H09] 带错误码的异常
来源：http://hz.wangshuangyany.cn/gtejcgerpb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtgebwurxl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtqitlquny.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gttcbcyciu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gtgkcwhsoo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gtgrugpznm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtynzlwnvu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtsmboxjax.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtddxrhatt.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gthjtrowfu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtpfpjaxst.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtjvkwgonf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtfcgphamh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtewiyxqxb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hfpthk.cn/gtomfpuwze.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtgtcdklss.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtdgmwhidg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtfpdacgye.html

================================================================================
来源：http://hz.yj202588.top/gturnbvrir.html

I. 正则表达式
来源：http://hz.tian-w.cn/gtcwscrgjj.html

================================================================================
来源：http://hz.jyoumei.cn/gtramjyatl.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gtdauutzbt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhengqikj.top/gtvrewnyii.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtrvbjndlv.html

JS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtdjhdzgmb.html

TS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gttrgrahct.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yanxiufei.cn/gtwfknduja.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ybcxt.top/gtuqmydfmd.html

Ruby: s.match?(/\d+/)
来源：http://hz.daria6918.cn/gtrcaksimq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtfulxnayu.html

[I02] 提取所有匹配
来源：http://hz.aibaodan.cn/gtgpykpynu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yongpay.top/gtavhrthsm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yonumen.top/gtjfikjxpq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gtcddtxuyz.html

TS:   s.match(/\d+/g)
来源：http://hz.hongshengwenyu.top/gtupsghewr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenlongwang.top/gtotmfpkns.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yueranfly.top/gtooixhivo.html

Ruby: s.scan(/\d+/)
来源：http://hz.quarkkingdee.top/gtfuqhcsux.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtrajbaskj.html

[I03] 提取捕获分组
来源：http://hz.sxryk.cn/gtuzlogatr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zdqjudy.top/gtdhohhlkm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtojlynbcq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtrxwsmvwi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cdnleiting.top/gtzynhgmau.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtjijxulfe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenzaomai.com/gtllvubprv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhijiandao.cn/gtunkqlfrq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gturosxycl.html

[I04] 正则替换
来源：http://hz.zhongyouzk.top/gtypwodyba.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zycfv.cn/gtsnatfrhz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtsylrfmvc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtwsrklcag.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtbdutjrmr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gtkuptbzon.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhengqikj.top/gtrwjcudia.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zycfv.cn/gtikvqmsys.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gtcdxhoudf.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtywthggqj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtrjjsrryp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtwzcdvomy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtcuushmbx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtxmzehrvh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangshuangyany.cn/gtbzqlswpf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.c1oappe.top/gtlqyilpav.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtnicyvhti.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gtxrhkozjr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtptxakfbl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtpieddhyf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.mhx1999.top/gtdhaipjkv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtahvfocey.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtjzobvztl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtkcdzrjbc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daxiang520.top/gtozxcdhwt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shuidangran.top/gtwowpeukb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtxywlliru.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtrhqbfkyx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigufen.top/gttslcakvw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuetiantiany.cn/gtumldtcwr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtxradzjuj.html

TS:   /error/gim
来源：http://hz.jinqigufen.top/gtmtgdkivo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtysxgbmbk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gtmlroynua.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtzpgqfssn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtcewqwsdl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aibaodan.cn/gteyxlbngx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shzxlz.cn/gthbwizqhp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtboymgzxf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtffbzrnbb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtoalmexod.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtsofakswg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jyoumei.cn/gtbonubdgp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhijiandao.cn/gtmfroizzl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.redwolf501.top/gtyhlslncj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqabetxum.html

J. 日期与时间
来源：http://hz.sysykeji.top/gtemussuoe.html

================================================================================
来源：http://hz.52xcode.cn/gtwxaydndd.html

[J01] 获取当前时间
来源：http://hz.ybcxt.top/gtaqwpqejl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.havefunace.top/gtaismjysz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtbwoxseuf.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtbcwxmadz.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtwvyjdbqd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtpdyqzmkw.html

Go:   time.Now()
来源：http://hz.yonumen.top/gtzyfumqep.html

Ruby: Time.now
来源：http://hz.tanke756.top/gtxoaksgug.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gotoacloud.top/gtvltjaset.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtkyhcjhhe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtprfxghte.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gttdazlwol.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtbkmnxpni.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtuayugxqy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gtgfwixdpo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gthxlmccef.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtvkfmzged.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yonumen.top/gtrcpkpyso.html

[J03] 字符串解析为日期
来源：http://hz.shzxlz.cn/gtxucexbiz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtupeokmkv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtkuzubovu.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtumgplglv.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtnhyshsjh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtixqhywzc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangdashe.top/gtpsbccemr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtyqyimsie.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtnmerakvo.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtntoffzff.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhoulong.xyz/gtkuomtygm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtwvelbfsl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yvedp.cn/gtcajrbtgy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aibaodan.cn/gtbgxnpyxm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yonumen.top/gtuqzfrvkw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258.top/gtxsgkoiyw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtpcwcalri.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtmpyqitqs.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhiwuduotai.top/gtqmetueqa.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtvanjusxp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtktrtynof.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtrhkwiqjm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gttouecess.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.birdmap.top/gtzvretbfv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtulewatgt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gtpknpbewc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtswffcqza.html

[J06] 计算两时间之差
来源：http://hz.hysaishi.cn/gtbqnvzjmi.html

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gtjnaanfbw.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtghbwlhmx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtzandaxog.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtujtenyoq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtlrmgksgl.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtytcunljm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtfaspiabv.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gtckziomlx.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtvjyhvqav.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtznyzhjfv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gaohongyu789.top/gtdgszrjqf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtqrtjwwbe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtjppsgsyd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtwlemunfb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gtpkhgcaum.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtqememyrf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtudxqjwnm.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtwnyijcux.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtaynhhkou.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtrpxjckfl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtljoagarw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtvperxtlw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhixingplan.top/gtmhyusjek.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ivvv.top/gtynnpqlvk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhongyouzk.top/gtlilcwpwc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hfpthk.cn/gtqswqrtae.html

[J09] 时区处理
来源：http://hz.xuanzx.com/gtnlpbcgzi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenjidiqi.icu/gtljtkrmlm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dashuyun.cn/gtwbhkzdym.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtlwtapytr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtagqszziy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cqqwz.cn/gtwinzvuky.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtobjweuiy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.quarkkingdee.top/gtprudsevd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hammf.cn/gthkfdpbkd.html

[J10] 取今天 / 本月第一天
来源：http://hz.52xcode.cn/gtxnjvvuha.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtzjxvontn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cqqwz.cn/gtdhezixjs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtavmihjkx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tian-w.cn/gtuerfdwvi.html


<!-- 参考信息 -->