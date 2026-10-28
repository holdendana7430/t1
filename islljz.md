代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.guowangkeji.top/gtcqfenxxj.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtufqgghbg.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtynispgei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtvoxgwzch.html

Ruby: attr_accessor :name
来源：http://hz.xziqi.cn/gtoihbtdpo.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtkqizpnnd.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtaurptxlf.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gtojdaybdt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtbbqmeizs.html

JS:   toString() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtzhbwuwza.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtbgafjzec.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtkwsfulji.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tian-w.cn/gthkvzpjbk.html

Ruby: def to_s; @name; end
来源：http://hz.sxryk.cn/gtnghipfnq.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtnrukjwun.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gtqmapecmq.html

Py:   isinstance(u, User)
来源：http://hz.aibaodan.cn/gtjslvekph.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtibzvrmyl.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtwwdjvang.html

TS:   u instanceof User
来源：http://hz.jqgfzy.top/gtfbarofqa.html

Java: u instanceof User
来源：http://hz.svipenyu.cn/gtgikoijng.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigfzy.top/gtmqnxssih.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtgebkoerr.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtdxiidzqv.html

[G14] 数据类 / record
来源：http://hz.xziqi.cn/gtcubzqwex.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtvkwjnonb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tian-w.cn/gtjjlqoonq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.c1oappe.top/gttzsdzysn.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtvkenhedr.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtofhmvgfj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gtqgwwauvq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtlmqmxwus.html

C#:   record User(string Name, int Age);
来源：http://hz.ydjk.org.cn/gtjpjejocm.html

[G15] 枚举
来源：http://hz.yuanzhike.top/gtqnvsagws.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtgulrxsot.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenzaomai.com/gtnwutipos.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cqqwz.cn/gtvthufepr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtbqohpyam.html

Java: enum Color { RED, GREEN }
来源：http://hz.gzhubu.top/gteozzbaso.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtufuaqazv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhiwuduotai.top/gtzcanrnwz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtmcmxqdxo.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gtbxomfxzt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangtech.top/gtnkqzjard.html

PHP:  get_object_vars($obj);
来源：http://hz.hnxiangtu.top/gthhmwynvv.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtqaowfzyf.html

TS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtjiznugtt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.haohaochexian.top/gtspbymlsw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtkijorvuv.html

Ruby: obj.instance_variables
来源：http://hz.jqgfzy.top/gtfbzodekv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtgknexwfl.html

================================================================================
来源：http://hz.xylfe.cn/gtsmoprsxn.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gtrwwyyoyg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjimqvdhy.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtnibbsabi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgufenzy.top/gtzbtoohue.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtiugplsdr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtnvvjjghq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtjohjzikn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aibaodan.cn/gtbecpyobt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gtdrnytrkf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuanzhike.top/gtsjrvkwls.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtmxtfnbtq.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258.top/gtutruebgj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gteosduohm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtqogygyzd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtrdvffzhw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtpjcsldrq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtwdruitix.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.quarkkingdee.top/gtmyoytirb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj202588.top/gtnxhfxnrz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtkdxeurnv.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtjzojhnoo.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtouwwwlto.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gttznlikfw.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gthpmelxix.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtpemywbth.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtbtngjiby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgfzy.top/gtkhjygqrt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gtnsalitij.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtrqjtkmed.html

[H04] 自定义异常类型
来源：http://hz.zhongyouzk.top/gtngnvmdfz.html

Py:   class MyError(Exception): pass
来源：http://hz.zhoulong.xyz/gtqrhvmtty.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtrtihwfjn.html

JS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtltlgxfrt.html

TS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtujewocdb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtovjehwfc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigfzy.top/gtamtdhkdx.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtntdvtvzo.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtvursncej.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtuanbspvs.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtpinjcfyc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.haohaochexian.top/gtosqqhkpg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtcctnesdf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtyyfzmjai.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangtech.top/gtjeekdpai.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtvbgtpjvh.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtklzysyqg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dianchejie.cn/gtkymwtdlt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gtoscjvsyu.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtcewgbybf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sysykeji.top/gtvbzuugrh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtsjwjanvd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtyzyrtdyg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gogol.net.cn/gtkvowgont.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtngairhvs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnqzz.top/gtpxkyjmmj.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhoulong.xyz/gtlueblcik.html

[H07] 断言
来源：http://hz.iojbl.cn/gtcfppvorw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gtjzhyushj.html

PHP:  assert($x > 0);
来源：http://hz.hywenlv.cn/gtejczhwch.html

JS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gtvxduievz.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtzlhdvuyk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtejqkrjoo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sweek.top/gthnbonwvc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtigxqhadm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtwbzmpucn.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtfbwrxmcd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yonumen.top/gtenewkoqe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtvoduseao.html

JS:   e.message;  e.stack
来源：http://hz.kuanghao11.cn/gtqobaypaw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtkrmacgtx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258.top/gtioajhvrq.html

Go:   err.Error()
来源：http://hz.cheryme.top/gtkmjxrmrw.html

Ruby: e.message;  e.backtrace
来源：http://hz.cucudq.cn/gtznjpwfzg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gtxwwjyclm.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtpkhtmsxv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtudbokzfs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gttzesywfd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gtefsbjsko.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtdnjiaovt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.haohaochexian.top/gtpuyzwckr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jiagoushi.top/gtjgntstwe.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhengqikj.top/gtbakvatbc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daria6918.cn/gtlcwioqyd.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtpxfhohce.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtlujvwxnk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtcxfmzwul.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtcztsbrij.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtjltdaeae.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258.top/gtetxwxkqm.html

Go:   defer f.Close()
来源：http://hz.xuanzx.com/gtgqiemzeh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtcfghevbu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sxryk.cn/gtodlsdxfy.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttbnbrpmw.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtokzdfgbf.html

================================================================================
来源：http://hz.ivvv.top/gtzpqcziur.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtmmhwglyr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtfpbddaul.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtwkhoogni.html

JS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gthmtxmxbk.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtbvavcarp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yonumen.top/gtxocqygjl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gzhubu.top/gtsvhkbghb.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuanzhike.top/gtvnphtdru.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtoilcgphn.html

[I02] 提取所有匹配
来源：http://hz.cucudq.cn/gtequiptrm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtuhxcekpq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtdpdrssda.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtksivbcqq.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtbgadewqg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gttjsdetlx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtwrntnftg.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gtgksdpbod.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.feifeiyinyue.top/gtnpnrrlix.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtrbdhrtyk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.bjfxy.top/gtpzsmtawo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gthemkvzrz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zdqjudy.top/gtreknxwrg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtpanymrdi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtfqvpyfws.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtywfmbzwz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtuftjeaoz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258888.top/gtlstihicp.html

[I04] 正则替换
来源：http://hz.yvedp.cn/gtejibeiui.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ybcxt.top/gthkgufchi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtmehxqbet.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtihwkphbi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtxqalgctv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.kuanghao11.cn/gtuqgcyoco.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtdwiyiwjj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtkktrbujo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tanke756.top/gtjdufmzkm.html

[I05] 按正则拆分
来源：http://hz.yj20258.top/gtycpwipkp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gthomlujbn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fzhhl.top/gtsdfpztxd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtqzyfjjxb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtevrjwbbn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtefgevchy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtcuhgwgma.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtinirxzcn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydzc1.top/gtbwqaewll.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xinyue.icu/gtzifpofoe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtqczdyijx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhongyouzk.top/gtxkqwuggt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtudnjvxnc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtohadvftt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gtqjsehwur.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ydjk.org.cn/gtmmhnxrxc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj202588.top/gtzuyjgmca.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtgabpkuej.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydjk.org.cn/gtkoxlokwh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtwxkdspuz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.9152youxi.cn/gtpaugweqc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dianchejie.cn/gtgsqwgroz.html

TS:   /error/gim
来源：http://hz.jianghu66.top/gtiqkakmuc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gtiaxxigtp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gtxcuhqwrf.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtymrhqnhx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtbfyuczbx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtzzidhfvy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtontjyozv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtqfwuuhqi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtlroxnsfq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtofidoowl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtiazxwdsw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtgfnputmy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtlszcvhui.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtcmkwllcc.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgocwvhmd.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gtejhosven.html

================================================================================
来源：http://hz.yj202588.top/gthgcobmty.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtnhjsczwe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtpmgrsiyb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtawxdbmeu.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtzfkjgrgy.html

TS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtcjaaenma.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuanzhike.top/gtspvppgoo.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtkjtqgyww.html

Ruby: Time.now
来源：http://hz.chenzaomai.com/gtsqzpupup.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.meibo888.top/gtijthrtve.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtsbhgnhbh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtmjwwzkes.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtckbhcogr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtocfspuls.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtyhmfchbl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gthlumpnpk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtvzhyngzr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtjjavpdpe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gtzkrhvjlv.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtdpbewmmq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daria6918.cn/gtzftnuhsi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.smart0.xyz/gtpdmevbnz.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtoquhqhdd.html

TS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtmykofyib.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtvyiidfuc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtybtmnlmd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtofhzbagv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tian-w.cn/gtuyteaxsk.html

[J04] 时间戳与日期互转
来源：http://hz.52xcode.cn/gtoabzbuwb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtnhebluku.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.quarkkingdee.top/gtqhmjjmox.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtqfwaxdpd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gtdoreaoge.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtwozbotiu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtcqhpvavw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yongpay.top/gtlmlgnvhc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shangyingyoupin.top/gtndabvyvv.html

[J05] 时间加减（加 7 天）
来源：http://hz.cucudq.cn/gtklujaqry.html

Py:   now + timedelta(days=7)
来源：http://hz.hfpthk.cn/gtulrgrvog.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sxryk.cn/gtkgplcsxj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtwixlpvbv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtqhutpdua.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtxobeznca.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtppqlhbhn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hywenlv.cn/gtxyumwbnr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shuidangran.top/gtublgesxk.html

[J06] 计算两时间之差
来源：http://hz.mhx1999.top/gtboirlsfo.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtkjzvpbmw.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtocjpriiv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gtapcijvjv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xziqi.cn/gtvufdchdr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gttegbiicc.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtgbeqddbe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hammf.cn/gtskkxfmye.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtyatcmvru.html

[J07] 比较两个日期
来源：http://hz.nanxuanxn.top/gtfvovbfwd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtuyfdwxaw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gteqinhsry.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gttogcfgyk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtcmgufvxi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtpyylmpnw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtbtwmcusd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtpivkahdv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtmuoukrre.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gtlwkuzruz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yvedp.cn/gtshbxbaaj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtzvhbhsfq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnxiangtu.top/gtsnacdtwz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xziqi.cn/gtaxkwwstf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtbdvenccq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gtkbakrpbc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gtervkdmvs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtngslbiae.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtfmqefzvl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nwbrower.top/gtpoaucwxp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtzqfhzobo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtgaiprhyo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtaeckafqx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtatdteqqj.html


<!-- 参考信息 -->