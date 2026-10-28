代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtovlnomwh.html

JS:   toString() { return this.name; }
来源：http://hz.gogol.net.cn/gtouldiwub.html

TS:   toString(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtatflndeh.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtbdwlmbid.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gthgqjrvnw.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtpzpbffum.html

C#:   public override string ToString() => Name;
来源：http://hz.zycfv.cn/gtyxlhtwcq.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtzbljidbc.html

Py:   isinstance(u, User)
来源：http://hz.ybcxt.top/gtfuppnilz.html

PHP:  $u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtxrkybued.html

JS:   u instanceof User
来源：http://hz.cdnleiting.top/gtcbhzrtsv.html

TS:   u instanceof User
来源：http://hz.aibaodan.cn/gtrgiojwdd.html

Java: u instanceof User
来源：http://hz.zhijiandao.cn/gtzcczggdo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daxiang520.top/gtadfxfaqq.html

Ruby: u.is_a?(User)
来源：http://hz.fengsongda.top/gtvukkbzmy.html

C#:   u is User
来源：http://hz.quarkkingdee.top/gtlwjnsbxa.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gturriouaz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guannengcc.top/gtnqfigmxx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtgiaksgcx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtcudvzwbv.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuanzx.com/gthlvhwvrf.html

Java: record User(String name, int age) {}
来源：http://hz.sysykeji.top/gtzydxdyku.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258888.top/gtontjtbxy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtydypukxy.html

C#:   record User(string Name, int Age);
来源：http://hz.smart0.xyz/gtenvaxbkt.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtjfavxtgj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhaomingkeji.xyz/gtpuhpvcbl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xinyue.icu/gtkwuuqrwo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtarhlnugj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtdowvtbsm.html

Java: enum Color { RED, GREEN }
来源：http://hz.yvedp.cn/gtxrxwlvwf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuetiantiany.cn/gtatcafqxh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gtzpyvyysl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtshdmwfnc.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtpvfbnlek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtfsyupgup.html

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtderqezri.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtlbnytxsj.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtndvgpprd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gtjbxopynh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ywan-chungtsiang.top/gtszzfuvyr.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gtwxkidiyv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtmkmfzcvj.html

================================================================================
来源：http://hz.tianlin.xyz/gtzfiryckl.html

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtertymvxl.html

================================================================================
来源：http://hz.yvedp.cn/gthmulpdmn.html

[H01] try / catch 基础
来源：http://hz.zhixingplan.top/gtvvsokytn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ivvv.top/gtnotmunay.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtsmsnoypa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtaqiwucrs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cheryme.top/gtjkvtdavs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtjtfwoghf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtqvsrblmu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtxdlidbgw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhengqikj.top/gtyyuydsfe.html

[H02] finally / ensure 收尾
来源：http://hz.fengsongda.top/gtbhfqvlds.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.andypj.xyz/gtzrfaxnzz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtnpujoxgg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtqkxtgafy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtpqljxbzb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtmjfhnxbg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.feifeiyinyue.top/gtgpcxyaxx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtydwyvwlg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cdnleiting.top/gtlpnddvjf.html

[H03] 主动抛出异常
来源：http://hz.nanxinkj.top/gtwvqisbee.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gthejwnslh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtfsyexbap.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtaievmxjt.html

TS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtwendphdq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gterpoisle.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hongshengwenyu.top/gtkcflddgc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtahmecoaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtpdrubnkh.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtsszswgcj.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtjhgxemsq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtpsotfxsx.html

JS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtssnlobcx.html

TS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtolhdhbph.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtccqeerdt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.meibo888.top/gtkuemwtgb.html

Ruby: class MyError < StandardError; end
来源：http://hz.yanxiufei.cn/gtirjbkwof.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtfhdnmpft.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtlczclbww.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gtjsitlomx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sufxvd.cn/gtplraaxzs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtkxlvveuw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gttkdnnrxp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtjpabcfqg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gttorykcsh.html

Ruby: rescue ArgumentError => e
来源：http://hz.cashguo.top/gtcinrlmcq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtnlrdlclo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtuafhmhqo.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtthylftyg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ivvv.top/gtvrnvktot.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtfualdihx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gttwobonfp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gttbnpufpn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gtllbsmdtu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtafuzphnm.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtfjrjjuvn.html

[H07] 断言
来源：http://hz.nwbrower.top/gtkybvymjo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.vqdsnc.cn/gtbqgwcjdz.html

PHP:  assert($x > 0);
来源：http://hz.haohaochexian.top/gttlqaprxp.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtwqscpfkf.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtrwlwnjlo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ppjwa.cn/gtkacfixvf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuanzhike.top/gtakcpilmc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.bjfxy.top/gtpgdoyfsb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtqilnfykd.html

[H08] 获取错误信息与堆栈
来源：http://hz.sxryk.cn/gthltmbqhq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gtzmsqtrcm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtsiwkijvi.html

JS:   e.message;  e.stack
来源：http://hz.sweek.top/gteacymtiu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.meibo888.top/gtsqispmdy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pengpengdd.cyou/gtqjlquhna.html

Go:   err.Error()
来源：http://hz.zhongyouzk.top/gtuxeworlq.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtqbdnvqhf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtjledaezx.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtuwanjohw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtgqbqmqgg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtnkicwilf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtxwezuehv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tian-w.cn/gtqoniidzj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtuayjsxig.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhongyouzk.top/gtjtknlwxf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cqqwz.cn/gtuajoeznx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gtawejhgir.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtomakvogi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtnsrmbsjo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhixingplan.top/gtrxehoaaw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtegofiixy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtpwvqxwba.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shangyingyoupin.top/gtcqothfme.html

Go:   defer f.Close()
来源：http://hz.chenzaomai.com/gtubsxpfhe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gthjnnyjyr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtkdfvykhg.html

================================================================================
来源：http://hz.c1oappe.top/gtgvvwfcae.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtizcsizas.html

================================================================================
来源：http://hz.ehwqpu.com/gtyzrcparg.html

[I01] 判断是否匹配
来源：http://hz.daria6918.cn/gtzyhqrutq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtxsjbwcqp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtqbvdsiyf.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gteiqkqbnk.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gttnjkkdsi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gttvzovomy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenzaomai.com/gtnqshfxoh.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtfjaulybb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtccewnefv.html

[I02] 提取所有匹配
来源：http://hz.yueranfly.top/gtblyeldkb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gturxxtmwt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtghnpoady.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gtkntmwtgy.html

TS:   s.match(/\d+/g)
来源：http://hz.daria6918.cn/gtvlblkbws.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxuanxn.top/gtcqhxnarw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnqzz.top/gtyzizyitp.html

Ruby: s.scan(/\d+/)
来源：http://hz.sweek.top/gtowwdcuaq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gttehtskxc.html

[I03] 提取捕获分组
来源：http://hz.hysaishi.cn/gtbhzkjejr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtvwmmkyso.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gtnlslcrle.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenzaomai.com/gtojnxoewx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zdqjudy.top/gtikmdugbu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xinyue.icu/gthyckjsyn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigufen.top/gteyslcudj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gtjtgoxvdl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtysezniib.html

[I04] 正则替换
来源：http://hz.jinyuanbaomall.cn/gtvpliqnyz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nwbrower.top/gtnjcmggnh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtledlxnyg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtysfpqbzd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtcpfuxpls.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgfzy.top/gtajjngbul.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ehwqpu.com/gtimbhpeic.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gtjvdcbpgh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xylfe.cn/gtyahqrdht.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtqvtfiyem.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gtxfxrwjtn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cucudq.cn/gtrberasvi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtephxhpwq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gttbxokcug.html

Java: s.split("\\s*,\\s*")
来源：http://hz.feifeiyinyue.top/gtqpeqflmf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gtyorhcycp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtigczvtxx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gtireedyag.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtdkkdqcsw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtjgcdwzwe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtkzwrrdqm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtcwindoqf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtgvoucftq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtmmofgwve.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtdbwkgdjt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tianlin.xyz/gtxgwbzjbv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtebncslda.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258888.top/gtrtblwqqr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtuieirzrw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gtgcmzktjz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.vqdsnc.cn/gtentgyxez.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtcipvkdcx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xziqi.cn/gtgzgiovqv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gtgsblovjf.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gtavlzziku.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydzc1.top/gtxzxgijyg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jlsjyb.cn/gtyygkwypy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtnolxzcsi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtnjxvwnqa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtlcirmevy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtooykthls.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtsthnfvzh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuanzhike.top/gtbylzmofw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtctdwjvmt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtfhguwmjq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzgwvrxua.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtnelnqpxn.html

================================================================================
来源：http://hz.yj20258888.top/gtgnzzbpmi.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtgfeqcxni.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daria6918.cn/gtdayqdmev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtqdkjvoia.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtbsmnbwke.html

TS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtgisbmnaj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.kuanghao11.cn/gtcmeprhzk.html

Go:   time.Now()
来源：http://hz.yangfankeji.com/gtzggatemt.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtzmztfxdz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenzaomai.com/gtujcoddry.html

[J02] 格式化输出
来源：http://hz.ydjk.org.cn/gtsgirifea.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtdoraorto.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtbyuwkvot.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cashguo.top/gtcythfgpu.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtvmkcrrnr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gtjhbsvaky.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gthjojwncl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtrdrhfann.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.iojbl.cn/gtpvawrpzr.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtvnywdpeq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xziqi.cn/gtvblehoml.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yonumen.top/gtjyqznvqr.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtbpewmbru.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtewcukpja.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtkpthhpkq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtcpbkgddr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtrbpejgue.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhoulong.xyz/gtizhjasao.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtjuajgqut.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhijiandao.cn/gttlworyap.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinyuanbaomall.cn/gtwxtgonkx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtvffkicmy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtzxjlhpds.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gthlkllfnd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtjrjkbkiq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yueranfly.top/gtozejqpin.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gzhubu.top/gterluephn.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtoqajjetz.html

Py:   now + timedelta(days=7)
来源：http://hz.yueranfly.top/gtzrokzspc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zdqjudy.top/gtalxtxhzf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gttkapiztl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtvntqkchi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtrktlljkt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tanke756.top/gtwudqrpky.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtlslbweej.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtiovmpyro.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtjcphphmc.html

Py:   (end - start).total_seconds()
来源：http://hz.meibo888.top/gtwxzdeygi.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gttfjoasgm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtcjoejbcu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtoakuyetq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtxuzvmndb.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtepdsawia.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtfakcwbuz.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtnkmufqvi.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtrlrokxyl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gthyngrgnd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sxryk.cn/gtuswxcajg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtxcsjzfjz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtvbywvwol.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ybcxt.top/gtjhmmtvon.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtgpqiasoz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtgfqggjzl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtsjxticuu.html

[J08] 提取年月日与星期
来源：http://hz.yuanzhike.top/gtxuxdxhov.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.vqdsnc.cn/gtyhvsuari.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gtmifasflo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gtfkwambea.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtlfdzlufh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aizwys.cn/gtreoptfgt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hywenlv.cn/gtfibzxrcm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtxieonytl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.feifeiyinyue.top/gtbqktpkvo.html

[J09] 时区处理
来源：http://hz.sweek.top/gtbsxvlizj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtxyohllmh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gthjvnbpjq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtvvijtmcl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtwndqxfkh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daria6918.cn/gtiqggoiva.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tianlin.xyz/gtucvumqea.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtvuhzdalt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hongshengwenyu.top/gtjnhitmjl.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtdgqvamxg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtdcejbgsk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtstystaxv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj202588.top/gtgrhelyll.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cqqwz.cn/gtpimqyggj.html


<!-- 参考信息 -->