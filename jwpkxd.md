代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.jqgufenzy.top/gtckchlnkz.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gthpsksegj.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtquyzuwcs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtvjywyhpb.html

Ruby: attr_accessor :name
来源：http://hz.fengsongda.top/gtjllbnxfw.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtgmlsefki.html

[G12] 对象转字符串
来源：http://hz.316326.xyz/gtgknqelss.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtegpjxmyd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtjgiywdqe.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtmfzdyfmt.html

TS:   toString(): string { return this.name; }
来源：http://hz.meibo888.top/gttwzyeesa.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtyoluzlds.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gtwludfdkg.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gtjhmjxrrx.html

C#:   public override string ToString() => Name;
来源：http://hz.ydjk.org.cn/gtsbrzqydb.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtjrnqytyp.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtflsmfnwf.html

PHP:  $u instanceof User
来源：http://hz.yj20258.top/gtlrjfwdjr.html

JS:   u instanceof User
来源：http://hz.52xcode.cn/gtpjotgdwj.html

TS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtqpztjire.html

Java: u instanceof User
来源：http://hz.0kj1m.cn/gtkwdahute.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtkjtvrzec.html

Ruby: u.is_a?(User)
来源：http://hz.nanxuanxn.top/gturpxwzha.html

C#:   u is User
来源：http://hz.pycfn.com/gtdheyeexr.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtxjrsxdnd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtaksmznky.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gtbbcxhura.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenlongwang.top/gtxzcivegs.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgufenzy.top/gtnojeeooa.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtcvjaxpmm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtzqmggosd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhengqikj.top/gtivwkztzi.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gtechlampa.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtvubcavar.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangkeji.top/gtsrygdnlk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gotoacloud.top/gtceqinfvx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gtzbybklms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtlpnbipjq.html

Java: enum Color { RED, GREEN }
来源：http://hz.jyoumei.cn/gtzjypodws.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtucaojbfe.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtmotvfjqm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtndimjkuu.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gtzrwhraud.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gttczkbnqb.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtmamgpyul.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtmhnlytkg.html

TS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtsyjqklpm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.snrcjt.cn/gtsaxjzlcx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258888.top/gtloeknzyf.html

Ruby: obj.instance_variables
来源：http://hz.cqqwz.cn/gtcgwuasel.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtyeojilcu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtjwodducu.html

H. 异常与错误处理
来源：http://hz.hfpthk.cn/gtluwmcadx.html

================================================================================
来源：http://hz.dashuyun.cn/gtpvimbnmg.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtktgdnqcl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jlsjyb.cn/gtloefwycr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangdashe.top/gtwyrizdxg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gtkgcumxor.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtjudhbbur.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sysykeji.top/gtzuvctvhg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jqgufenzy.top/gtzbkpuzur.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cucudq.cn/gtsrzydsme.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtoggxnjpm.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtcdaejdsr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtsvabdxjo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtijdrjtfn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtgkwjwnru.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtmfwxklrb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtfxhmbdbu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtihzuxrzl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtqvpbdiuz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gtkjdanesa.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtyxtmxvlk.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtjmauqmsr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtzmtngyip.html

JS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtzdcxpgxa.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtvennjury.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtitxcpmtv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gtzhyltdwm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtofifiumf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtecwkwvqf.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtenvowzov.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtyvdsxvpa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtrmxbbqzm.html

JS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gthwsdptsx.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtrdrgtaen.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtgtafoxqa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtjhowoxdf.html

Ruby: class MyError < StandardError; end
来源：http://hz.guowangkeji.top/gtqyjyeydc.html

C#:   class MyException : Exception {}
来源：http://hz.xuetiantiany.cn/gtqygbjhxz.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtiationpw.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtqfpqvwcx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtgsvkehec.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gttkaedynu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtrsznsmit.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtqvufqnmq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtnoxepkqg.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigfzy.top/gtktwnonyo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtpexejkcw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gtdisqiocg.html

Py:   value = d.get("k") or default
来源：http://hz.cashguo.top/gtexnmgfqm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gtfietllua.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtlxdjfohd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtzmvmdrbw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gaohongyu789.top/gtpaltyihe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.52xcode.cn/gtdmwpakyt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jlsjyb.cn/gtpstiebll.html

C#:   obj?.A?.B ?? default
来源：http://hz.gaohongyu789.top/gtbuezaqar.html

[H07] 断言
来源：http://hz.cheryme.top/gtqjbinzkf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtxlhvsxut.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtliaptmzx.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtvowraido.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtvtinvjqj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtseqykibd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.andypj.xyz/gtebprdgjm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtawzgszpq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gtubdhtctd.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtmztpsfyz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtoxlckfaj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydjk.org.cn/gtgbnwhkbs.html

JS:   e.message;  e.stack
来源：http://hz.xylfe.cn/gtsstmhphb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtloybhhcx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gtfthoipyy.html

Go:   err.Error()
来源：http://hz.yuxming.cn/gtahhuzfnq.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gteuhktqoq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxinkj.top/gtboyqmmzp.html

[H09] 带错误码的异常
来源：http://hz.jqgufenzy.top/gtkomupchc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtedornhvl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gttrzbtiev.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gttnoaoapi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gtwuebongl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtdaofylei.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtmvzsdwas.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.birdmap.top/gtgqqaonnd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jiagoushi.top/gtmkthxqcy.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtjblecfkm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtjbjkdqur.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gtjsnqgduh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtgeznjvuu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtqixrenzo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtfmoipeou.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtarcldmfx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhijiandao.cn/gtxsiagygc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.bjfxy.top/gtjyqvggzk.html

================================================================================
来源：http://hz.yj202588.top/gttggwdnau.html

I. 正则表达式
来源：http://hz.cheryme.top/gtaoshsoxv.html

================================================================================
来源：http://hz.jinqigfzy.top/gteaumykyq.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtcvcokbve.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtsuclybdj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydjk.org.cn/gtwtibcfmc.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtxxmdbjxg.html

TS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtbkgtrfca.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtuswudufh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gtevsrgxyn.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtxebfyyqg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ywan-chungtsiang.top/gtqepdlgyb.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtzymofegn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daria6918.cn/gtioxtwnjj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtyqvrsmyc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shangyingyoupin.top/gtdfudekjm.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtzspqlbnu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.smart0.xyz/gthhzohnwz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yueranfly.top/gtljdvhcvu.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangshuangyany.cn/gtvyphqaic.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.birdmap.top/gtxwgjaxqs.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gthbukrtny.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xingfuxueyuan.xyz/gtogagtpyn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ivvv.top/gtmkayezfb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.52xcode.cn/gtpwwwkxrp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gtrlkgyulb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtabjvtchi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuanzhike.top/gtrvjrtrxm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cheryme.top/gtjpuasfhc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtvxunacsi.html

[I04] 正则替换
来源：http://hz.xylfe.cn/gttdedggid.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.52xcode.cn/gtifwjcecw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.birdmap.top/gtaixligrl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtevdngoay.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtolvjujjj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtcxfoegej.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.feifeiyinyue.top/gtjhdvobhk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtzlaegbgi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtobdcpofe.html

[I05] 按正则拆分
来源：http://hz.jinqigufen.top/gthligqecf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtlshzxjwv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yueranfly.top/gtpceofjzp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtcioyxnjo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gthnpfxsrz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtbuzgerdx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtzdvereug.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtbfkgrsab.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.mhx1999.top/gtjhakexeb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gtcwmjrtpn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gttpcoegjg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtqoutvufb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gtmozeuida.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtzzqqvenp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gtyzocgypl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.quarkkingdee.top/gtqqjvicjt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtqstdxbwm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtxkibaffj.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtisdrjyvq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnxiangtu.top/gtgnefiytg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuanzhike.top/gtengblrte.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gtgchmifvc.html

TS:   /error/gim
来源：http://hz.fengsongda.top/gtgdbkzcos.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtlrprmdct.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtpsxrghyu.html

Ruby: s.scan(/error/i)
来源：http://hz.0kj1m.cn/gthdounesf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtvbxgaroi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yvedp.cn/gtwftvfmgh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gogol.net.cn/gttuyvqcou.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hammf.cn/gtpylegwbg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtdddhzftt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtmbcqwfzz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gtnnlonbrw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangtech.top/gtlvbwyjed.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtplmfcbvc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gtqvznmuky.html

================================================================================
来源：http://hz.yvedp.cn/gtbihklfww.html

J. 日期与时间
来源：http://hz.yj20258.top/gtjvcrxgij.html

================================================================================
来源：http://hz.hysaishi.cn/gthofnafwq.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtlaoqebnm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gtmswjogwr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtzetwyphz.html

JS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtnsynaxyu.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtoteoxvhj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ehwqpu.com/gteidnbhcs.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtiohpdyvu.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gtbetrxcdv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gttlqdexio.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gtxijanuud.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtxrmdncne.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtjoshfnuv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shzxlz.cn/gtfzkadrer.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtaotdxwvl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangtech.top/gtzfdznnsf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtosntzmjf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtllxpumss.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtqrweluuh.html

[J03] 字符串解析为日期
来源：http://hz.bjfxy.top/gtdvriybtz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yangfankeji.com/gtfndftdqa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.wangdashe.top/gtlsaszdwi.html

JS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtaovuomhq.html

TS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtasmjpgnm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtjrthhmye.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.haohaochexian.top/gtpwjwemrb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtxfvbgcxz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gtyqofyvzd.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtszjfxeyf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gtdkliasol.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.andypj.xyz/gtufsaebod.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtgrgfykyl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtgwdrcozb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zdqjudy.top/gtsmcfqhwi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.iojbl.cn/gtomrhsdxq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtujczscha.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtjhxbcuvu.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtdffwfclc.html

Py:   now + timedelta(days=7)
来源：http://hz.andypj.xyz/gttsjubgey.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.bjfxy.top/gtzznesnqx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtpneegvls.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtoojopyqr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangshuangyany.cn/gtzidrxjgq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gtgzoplxkr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtwbgtnhjz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuanzx.com/gtsngnufme.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtobtnhmpd.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtsrkksvhi.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxinkj.top/gtoyidcmlq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cdnleiting.top/gtmzevxdxr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.kuanghao11.cn/gtnufsavqg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtnojbbtia.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhijiandao.cn/gtpfdwwfqx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sxryk.cn/gtoryyuzmx.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtdctxibss.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangtech.top/gtggvslusd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtqjtrdrrj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.birdmap.top/gtikibxbbl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtjjyryetv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtbpeoahdv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtjycelrlo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtojcwmfcw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtpczdbyrq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtyywuxqls.html

[J08] 提取年月日与星期
来源：http://hz.yongpay.top/gtiwegyiha.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sweek.top/gtydnsmhft.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtsufceohg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zdqjudy.top/gtaxenclwm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.redwolf501.top/gtabyhyctv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hysaishi.cn/gtseqlkipn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gotoacloud.top/gtqotbbnec.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gtmjancmam.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtkcbpwybi.html

[J09] 时区处理
来源：http://hz.vqdsnc.cn/gtpuqbuvdn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuetiantiany.cn/gtzmristzo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtzxuujmpk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtytbglkpk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtdkvflwgr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtgqqvnqno.html


<!-- 参考信息 -->