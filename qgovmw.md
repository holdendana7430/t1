代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtenthejti.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gtbvhbwjfb.html

TS:   toString(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gthyfqxgha.html

Java: @Override public String toString() { return name; }
来源：http://hz.nwbrower.top/gtgjtvudwg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtsbmmmnbt.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtplwwylej.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtkscgxhyd.html

[G13] 判断对象类型
来源：http://hz.haohaochexian.top/gtzqcopcfx.html

Py:   isinstance(u, User)
来源：http://hz.0kj1m.cn/gtozeuatmf.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gtilfqhazm.html

JS:   u instanceof User
来源：http://hz.yj20258888.top/gtfxkkgwex.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtejmsjxvu.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtriiakrtr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gaohongyu789.top/gtbqlojecj.html

Ruby: u.is_a?(User)
来源：http://hz.fengsongda.top/gtzravdhjq.html

C#:   u is User
来源：http://hz.9152youxi.cn/gtausrissf.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtkfisrqzf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtktpdngve.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ppjwa.cn/gtntxxavbs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhaomingkeji.xyz/gtinbjtrjx.html

TS:   type User = { name: string; age: number };
来源：http://hz.gzhubu.top/gtcjawzpqj.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtwlearuah.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtemiewmcw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.redwolf501.top/gtkxtybeeq.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gtkhhvtnyn.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtgsyzbfae.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtjbyypbps.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gttfpwmxxp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtognxssxd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtygwippmw.html

Java: enum Color { RED, GREEN }
来源：http://hz.hammf.cn/gtpcmfgfvm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnxiangtu.top/gtpsynwujc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtvusxyfez.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gthotctabt.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gtftwvwvww.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.birdmap.top/gtolsdbxdo.html

PHP:  get_object_vars($obj);
来源：http://hz.aizwys.cn/gtbrueopgk.html

JS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtoduvlspl.html

TS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtfciyreow.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtthxlbvbw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtyistsnnf.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtmertvrwz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fengsongda.top/gtrtqzsaji.html

================================================================================
来源：http://hz.guannengcc.top/gtbovlxkuf.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtxhjtzpjt.html

================================================================================
来源：http://hz.yonumen.top/gtgmmciwuh.html

[H01] try / catch 基础
来源：http://hz.daxiang520.top/gtbumqykrf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxinkj.top/gttlfsuztq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtkiktulnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtfyckuhfw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhengqikj.top/gtcoksbnyo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.52xcode.cn/gtwwyqgqoy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtigbepyxr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shuidangran.top/gtwykuwyge.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtelyxopkn.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtrihvoemg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigufen.top/gtjssxvibc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtxskksztz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtnlqrqtby.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtjypyybjr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtuataqrrc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yvedp.cn/gtsnpkxiho.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.snrcjt.cn/gtbbyoiaqp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dianchejie.cn/gtucigbejv.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtgqyoujmh.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gtdsqrwslj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtqimxuwms.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtphshmamb.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtrvtrvkot.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gtziwocofy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtmllhemji.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xziqi.cn/gtqbdgrrqn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.havefunace.top/gtjuplcjmw.html

[H04] 自定义异常类型
来源：http://hz.yongpay.top/gtylslqpaj.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtybkmzcxl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtqpvsjyyf.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtnogibqlf.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtaezgeskd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtioaunrup.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtxacbtcun.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtwpjvextu.html

C#:   class MyException : Exception {}
来源：http://hz.xuanzx.com/gtmxyqwgzf.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gtdustazeb.html

Py:   except ValueError as e:
来源：http://hz.tian-w.cn/gtceboccyy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cheryme.top/gtlkvglniv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtfojcnxck.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtxhiumjxu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtbxbrwtsg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gtwnaiwubl.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangshuangyany.cn/gtglyhjmho.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtvwmlpbiq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gtsnndsubi.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtioddzqqv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtamfawwzt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtinjwsjsu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtfvuxwxha.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtwtfnpgro.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnqzz.top/gtdbqpwtsq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtnxjptxix.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtbillhxoi.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gtpzpbdqub.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daria6918.cn/gtbbcakaqp.html

PHP:  assert($x > 0);
来源：http://hz.jinqigfzy.top/gtnwwowjkm.html

JS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gteosqouzn.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtoxsjoqzn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtieiygoib.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtjmefnnro.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ybcxt.top/gthsbuptgj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtozvtmzih.html

[H08] 获取错误信息与堆栈
来源：http://hz.cucudq.cn/gtjgwwbnhd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zdqjudy.top/gtadklqtds.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cqqwz.cn/gtkydgkzfv.html

JS:   e.message;  e.stack
来源：http://hz.ppjwa.cn/gtvjdopcpu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cdnleiting.top/gtzvtejatg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.bjfxy.top/gtenynobje.html

Go:   err.Error()
来源：http://hz.snrcjt.cn/gtlrhrsoqq.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtbqxugnub.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtmfwuyjqh.html

[H09] 带错误码的异常
来源：http://hz.sweek.top/gtruobnpwo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tanke756.top/gtjwguvtxb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtnauhflop.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinyuanbaomall.cn/gtyngyggxq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtryolfkbd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtiiozimiw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtimgfttmq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtvlwfagqy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtugbpztei.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtqonymmwp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gttloiboqi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.0kj1m.cn/gtymkyvvhg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtruyebaug.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtskjxanzp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cheryme.top/gtzwsfhyrp.html

Go:   defer f.Close()
来源：http://hz.smart0.xyz/gtqycknhij.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtuduulrve.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtlmczraat.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpnsdmfpe.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtfvgkyicl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnhpejkml.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gthamjvyvi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtdjfpkuop.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtqoziwwzu.html

JS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtunwlkjdo.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtmyototco.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtoobwhxky.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinyuanbaomall.cn/gthqyckpuq.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gtqxlfpykp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daria6918.cn/gtfuytatpc.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtsslplkch.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yongpay.top/gtqisyoqvq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ybcxt.top/gtfjdygnlx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtlybgjabw.html

TS:   s.match(/\d+/g)
来源：http://hz.shzxlz.cn/gtfwdudyyw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhiwuduotai.top/gtjlwfoear.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxinkj.top/gtdyhmblpa.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtkybksbjf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pycfn.com/gtmfekbvyw.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtclcdjifu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtpuhyxiyy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtdkwlilce.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xingfuxueyuan.xyz/gtrdxcmjnh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gtwqggqbkl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yonumen.top/gtkryqlkkz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtanqqgihe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cdnleiting.top/gtklsllrdl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtoyipqwjy.html

[I04] 正则替换
来源：http://hz.yanxiufei.cn/gtyqococjh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtwhzuzjpo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gtnfqptypc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtcrwdcbnu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtajzkmbbk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuanzx.com/gtwxyrjbub.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zdqjudy.top/gtprhzoomz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258888.top/gtexbhjhfc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtndjzjxvq.html

[I05] 按正则拆分
来源：http://hz.cheryme.top/gtqshwjnzq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gtcecikbzt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yonumen.top/gtntwnieqq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtgkdlckhc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtvwgyijsz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hongshengwenyu.top/gtxcalxedh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.snrcjt.cn/gtbqbabrne.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtoqrlyklg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtyqryepbo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtsisllnrn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtffvvwqfm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.feifeiyinyue.top/gtaqipanps.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtpxjenxem.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtxdjiqvuq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tanke756.top/gthmajxdfd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cqqwz.cn/gtxouwokkv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258888.top/gteqowryon.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtdqqdqbkk.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtwlwrwlyn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtzbitiixv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gttysdcowu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtlfiaenpw.html

TS:   /error/gim
来源：http://hz.nanxuanxn.top/gtaesxfywo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtiscforyl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gtzzkwqctu.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtzobybtji.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtljgyyrzm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtqwqtzvvx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jiagoushi.top/gtnqdubekx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gtyfljibmq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtwomuwzxh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtgirceeqn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fzhhl.top/gtmutrlxjx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtprdgpcax.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtgkiyilqc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtfrshntyj.html

================================================================================
来源：http://hz.sysykeji.top/gtyyuzxthk.html

J. 日期与时间
来源：http://hz.meibo888.top/gtziijkyjj.html

================================================================================
来源：http://hz.daxiang520.top/gtafrklnid.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtebrlctpx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.0kj1m.cn/gtwuwxubod.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtrssqjuxx.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtpiwiajsj.html

TS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtwzyxcyrz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangshuangyany.cn/gtgegufdnj.html

Go:   time.Now()
来源：http://hz.hysaishi.cn/gtqddturvz.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gteyqukwtg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtoidiawau.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtphwhnfwx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtflyjyldi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gttgbxxwps.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ivvv.top/gtrdycenft.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtacnpysav.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhixingplan.top/gtkjhpgjbt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtynkrfiof.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtpvjgnpav.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtatlrhmfm.html

[J03] 字符串解析为日期
来源：http://hz.gzhubu.top/gtyptvqjyd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtiiqkfxvc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtgmhlxoyz.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gthvzzrjvj.html

TS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtqkblukft.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtklgosoul.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtzxshsxwi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtisogjpje.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtzlkxkcxc.html

[J04] 时间戳与日期互转
来源：http://hz.zhengqikj.top/gtqlvjqvxo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ybcxt.top/gtczpeboqo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gtdxcokmam.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guannengcc.top/gtdslduiqf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.snrcjt.cn/gtfszbqsxc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtislpfvlb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenjidiqi.icu/gtkyztyocv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtifsvzcyw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yvedp.cn/gtvvjifbnr.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtbybezmsx.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtjxrgdprz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtrjpfgnwu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtqiwbijbj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtthxzpzsp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgufenzy.top/gtstauiszj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtfvxngeqa.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtmqktudhx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.svipenyu.cn/gtfkgezupc.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gtfpqilolt.html

Py:   (end - start).total_seconds()
来源：http://hz.cqqwz.cn/gtahnostfh.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtnvcwsqzc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinyuanbaomall.cn/gtrykweafc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhiwuduotai.top/gtoqalfjzs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gttplqpina.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtohtcpebx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhijiandao.cn/gtsiugrprx.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtgbzndhfe.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtrilxoavw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtcjpcusrv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtdnbakitk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtpimycpna.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtqqtpnhlg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sufxvd.cn/gtmlnllfxw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtedjjnefi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtpggvsphv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtnwhvkofv.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtslqkcdhn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gticirersv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cashguo.top/gtemfchvvy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtdappabje.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ybcxt.top/gthqkaenyj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gtodrehnjt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtzsiflgwc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtepjhphfi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtvvfgbugn.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gtmhomtktq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtvusesyya.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fzhhl.top/gtrpsbmgdn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtiymxuius.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtwgzasxsr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gticeatbzr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtvpmfivwg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtxtwthtfi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhaomingkeji.xyz/gtwloidsfi.html

[J10] 取今天 / 本月第一天
来源：http://hz.cashguo.top/gtdemzmmvu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tanke756.top/gtfdbunvhp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gtytyhmils.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtkxbtrqbc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtozjofwxn.html


<!-- 参考信息 -->