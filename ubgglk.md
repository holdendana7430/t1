代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtspkvehcl.html

JS:   toString() { return this.name; }
来源：http://hz.fengsongda.top/gtknnkimgy.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtnvuqbwku.html

Java: @Override public String toString() { return name; }
来源：http://hz.yangfankeji.com/gtizwswrxw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtpyjipccn.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtaeaybpft.html

C#:   public override string ToString() => Name;
来源：http://hz.zhaomingkeji.xyz/gtlwdegsiw.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtxwcjivnt.html

Py:   isinstance(u, User)
来源：http://hz.gogol.net.cn/gtcpeipmul.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtxiaokpiy.html

JS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtqitzchou.html

TS:   u instanceof User
来源：http://hz.daxiang520.top/gttwhpplif.html

Java: u instanceof User
来源：http://hz.yvedp.cn/gtmtdxjymb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cashguo.top/gtpiipfixn.html

Ruby: u.is_a?(User)
来源：http://hz.hywenlv.cn/gtknovzclk.html

C#:   u is User
来源：http://hz.hammf.cn/gtjhgohyoe.html

[G14] 数据类 / record
来源：http://hz.shuidangran.top/gthqucfhvi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtksfolyby.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.haohaochexian.top/gtqidfshxd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtekwfjcxl.html

TS:   type User = { name: string; age: number };
来源：http://hz.jyoumei.cn/gtovgbkwpo.html

Java: record User(String name, int age) {}
来源：http://hz.yangfankeji.com/gtysvcvcmh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gtubgnxtmj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtsojpmqjd.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtaeqaivzi.html

[G15] 枚举
来源：http://hz.tian-w.cn/gtkwcnqyvs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtdcndswrs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtlzynhluu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jyoumei.cn/gttciiehtt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gthokxpqap.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtiycorouk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.kuanghao11.cn/gtipdajmtz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yvedp.cn/gtdivbrbbk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtjmhrmvqx.html

[G16] 对象转数组 / 字典
来源：http://hz.gotoacloud.top/gtcmralkxt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gtcgpsjwdq.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtqrdknyii.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtfnzvmkyy.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtiwjvyxob.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.kuanghao11.cn/gtrzdjjixy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtjruvflnn.html

Ruby: obj.instance_variables
来源：http://hz.havefunace.top/gtrwwxaxbv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daria6918.cn/gtkyktwpri.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkyijjmuk.html

H. 异常与错误处理
来源：http://hz.fengsongda.top/gtdhjiupgg.html

================================================================================
来源：http://hz.aibaodan.cn/gtiinbueun.html

[H01] try / catch 基础
来源：http://hz.xuetiantiany.cn/gtecvrprtn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtuiiuuxws.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtyptmfbgh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtgyqywipl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtadkkyfzh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gttwcvdoje.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fzhhl.top/gtqsdcprgp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtdsslzitf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shuidangran.top/gthjzrhfvw.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtgmkcyfqf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtyhjfuhgd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtjvcbfugl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gttdvjexvx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtaqukyxjq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtgxsjajlh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtxgdhrohq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gthnokrzkm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtidzflrih.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtdhsdrvyl.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtbngimbjn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtbioskjhb.html

JS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtgernxzvg.html

TS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtuvlajwbn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtewehyxob.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtgduwurao.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtfnxrhdmc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtmwrvqlkr.html

[H04] 自定义异常类型
来源：http://hz.birdmap.top/gtdllehnve.html

Py:   class MyError(Exception): pass
来源：http://hz.hnxiangtu.top/gtlnagpmai.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtewnawjfc.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtoqsrivns.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gthbcgfhyt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gtnqdjssrz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangdashe.top/gtjlhkmbdv.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtaanklwqg.html

C#:   class MyException : Exception {}
来源：http://hz.vqdsnc.cn/gtrdeqxolq.html

[H05] 捕获特定类型
来源：http://hz.quarkkingdee.top/gtwsepxfrk.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtvyplqmzr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenjidiqi.icu/gtjebeifuj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtwbfvxcph.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtcynyylqa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.316326.xyz/gtpskhrzth.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.mhx1999.top/gtpzjartob.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxuanxn.top/gtsqpyxthu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtwsmbddhi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gogol.net.cn/gththzzgje.html

Py:   value = d.get("k") or default
来源：http://hz.0kj1m.cn/gtjyetqlmx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtxdgtscza.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtwqmydvwr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtyzlmmaxp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gtygpctadt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.c1oappe.top/gtzxopehnr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gttmltbbkk.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtagxiuppn.html

[H07] 断言
来源：http://hz.zhijiandao.cn/gtiwcopycl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guowangkeji.top/gtlfiprakr.html

PHP:  assert($x > 0);
来源：http://hz.dianchejie.cn/gtyjuwmoug.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtyhrjryit.html

TS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtkhaebdgs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtpatdciuq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.redwolf501.top/gtryxrfsrw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydjk.org.cn/gtztwjqqpy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtubllfcxe.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtadypttxk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenzaomai.com/gtaclssnkf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.meibo888.top/gtcjtbehdx.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangkeji.top/gtkgnlmwbb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtntslpili.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gtehkwwtjj.html

Go:   err.Error()
来源：http://hz.nanxuanxn.top/gtaighngft.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtwsopjfhj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jyoumei.cn/gtrjqyfbae.html

[H09] 带错误码的异常
来源：http://hz.316326.xyz/gtlqcjypgq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigfzy.top/gtfjbhsiqo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtdcibneet.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtanqnnszu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gtmfuzstvm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.vqdsnc.cn/gtrbfvfwmc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtwxkntdmg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtbobfnvqq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cheryme.top/gtcfnoyeib.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtzzonsaua.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtlofbljtw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.birdmap.top/gthsovejts.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtdbitasch.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtllgoyoah.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.iojbl.cn/gtneaorggq.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtkfbfxlyn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtsdkafenm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhijiandao.cn/gthwqfguks.html

================================================================================
来源：http://hz.jinqigufen.top/gtpodnogxa.html

I. 正则表达式
来源：http://hz.sufxvd.cn/gttkllbfmc.html

================================================================================
来源：http://hz.ehwqpu.com/gtzzqworbo.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtguebennu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gthtmfylmw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guowangkeji.top/gtfvfiissq.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtumnjqapm.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtschxwqwh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtptpusaad.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtmepajwuf.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtmixeapvn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtxjqltxen.html

[I02] 提取所有匹配
来源：http://hz.hysaishi.cn/gtejukwrzs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yueranfly.top/gtfreemjfm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtrxoxurmf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xingfuxueyuan.xyz/gtmfkhzvqu.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtxbgsdzfc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtjbnnvjom.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtpruslqct.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtfpyhxock.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hywenlv.cn/gtxpfvavoc.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtnmzkfhyo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gogol.net.cn/gtengvccrz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuanzhike.top/gtscvlndqe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jyoumei.cn/gtgpumircm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xylfe.cn/gtaitblunk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258888.top/gttpbvlunr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtxsokvtam.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtsbnadrie.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtsbmlehzm.html

[I04] 正则替换
来源：http://hz.nanxinkj.top/gthhzabakj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhaomingkeji.xyz/gtqrhmbjbb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xylfe.cn/gttdetqior.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtkgxucodr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtcnzxrlwa.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.feifeiyinyue.top/gttacbtutt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtropuxrqx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtvpifxtvg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhiwuduotai.top/gtwdnzxmtg.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtglfyddjs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hywenlv.cn/gtjfadizdg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pengpengdd.cyou/gtnfhswrdi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtcebtvqxw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtsrghyzbh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yongpay.top/gtbnenyvgo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gtthxcvuke.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtzntvolzo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuetiantiany.cn/gtyckcqpja.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtkemrmwzc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtwaqyrddz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtdokrjepx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtokdzmrrk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtcoyewlwu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shangyingyoupin.top/gtiortudbt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jlsjyb.cn/gtcfsjivpb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenjidiqi.icu/gtgygfohdw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtqxzvwbwr.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtrdsaaexx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gtnruzltkp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.svipenyu.cn/gtqnkkxnwp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtbznjrixa.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtuosdqxfp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daria6918.cn/gtdysnasqk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.svipenyu.cn/gtanazylge.html

Ruby: s.scan(/error/i)
来源：http://hz.xziqi.cn/gtwjrljjkx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtplfjwrxw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258.top/gtsaveghrj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.feifeiyinyue.top/gtoegkjbfn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtzenioujd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtfiicdccp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtpbarauol.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtbhifybor.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuxming.cn/gtdvxmorus.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtdzjemlzq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtkpeoqdis.html

================================================================================
来源：http://hz.chenzaomai.com/gtglbrftxj.html

J. 日期与时间
来源：http://hz.kuanghao11.cn/gtilnglryp.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfyymjmpt.html

[J01] 获取当前时间
来源：http://hz.hammf.cn/gtksvosmdk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cucudq.cn/gtqykvvhbz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtqrfyycgp.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gtqhlwnkpp.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtzsprxlov.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtfgzylnxb.html

Go:   time.Now()
来源：http://hz.yueranfly.top/gtvghkfpfy.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtpodiywgw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtqvmqdnyl.html

[J02] 格式化输出
来源：http://hz.shangyingyoupin.top/gtdsdmpaey.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtuoqdffxg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtscopawwb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dashuyun.cn/gtugfajbii.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gthkqkhyua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtuslbtiiz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dashuyun.cn/gtvokkxeqi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtylxipyxd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhaomingkeji.xyz/gtxwwzpuge.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangtech.top/gttdffmvit.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhixingplan.top/gtsqlfavin.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtwfokjyvm.html

JS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtntycrjhl.html

TS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtaagmsbeh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtvdqnkvdi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daria6918.cn/gtlkoyudoe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtjobhuvfm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gthbmpydkd.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtziudqyyg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtqdhafbss.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtdcblquse.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtcymavnfu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangtech.top/gtsdtjjjvk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ywan-chungtsiang.top/gtzicfrnaw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtqscyysjw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtjwkxuskc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigfzy.top/gtyuetlafn.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gtzyzdojcx.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtdakhedhz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cucudq.cn/gtiajnebxq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtxwbflqvm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangtech.top/gtaabdbptz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuanzx.com/gtvvxhahmx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtbcjyhzmn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtndzygjag.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gtpziienrn.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtvjofgtvr.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtulrqicgf.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtozmmzcih.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aibaodan.cn/gtydxwreju.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtyopimtwd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtbhbcgjbg.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtqvxayrdx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuanzhike.top/gtyzdmfsfw.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gtheqsjqgp.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtneqnneml.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtbyymlzth.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangkeji.top/gtmgavhili.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gthikfmpcg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtnrfelagp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gthxakpvnz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tanke756.top/gtxpvslntl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gttktgidbk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtddwhdpkz.html

[J08] 提取年月日与星期
来源：http://hz.zycfv.cn/gtvvbedymo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xinyue.icu/gttfgpcuos.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtzkwtllav.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.redwolf501.top/gtwvudgtzg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtalzpgmul.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gtidaildpz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yanxiufei.cn/gtpehcfryn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtyvbglyjz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtwqvsougz.html

[J09] 时区处理
来源：http://hz.quarkkingdee.top/gtorkwnjgn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtcalqauei.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtywpkdoco.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtvoihcwub.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtjvzujivi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtkyddggci.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtrxswczdp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.redwolf501.top/gtimdcbrss.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhiwuduotai.top/gtypmegbhv.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtkqkiryny.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuetiantiany.cn/gtalofquwc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtwgbraibl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hfpthk.cn/gtzlkhupju.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gtguokqche.html


<!-- 参考信息 -->