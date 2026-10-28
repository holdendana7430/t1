代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.ywan-chungtsiang.top/gtldulkllx.html

C#:   public string Name { get; set; }
来源：http://hz.hammf.cn/gtetayumeo.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtbdnzsnca.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtpuhyyynu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtccqacixt.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtxllzedrf.html

TS:   toString(): string { return this.name; }
来源：http://hz.fengsongda.top/gtegnvsoqn.html

Java: @Override public String toString() { return name; }
来源：http://hz.9152youxi.cn/gttiggatyp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtnwpiszig.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gteqhchmbo.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtjdodkvna.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtvbdceupj.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtydzrzbbt.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtgwwdqttr.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtgfmdralv.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtssayskqf.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtqjfogbvn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gtzybybngd.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtakfvyuen.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtzlcbewoi.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtlhhcbmiy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gtupifwbmv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.316326.xyz/gtcmldiomw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtxlnmabzt.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtvrsdrfzg.html

Java: record User(String name, int age) {}
来源：http://hz.jqgufenzy.top/gtcvtckybi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtgndjllxl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gteitgphfr.html

C#:   record User(string Name, int Age);
来源：http://hz.sufxvd.cn/gtlaubyluf.html

[G15] 枚举
来源：http://hz.ppjwa.cn/gtreklsheu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtlzhlauwe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtkwfsjvky.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtnjffygdg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gttoyrofuf.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtpntedoul.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guowangkeji.top/gtjgtxkjuk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtthvcqboo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtgvlsasnh.html

[G16] 对象转数组 / 字典
来源：http://hz.dianchejie.cn/gtlfzftaqm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yangfankeji.com/gtxwrvibjb.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtenxnlqgg.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtsodiwkgb.html

TS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gttfsnrevo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gtswkjfdue.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtqnnucpkh.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtnwdcqwed.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.mhx1999.top/gtkpajfsyq.html

================================================================================
来源：http://hz.sxryk.cn/gtjwtejnqd.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gtholvnhdv.html

================================================================================
来源：http://hz.sufxvd.cn/gtpaelkohl.html

[H01] try / catch 基础
来源：http://hz.ydjk.org.cn/gtvzdukwyy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtcophokvy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigufen.top/gtcyfkdjgz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gttiebfmsj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtxxfnccwf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.mhx1999.top/gthjlruvkr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yvedp.cn/gtdcxjpaho.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtzuqopfzw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtxnpcehhr.html

[H02] finally / ensure 收尾
来源：http://hz.yvedp.cn/gtbiqsvfdh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtsppemqry.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gttzodcqlj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtgvmwmywv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtvxpugarr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtkdtgztwh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.0kj1m.cn/gturxforen.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gtowffhnli.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yanxiufei.cn/gtfnpidheo.html

[H03] 主动抛出异常
来源：http://hz.sysykeji.top/gtprurbzno.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigufen.top/gthymyjmdh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtpisgwxqv.html

JS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtqhlejzso.html

TS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtyjlqhcev.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtrbfgbant.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtcxrrudog.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangshuangyany.cn/gtebtegleo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtrhsvkbjc.html

[H04] 自定义异常类型
来源：http://hz.nanxuanxn.top/gtauiaaihh.html

Py:   class MyError(Exception): pass
来源：http://hz.sxryk.cn/gtcooxspay.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtqifokdrd.html

JS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtdnuaokkq.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtksrqafux.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gteqtemhhk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydzc1.top/gtciuczvsp.html

Ruby: class MyError < StandardError; end
来源：http://hz.jiagoushi.top/gtksvobcfd.html

C#:   class MyException : Exception {}
来源：http://hz.kuanghao11.cn/gtllknxskc.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gtvoavcxxg.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtrumcuqfp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hongshengwenyu.top/gtisjchtkl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtwmxaghps.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtgynyuvxl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuanzx.com/gtuswlwnsq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.meibo888.top/gtkeymztrc.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gtbjegcpba.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtsocmhgdp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtikuyhggr.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtswlsiulz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.9152youxi.cn/gtwllpxkzn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtaqjjvvvv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtmglwnqva.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgfzy.top/gtboihrrku.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.52xcode.cn/gtrbonljxl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtqtbcimzu.html

C#:   obj?.A?.B ?? default
来源：http://hz.fzhhl.top/gtegfgfyhk.html

[H07] 断言
来源：http://hz.hnxiangtu.top/gtngylrtgx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cucudq.cn/gtilcwkyee.html

PHP:  assert($x > 0);
来源：http://hz.mhx1999.top/gtikvvbvhb.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtpoogvugo.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtritbmksb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.svipenyu.cn/gtnlvndtmz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtyrblheit.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydzc1.top/gtfccmlaau.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtffhqsdyu.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtddojloom.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.snrcjt.cn/gtkwshwazs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shzxlz.cn/gtgsdieaei.html

JS:   e.message;  e.stack
来源：http://hz.ivvv.top/gtaciwccle.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gtggpugavu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gtysaqhmvt.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtmdecnyoa.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtqlvtlfiw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shangyingyoupin.top/gthtmsrwsg.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtwxldiohy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtgtbxrdlz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guowangkeji.top/gtkzpdrulp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtrbxxhiej.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhengqikj.top/gtghyikouc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtloqxfpyk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cucudq.cn/gtwmnxttkc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtdpetwddl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtyhorjpkk.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtcqsacyjn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gtizhppgnm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtxoaxdbtw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtogafffqm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtrnzccmid.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gthaivlppq.html

Go:   defer f.Close()
来源：http://hz.pycfn.com/gtfyljnrtg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenzaomai.com/gtqomtyzks.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gtubjehotq.html

================================================================================
来源：http://hz.hfpthk.cn/gthfkmrlti.html

I. 正则表达式
来源：http://hz.dashuyun.cn/gtyxovugap.html

================================================================================
来源：http://hz.aizwys.cn/gtfhtfseje.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtnrvietpi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.mhx1999.top/gtyzxnhrdy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtuuumjhaq.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gticdpyzzq.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gttxvcetkk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhengqikj.top/gtnxvoywul.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sufxvd.cn/gtrvlhiwll.html

Ruby: s.match?(/\d+/)
来源：http://hz.9152youxi.cn/gtvuozlylo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.iojbl.cn/gtapyiamxb.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gttkwguvej.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtprbgwvwq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangdashe.top/gtyreenifm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtvnvvgbze.html

TS:   s.match(/\d+/g)
来源：http://hz.redwolf501.top/gtaqltbcmd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jyoumei.cn/gtttqzbmvx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ehwqpu.com/gtnwfuznwy.html

Ruby: s.scan(/\d+/)
来源：http://hz.daxiang520.top/gtjlumkunm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhijiandao.cn/gtvhzsrctc.html

[I03] 提取捕获分组
来源：http://hz.gogol.net.cn/gtwwcimjmc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangshuangyany.cn/gtpfrwwyei.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtfuchumdb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yvedp.cn/gtdnafzkik.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtbdccdvgi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtuoxubrij.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtwrsbsqej.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtagcfldon.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yongpay.top/gtppvyntbx.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtoqvejxpn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtnycefrvl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtjkvscbos.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtubcssste.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtzpgijnep.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cdnleiting.top/gtygvptloy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cheryme.top/gtuzlwwylg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gtzapmglrb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtahltwwcs.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtjikiwbvg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daria6918.cn/gtssqrvozb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gtwdageffp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtgadtujiq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtlmmzkygp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fengsongda.top/gtvmiqeuej.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cdnleiting.top/gtwequahoa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtsrsqtlkz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtblpiands.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cucudq.cn/gtocvzxsea.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtlpybqquo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtadpwibco.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtypmevrhy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtqsxiiagp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zycfv.cn/gtzgxxqrsc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ydjk.org.cn/gtqhwdqhwc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtgqhtupnl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtbvkgvgep.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gtphxwusac.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtjtikeobf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jiagoushi.top/gtqxwndeip.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinghuilouyu.cn/gtjvdilksc.html

TS:   /error/gim
来源：http://hz.ppjwa.cn/gtqztrrips.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtwbvxnrni.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ybcxt.top/gtvdmaaotv.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258.top/gtmxmjmxzk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xylfe.cn/gtfetqeori.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtfrrfnunr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jiagoushi.top/gtyttafpka.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gtjqvnvpwx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtxgrsdqgz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtioaqbnox.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtbbztpnvu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtlsbmpdni.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258888.top/gtuyszodju.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydzc1.top/gtxmvdjrjv.html

================================================================================
来源：http://hz.zhixingplan.top/gtrudnkrhi.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtodulbbtf.html

================================================================================
来源：http://hz.nanxinkj.top/gtyjqbqqtn.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtmmavsdzu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtbbrhvgdk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtugpsxsgt.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtqgshqqng.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtkcmbvcdu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gtxtvrsczl.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtcunoyrmp.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtbhdhpene.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.bjfxy.top/gtsslwnpcj.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtaamwlqtu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtelqvkixa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtrmtvfvxi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtkstkncrd.html

TS:   d.toISOString()
来源：http://hz.daxiang520.top/gtevahfyry.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtvlkwnkcw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daxiang520.top/gtbagxsnfh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtwigkmkcd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gtnynvgvjs.html

[J03] 字符串解析为日期
来源：http://hz.ydjk.org.cn/gtnyhtkvim.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtjpvitmdn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xylfe.cn/gtwwmdnmlw.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtcpgxnxhc.html

TS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtbauluwwx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtbkpeubgp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtajqlhbeo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ivvv.top/gtgebrfgsy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhongyouzk.top/gtshucetvy.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gtmymwvptu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtskbktuif.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtwxxpylny.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtafqtekkm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtulikepqy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtzxkaqwal.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtgxbkrmnb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtxioleylo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuetiantiany.cn/gtxctahcad.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenzaomai.com/gtkvhvxeyo.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtjaqbemwh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cheryme.top/gtgpiklgjt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtinbaodrt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gttpppgxbt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tanke756.top/gtkrearbmd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtbgcimuxz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gtvwabfyfr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guowangkeji.top/gtwjlepfmk.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtownggnjs.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtpnkknqgm.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gtaaiwajmv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gtuzhgxeiy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtvfkaiziw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtixjagyqg.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gthbgsnfeb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtgzalxvse.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtsbbgzqrg.html

[J07] 比较两个日期
来源：http://hz.yuanzhike.top/gtdcceocou.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtiyasiumk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtgtlyqvyd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtkfqfeyvs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtlgbmjcrw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jlsjyb.cn/gtyfoufkjp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtytfekyyq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gttflpsjex.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtzeunkays.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtmwzopaeh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shuidangran.top/gtjbrdikpd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangkeji.top/gtkddnkken.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.mhx1999.top/gtbrpcscvn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cheryme.top/gthyetvfuh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtsbxwvrje.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xziqi.cn/gtxpgybzlq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gotoacloud.top/gtlybbwhsi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fengsongda.top/gtsqkdwwki.html

[J09] 时区处理
来源：http://hz.shanyushiyangkeji.top/gtehibrcxz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtlypbofkh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gzhubu.top/gtrrxlxsfm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtoghaymwx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gthoosfupz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hfpthk.cn/gtahyqkgnj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zdqjudy.top/gtvoifjpfh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtnpljgkbc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenzaomai.com/gtkyzirllh.html

[J10] 取今天 / 本月第一天
来源：http://hz.9152youxi.cn/gtpqkedlfo.html


<!-- 参考信息 -->