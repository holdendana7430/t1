代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cheryme.top/gtqqshzpkc.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtgwkysboy.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtuoucsxom.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gthmuyjwxy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtwgzvtlwa.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtlskrshis.html

C#:   public override string ToString() => Name;
来源：http://hz.chenzaomai.com/gttkatlsyl.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtwabossfs.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gthxbbymak.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtzzchfqvr.html

JS:   u instanceof User
来源：http://hz.aibaodan.cn/gtmtuirswi.html

TS:   u instanceof User
来源：http://hz.haohaochexian.top/gtganklfzc.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtmygebwsz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtievkgmkr.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtrnwskbbs.html

C#:   u is User
来源：http://hz.jinqigufen.top/gtbdvorlym.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtwlrsoldt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tanke756.top/gtioxqztnp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtztekjnbg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gtfnjudlsx.html

TS:   type User = { name: string; age: number };
来源：http://hz.jyoumei.cn/gtgthkazew.html

Java: record User(String name, int age) {}
来源：http://hz.sysykeji.top/gtuugudgne.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtcesvzmbe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gttcxgctvy.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gttwmqfdsk.html

[G15] 枚举
来源：http://hz.sysykeji.top/gtrkeuzqzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtofrqeefk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtztkbvjfm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtppewbryc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtiyfflski.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtbwpuxxgj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cheryme.top/gtsnbkezro.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gtwevcggeu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtcdlrhzez.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtxafqbpxd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.havefunace.top/gtgeafnqqk.html

PHP:  get_object_vars($obj);
来源：http://hz.316326.xyz/gtqdfgjjdv.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtuwgzujgp.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtmayoyfoh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gtjjuhcfwv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.0kj1m.cn/gtdkdiucbm.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtvxawemdr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuanzhike.top/gthjmyytsm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlpdsnxnp.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gttoepabnl.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvuyhfpgu.html

[H01] try / catch 基础
来源：http://hz.zhijiandao.cn/gtujlgolro.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhijiandao.cn/gthtcgorxy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.havefunace.top/gtozexxwhq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuxming.cn/gtmqntfnrx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtrfxbdgqk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xinyue.icu/gtwslcjijh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shangyingyoupin.top/gtlbtrvvrm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtvffubavo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtnkpleplh.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtjgspcstm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtmejsdflb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtszvplejk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtsiyzasbd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gttuiptqds.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtcqfokgji.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dianchejie.cn/gtllgcrshd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.svipenyu.cn/gtbymqaqay.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gtzessoysg.html

[H03] 主动抛出异常
来源：http://hz.yanxiufei.cn/gtzwvrufdr.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtobsqgjxz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtmctgdvey.html

JS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtgydxfujr.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtztdmydhh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtpgvtuoif.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtzubthsve.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtjgurjxgo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtzkdgwsyk.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtrvizntua.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtawwgsmqe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtnbaonnnc.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtfgomnriy.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtjrmlygcz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtnutttwlj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangdashe.top/gtuwhbwybv.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtyvursllz.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtyrgsmsbz.html

[H05] 捕获特定类型
来源：http://hz.yonumen.top/gtxcqgjqzw.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gttmtswdbl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtmhsnohar.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtshcnfbvx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtyggucfkz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daria6918.cn/gthwsroiut.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtrivvqfmf.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtagxxgeou.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtyhlirjrg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gttvzqmazk.html

Py:   value = d.get("k") or default
来源：http://hz.jqgfzy.top/gtfguwphlp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtitxowteh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtcmxtwvbz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtuyjcfcde.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shzxlz.cn/gtowlvjvcp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtnhkeyvie.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtjajyryag.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtxnmttein.html

[H07] 断言
来源：http://hz.zycfv.cn/gtbpxrnzdi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shangyingyoupin.top/gtpldwcrdy.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtvzpebfqp.html

JS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtbswlfdhn.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtlsonhlqz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtdenztaze.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gteaysoerj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinghuilouyu.cn/gtcyvqymyr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gtsiwvlmxq.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtxpkhusgo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtirwzvtmk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtvngcpowk.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gtqxhezjwk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hysaishi.cn/gtmcnahfyk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gteonzmpat.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtdshkjzsv.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gttidsecqa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.vqdsnc.cn/gtxynmhzzd.html

[H09] 带错误码的异常
来源：http://hz.zdqjudy.top/gtvzgxijkj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtvikgxmle.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtffqnaglw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guowangkeji.top/gtzrvtyhte.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sweek.top/gtmgdtebyy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtbhfoinls.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sweek.top/gtbforfren.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hysaishi.cn/gturpxlwvl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daxiang520.top/gttcmwnxzz.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtrgrypvbv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtiowseahq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtsbhmietl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtbyvgyhxn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtuhjpbiap.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtedvcsrgh.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gttiziilki.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtolhhfmys.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangdashe.top/gteuurdntu.html

================================================================================
来源：http://hz.zycfv.cn/gtpdkwgbww.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtkkblomeq.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzlhbggmw.html

[I01] 判断是否匹配
来源：http://hz.daria6918.cn/gtbrouigsn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtlhshkdav.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hongshengwenyu.top/gtznfxhwsn.html

JS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtudgwhhkx.html

TS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtzgmfnley.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtllazeoop.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtkafwrhky.html

Ruby: s.match?(/\d+/)
来源：http://hz.gzhubu.top/gtnobxlsga.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtbufgdqfa.html

[I02] 提取所有匹配
来源：http://hz.yuanzhike.top/gtfnhcdzum.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtmbvmchjn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtpnhsuddw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.andypj.xyz/gtssecvomo.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxuanxn.top/gtlcirqicr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gtdmmrjbej.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtsaftubvd.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtbktbkjnq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtrqebqeog.html

[I03] 提取捕获分组
来源：http://hz.jinyuanbaomall.cn/gtfhjsqdfy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtpiptpppv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.vqdsnc.cn/gtwfxfgoci.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtkjfegmdl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinyuanbaomall.cn/gtmjnwgwbb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtmbsrxxxk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtvaypynok.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtcevyvytv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yongpay.top/gtvvdqrutz.html

[I04] 正则替换
来源：http://hz.ppjwa.cn/gtbacmnfyo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtjprmkffi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtjrhdptza.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtyssuwnus.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtdeigelno.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gtiwbzxaot.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xingfuxueyuan.xyz/gthqvfwqfr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yueranfly.top/gtbgjjevdn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gtilwbhizw.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtjttdhdsl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nwbrower.top/gtgxbhyslz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtaedwrmom.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtwvxtfvhf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtrmjstafi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.andypj.xyz/gtaclbbmfk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtttmrtkia.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtekmyvort.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtwzkudpud.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtnqwqjjbl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtlcakbnjd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gttthinryo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtxcxbkzpp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtvoskarsk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtacefmtmn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtnwsjvoqr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtdqkodwfr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtxitjmwxt.html

[I07] 忽略大小写与多行模式
来源：http://hz.xylfe.cn/gtgomdpfhq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtkebaxkwp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtlhqjrwwk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.snrcjt.cn/gtqqkmcfch.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtpcbllctg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtxynfkvcw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gttkxsvhch.html

Ruby: s.scan(/error/i)
来源：http://hz.snrcjt.cn/gtdrgymhps.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jyoumei.cn/gtpmcemkwj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tanke756.top/gtalitvghg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hywenlv.cn/gthupoeelp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtxsuvjkjz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gteqwycjgf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtpivalxov.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aibaodan.cn/gtnwpmldxf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtwfkxlvte.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtyeplorhk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtlzgpffzb.html

================================================================================
来源：http://hz.ppjwa.cn/gttaveqcth.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtysjagqwn.html

================================================================================
来源：http://hz.yj20258.top/gtwavhefqd.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gtipajkhhx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cheryme.top/gtmngoryuy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtevqeogbt.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtljnvbvoc.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtrcryaukl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtyjqcddlf.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtdvcojptq.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtmzlauzfy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxinkj.top/gtsretuvom.html

[J02] 格式化输出
来源：http://hz.jlsjyb.cn/gtitzotggc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtfjmmczte.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gthtdjhkch.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gtdscsqfkd.html

TS:   d.toISOString()
来源：http://hz.xziqi.cn/gteplfzqjv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sweek.top/gtcjpbfgxa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtpailklne.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gttvzfuhnf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtgqezlwjd.html

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtykcrueqa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gtienmmxbg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gtycaifnhw.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtbvvukqpx.html

TS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtgbajkfma.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtzxdgbghp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtfjakvhap.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtwhfcsajj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fengsongda.top/gtfslwuapc.html

[J04] 时间戳与日期互转
来源：http://hz.feifeiyinyue.top/gtgrpwerbb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangtech.top/gtuyurkeyt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgufenzy.top/gtskgvodna.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtswdrnmlc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gtstjcqzax.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.bjfxy.top/gtktdwslid.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtzopksyvc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinghuilouyu.cn/gtubauqgch.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtmafgvmhr.html

[J05] 时间加减（加 7 天）
来源：http://hz.jyoumei.cn/gtpnqpbheg.html

Py:   now + timedelta(days=7)
来源：http://hz.xylfe.cn/gtxbagflny.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cucudq.cn/gthdpyactp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtadudvufs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gttavobjrk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tian-w.cn/gtvutwopqs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangdashe.top/gtcpncljqp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxuanxn.top/gtnbagrvse.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.smart0.xyz/gthkvsyvcv.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtdnymsuzb.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtqgcwabkt.html

PHP:  $end->diff($start)->days;
来源：http://hz.shzxlz.cn/gtunaezbop.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhongyouzk.top/gtqncftuoi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtpsyrogci.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydzc1.top/gtmunjqwhv.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangkeji.top/gtnwnkandc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhijiandao.cn/gtggleexos.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigufen.top/gtommsxaif.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangkeji.top/gtqnddtgpk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtsvlgegqt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ehwqpu.com/gtyfxstcmy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gtfucsesqi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtcncidzzn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fengsongda.top/gtaeecjzxe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.quarkkingdee.top/gtcerfwmlf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtuspykkhp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtwyqjunbx.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtowjozltm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtbipeavmm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cashguo.top/gtaxhhxhyz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtjcgjjzfz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gthlrgalvw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtrobmblkq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cashguo.top/gtzkwmfmhy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtuzmyueml.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jiagoushi.top/gtbfeuftty.html

[J09] 时区处理
来源：http://hz.mhx1999.top/gtlafuqjlb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zdqjudy.top/gttzbinujr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ywan-chungtsiang.top/gtefwhpscb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtpzerfvse.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtvzswctzi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.mhx1999.top/gtruporqti.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtmvrvatio.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtqgdvycad.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.vqdsnc.cn/gtivswaaad.html

[J10] 取今天 / 本月第一天
来源：http://hz.52xcode.cn/gtraeyxkps.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtnhjwzaqf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhiwuduotai.top/gtckltdzra.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtphkyjsnf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guannengcc.top/gtsrtyqoma.html


<!-- 参考信息 -->