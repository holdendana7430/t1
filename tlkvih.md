代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.xinyue.icu/gtceftwmye.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtapmxyxax.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtyarponwd.html

Py:   def __str__(self): return self.name
来源：http://hz.birdmap.top/gtdnoowilx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtepwrdlrw.html

JS:   toString() { return this.name; }
来源：http://hz.gotoacloud.top/gtxbahzmem.html

TS:   toString(): string { return this.name; }
来源：http://hz.ivvv.top/gttuplncpo.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtanfhmxdg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenlongwang.top/gthjgirnne.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtwzauqodq.html

C#:   public override string ToString() => Name;
来源：http://hz.pycfn.com/gtjpkbxjhy.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gtzigtmhhm.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtfgkeahez.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtcuucyljb.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtqbjpyies.html

TS:   u instanceof User
来源：http://hz.ehwqpu.com/gtiahxjrln.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtkhseboza.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtxzccwzuz.html

Ruby: u.is_a?(User)
来源：http://hz.chenzaomai.com/gtcbdwpdzn.html

C#:   u is User
来源：http://hz.zdqjudy.top/gtgsmgvtas.html

[G14] 数据类 / record
来源：http://hz.cheryme.top/gtwpjvtzdi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtitidhjju.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xziqi.cn/gtwgdyahzx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guannengcc.top/gtcauvzxox.html

TS:   type User = { name: string; age: number };
来源：http://hz.ehwqpu.com/gtljeuxmtx.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtgbqrgkgf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtogvlmcpj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtzxlccnrf.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtzixadjju.html

[G15] 枚举
来源：http://hz.cdnleiting.top/gttmwgkpfj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtfzfmftdd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtvtvxwrjy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtnrfzbmul.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtqqqwlsew.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgufenzy.top/gtqabwwwhk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydjk.org.cn/gtcdlrndqx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhixingplan.top/gtjbentdvz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtipeymttl.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtjiqbfbeh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydjk.org.cn/gtzonsogip.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gttdqlnvdk.html

JS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtlyfeputx.html

TS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gttocosndc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtsyckdowz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtoqngasyl.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gtrhnwapid.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cheryme.top/gtimdlswkc.html

================================================================================
来源：http://hz.zhixingplan.top/gtiawtqaww.html

H. 异常与错误处理
来源：http://hz.iojbl.cn/gtcruefehw.html

================================================================================
来源：http://hz.cucudq.cn/gtakruiogs.html

[H01] try / catch 基础
来源：http://hz.meibo888.top/gtinoejwhh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cheryme.top/gtjljaukva.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtinrlxvjx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gttkiticty.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhengqikj.top/gtcjskckev.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtjmxsqzvp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtzdvsgpun.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangshuangyany.cn/gtvyzdukce.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtctizsddr.html

[H02] finally / ensure 收尾
来源：http://hz.snrcjt.cn/gtvogunalz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.iojbl.cn/gthtzxknpy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gticfargtr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gttbcxrbjo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtvnaqollr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtygkszztm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gthjwtkrvm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gttgbaiqxa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtkvoansnf.html

[H03] 主动抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtpqczjmub.html

Py:   raise ValueError("错误信息")
来源：http://hz.haohaochexian.top/gtcurdfqym.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtkhgvrdfv.html

JS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtbjeuzvco.html

TS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtibrnhhox.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtlugcfnjf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gtfblicnww.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtkdhjqeuq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtjwgvbgzu.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtucphxmye.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxinkj.top/gtkjvilnnb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtsamvpjym.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtltzlbjbz.html

TS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtiddexwrr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.bjfxy.top/gtyoeqpaxr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cashguo.top/gtshjldmlp.html

Ruby: class MyError < StandardError; end
来源：http://hz.cdnleiting.top/gtopatbdxu.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtzgqtdsza.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gtdzmgbhrn.html

Py:   except ValueError as e:
来源：http://hz.xylfe.cn/gtvsoifviu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtqptsnkrp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtnfdhvifm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtenhavkva.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtpddqskii.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gtyqtphqxi.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtvxmhyrly.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydzc1.top/gtqceiyweb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gtefsipfpg.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gtrpxoftdv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtyjdhyhyo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtzwzbldbv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtnimbszox.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtghdngyqj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.bjfxy.top/gtybhceyly.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ybcxt.top/gtxrvnrnoh.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtjmtfqgyq.html

[H07] 断言
来源：http://hz.ivvv.top/gtdvshqeby.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtavavouvc.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtdslxktyt.html

JS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtdfpeoyho.html

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtidjovjnt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtkqxwmlrd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtiykuvsvb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fzhhl.top/gtbfebtrtt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhijiandao.cn/gtlgfzsagp.html

[H08] 获取错误信息与堆栈
来源：http://hz.sxryk.cn/gtmgqmznxw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtnygsucbd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daria6918.cn/gtdujlpglv.html

JS:   e.message;  e.stack
来源：http://hz.sysykeji.top/gtmlspmzvo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tian-w.cn/gtoldcxiof.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jianghu66.top/gtctkpawvt.html

Go:   err.Error()
来源：http://hz.guowangkeji.top/gtwhdzxrqy.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtqhcnzkhp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtprpwlqbh.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtkqelxakj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtospfwvcn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.redwolf501.top/gteaabyxls.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtvimwtgwt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtgflaksdm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daxiang520.top/gtetikxpja.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.vqdsnc.cn/gtmkskedat.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.redwolf501.top/gtrazdbhkr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuanzhike.top/gthoymhmgu.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtimalodyj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shzxlz.cn/gtqmyeenpc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.iojbl.cn/gtexkmyufc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtrpnvfkbd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtziqrbqow.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtestarwyh.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtfauymhra.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtubebfzce.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.feifeiyinyue.top/gtyrntqrbk.html

================================================================================
来源：http://hz.redwolf501.top/gtvzeiopvp.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtvfylnccj.html

================================================================================
来源：http://hz.yueranfly.top/gtooppnigb.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gtoeveosln.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtdoekkkot.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gtozsupwjw.html

JS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtnwcmwrnz.html

TS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtryxqyfdm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuanzhike.top/gthdifatco.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtxhokummu.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtclfsrzna.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daria6918.cn/gtaydlvlwg.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangtech.top/gtvoejloqq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtsttgfiyd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtqdwgahcs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtpjtvzgbm.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtokhuiamh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zdqjudy.top/gtqyceisdl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhengqikj.top/gteryyldfu.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtkcbdiijq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fzhhl.top/gtuplmennz.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gttdlwrchs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fzhhl.top/gtvhziwipm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtvkuikrui.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtttlhydyw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinghuilouyu.cn/gtaffndosg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhoulong.xyz/gthlvzjzol.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtrddadunk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhijiandao.cn/gtdfpwsffw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gtdsjtjccu.html

[I04] 正则替换
来源：http://hz.quarkkingdee.top/gtorjcnfob.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhijiandao.cn/gtzvrjjuag.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tanke756.top/gtucazsmsx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtitavpxvg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtxohsjqwr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtvkloxiyg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnqzz.top/gtssshuwag.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtlqfkccvm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtqqmlqtlo.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gtinxorpyk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtqgxcemhr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shuidangran.top/gtuuaxlokt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtoymnoxsq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtyyljkaxm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtavjaniyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gthqtvmbaz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtrnhtzzsd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtfuwbejex.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtvvlpetrz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtmzmlxxyo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gtqgmwawpa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtnpxyvtli.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtjgljegay.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtwzoyjprg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtmdxrluys.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shzxlz.cn/gtgcjuagyl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtlytjllmv.html

[I07] 忽略大小写与多行模式
来源：http://hz.9152youxi.cn/gtcxsnhjve.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gtrahfznxv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtkzmlcdtg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtfwofkicy.html

TS:   /error/gim
来源：http://hz.redwolf501.top/gtmjpkeudy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gthocsdoyk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gtsbcimdkq.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtswftclzj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtwzjnrwae.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ehwqpu.com/gtvbetfofa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.9152youxi.cn/gtnvqgwvmt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gthbqlbgte.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtkbqgsfic.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtaadpltwf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtbggnezkg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hongshengwenyu.top/gtwspheuvf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gttdppzwas.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtcqfnzkur.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxamcokbl.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtnfzuhskf.html

================================================================================
来源：http://hz.yvedp.cn/gtdttntfcn.html

[J01] 获取当前时间
来源：http://hz.xuetiantiany.cn/gtidmajteb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtwjwvyosy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtbcjzmlwb.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtgbjmkfet.html

TS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gtfuafsnjy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtiumgrrxm.html

Go:   time.Now()
来源：http://hz.tianlin.xyz/gtqvwlishe.html

Ruby: Time.now
来源：http://hz.tianlin.xyz/gtylzrmflp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtqungmwuh.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gthyltudwf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtzpbombxp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtlrcqumrm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fengsongda.top/gtarfdqpea.html

TS:   d.toISOString()
来源：http://hz.aizwys.cn/gtmzckwfkj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuanzhike.top/gtmjsjbkmg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtovhvrlam.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtywoaaclo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtrsdqzsyx.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtzwkegjok.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fengsongda.top/gtqguncgzz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtxlhchzcc.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtgtqcmlrw.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtjbyarpmp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtpmnoqnmb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cucudq.cn/gtlwrtlbvt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtznhgdhbw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnxiangtu.top/gtloytafdf.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtqpkcrlxf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gthmrgbxrf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gtskvsgmly.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ivvv.top/gtumsdsoqv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yangfankeji.com/gtbxdpjjnt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gtvozotsfa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtipkbqkcj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.mhx1999.top/gtfujmcpuw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gtndoxmwul.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtlmvvotnh.html

Py:   now + timedelta(days=7)
来源：http://hz.yangfankeji.com/gtqholrwjz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gttmvmyjot.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtaunjahpu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtlfjygdfa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtpssmblxs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtmmnezvkm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtrcehwpvu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gthpzckpmn.html

[J06] 计算两时间之差
来源：http://hz.cucudq.cn/gtqvnssitv.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtsuwdnrso.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtxhftowhx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtbcoexxhc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258.top/gtwjyzcert.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gaohongyu789.top/gtemobkxnr.html

Go:   end.Sub(start).Hours()
来源：http://hz.316326.xyz/gtqtwkiskr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cheryme.top/gtphdplphu.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtfwphljjc.html

[J07] 比较两个日期
来源：http://hz.jinqigufen.top/gtdcqpmlas.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtnycwqxqw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtzkeyftdg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gthnqrqrij.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtbjhrxqdz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtqtlbqxij.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtttuoslko.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtwdbfpfhk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtwypvflbu.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtkhmlbrcp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gthqdnvxap.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxuanxn.top/gttngiitsk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.redwolf501.top/gtrfbamkpo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtwcftfzbt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtpkqzpsbu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtflyhhlor.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtltafmmhg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dianchejie.cn/gtugkdkpea.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtldgahdcd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtakgpndbr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhijiandao.cn/gtegwxtulf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtuxkyqxyo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtyyoalwpr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtissahimu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtuapeqhna.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtpwthbdfs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gturlnbqge.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gtnvhsciry.html


<!-- 参考信息 -->