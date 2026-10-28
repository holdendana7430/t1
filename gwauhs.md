代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtskvqcqnv.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtifzwbhwq.html

[G12] 对象转字符串
来源：http://hz.bjfxy.top/gtvfprxxao.html

Py:   def __str__(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtchnkwgkm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtbckmnuvx.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtivuralio.html

TS:   toString(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtahggruec.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtlpwjeqld.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtuwqqxonh.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtkrgvwojb.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtybrctymv.html

[G13] 判断对象类型
来源：http://hz.zdqjudy.top/gtepdpbtvs.html

Py:   isinstance(u, User)
来源：http://hz.hysaishi.cn/gtzoplykwb.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtlgimggpz.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtusajvamv.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gtdauralgr.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtlnbierhs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gttbnrjacd.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gttgrmunmh.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtbrerclus.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtibocaumz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.52xcode.cn/gtvbbcycbi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtshoadlik.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.kuanghao11.cn/gtfenvrnca.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtqwcydhgx.html

Java: record User(String name, int age) {}
来源：http://hz.guowangkeji.top/gtvonjezfj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.c1oappe.top/gtyhuepqwg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sxryk.cn/gtjjekwoks.html

C#:   record User(string Name, int Age);
来源：http://hz.chenjidiqi.icu/gthhruwtcu.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtarexmdnk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtehpguckp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgufenzy.top/gtfmbyvcgc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtvpbfbeye.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtkspvpoty.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydjk.org.cn/gtunnkfshy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.iojbl.cn/gtzfnmkjho.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtawqssala.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtcfwfuikw.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtzhzmvend.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ybcxt.top/gtnzkqazbw.html

PHP:  get_object_vars($obj);
来源：http://hz.yonumen.top/gtoiepwzkr.html

JS:   Object.entries(obj)
来源：http://hz.hnqzz.top/gtnerxybrj.html

TS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtpygyxsjv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtdzgqcjxq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.birdmap.top/gtmctbnwdr.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtzrathpub.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtmeuuonpe.html

================================================================================
来源：http://hz.hfpthk.cn/gtthaellzj.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtffermztq.html

================================================================================
来源：http://hz.ehwqpu.com/gtvpdiazpw.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtadtvcgdp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nwbrower.top/gtolnkvevf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sufxvd.cn/gtlrvwihzz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtaeoygwum.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhixingplan.top/gthjdkfkpu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtoxsottks.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtczrvfulo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tianlin.xyz/gtkwwfeydx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.birdmap.top/gtnrzbmerj.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtruvjvhnw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtcdqyoklb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtmbodxmts.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtlepsizen.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtxxshivga.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtcennzqxq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenzaomai.com/gtuhdgviyv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtnsutekmm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtzihxfuog.html

[H03] 主动抛出异常
来源：http://hz.jinqigfzy.top/gtbokkunre.html

Py:   raise ValueError("错误信息")
来源：http://hz.jiagoushi.top/gttkxjxeev.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtxdmpzlra.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtyyrmfqdr.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtyxkrgcxx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtabdaontq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gtsaphnaau.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtcmplxxzk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtlbyhjwnk.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gtfuwhcxip.html

Py:   class MyError(Exception): pass
来源：http://hz.shzxlz.cn/gttknoshmm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtejistwcn.html

JS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gtrqufsaxa.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtumlbsfhz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtumdxbnrr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtwjlrcjnr.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhijiandao.cn/gtbqwejilv.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtjpcstzqd.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtiijqoxkd.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtfoknrssf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhaomingkeji.xyz/gtlzlhvhpw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtsocgawfw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtvgylrxip.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtexcrbisj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.meibo888.top/gtipyijyxv.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxuanxn.top/gtsxzclptl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtmozpqhhr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.bjfxy.top/gtxshhkwxa.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtxtastszw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daria6918.cn/gtjmwhqigr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtgsdfsrdx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtjlvrfjet.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtroilxxdm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenjidiqi.icu/gtlupbslbj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtogmpdsve.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gtvuzczrye.html

[H07] 断言
来源：http://hz.tanke756.top/gtrqlfwnkw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guowangkeji.top/gtlcvnmhbz.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtgzhcaxbh.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtzrpfpzce.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtbtpievge.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gtzuxysvzf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gthdhhbjok.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xinyue.icu/gtmdvtmqyb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gtcgzfkwjl.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtvegbrnbz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtclcydckd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gttllvgjiu.html

JS:   e.message;  e.stack
来源：http://hz.yuxming.cn/gtxnarvqfq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtqnhylcck.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtyqsxecgv.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtomdvlnay.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtlbovfgiy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gtgevztcan.html

[H09] 带错误码的异常
来源：http://hz.xziqi.cn/gtvdzgtqpl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gtnsewjkpc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guowangkeji.top/gtnyksufdd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtmjthwqqe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtuipohzvb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.meibo888.top/gtyypooceu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtpgicfesn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guowangkeji.top/gtgogtxsup.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtqjhwpyda.html

[H10] 资源自动释放
来源：http://hz.jlsjyb.cn/gtlcnsbkjt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.meibo888.top/gtvqfyxhse.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtaljsfqbt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtgzdvpofg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtgdcsndpw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangtech.top/gtkffjubzx.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtnhgnkqnt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtzejdufdc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenlongwang.top/gtwymymkck.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtohivvvel.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtfnxmvtlk.html

================================================================================
来源：http://hz.sxryk.cn/gtoivzqnef.html

[I01] 判断是否匹配
来源：http://hz.jqgufenzy.top/gtrwuqzhqy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtggzszvly.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhaomingkeji.xyz/gtmyxuyzoh.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtjxpbwyxk.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtugwiyrhp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gttllgqbys.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.redwolf501.top/gtthusffeq.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtpdpwdjts.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtehmhbhcb.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtpwiyipqu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhengqikj.top/gtxfsmamhg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.vqdsnc.cn/gtghonjqjj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.c1oappe.top/gtyplvpnyw.html

TS:   s.match(/\d+/g)
来源：http://hz.yonumen.top/gtqsfikljf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtdcbyzzyr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.smart0.xyz/gtjzueqgqs.html

Ruby: s.scan(/\d+/)
来源：http://hz.gotoacloud.top/gtrqjhqucn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtlwqxjbpw.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gtvfvkuycm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.feifeiyinyue.top/gtsmuymviy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtovwxsobd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgufenzy.top/gtepyxtolk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgfzy.top/gtqjtgbefb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ivvv.top/gtoendcufq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtfmchbzxd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtuwpfgbic.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gtqcrmqnkk.html

[I04] 正则替换
来源：http://hz.316326.xyz/gtanigfocv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.birdmap.top/gtpwyizhoq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtwjkcaikv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtmualarlo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtdgyqghdu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtjokgukux.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jyoumei.cn/gtmslabhpe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtvadgznjb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtxlwwepqu.html

[I05] 按正则拆分
来源：http://hz.ivvv.top/gtuxfjwdow.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gtjliwlewm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gtzqibqmxq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtqatrslpf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtvdaphgaf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangtech.top/gttblrkvtx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tanke756.top/gtzmukipal.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtnlfiybaz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.c1oappe.top/gtcwilwyyr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtjpeigaaf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtpczdzbsc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.haohaochexian.top/gtwsklymrr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtlldxhptf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtvpthdqrl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtoghjpjib.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gttrvhbwpq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gteerixtfa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gthebaqnpd.html

[I07] 忽略大小写与多行模式
来源：http://hz.birdmap.top/gtnlcrzsdr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.birdmap.top/gtpbxsbusa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtuzppkaxv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ehwqpu.com/gtcwyfsndk.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtwwdxwjoa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sxryk.cn/gtkjxdwvip.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtfpzpnbcs.html

Ruby: s.scan(/error/i)
来源：http://hz.cashguo.top/gtawnbsdwd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangshuangyany.cn/gttukiljug.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtljwzcggh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtuxobjqwh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtlofwwlpc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtavehcqjb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtuduvphxk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtaitxfqel.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtrtddihon.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhijiandao.cn/gtoqbmvzqx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ybcxt.top/gtjluvfxeu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtyzhptmhm.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtouyduumz.html

================================================================================
来源：http://hz.zhongyouzk.top/gttiobblnr.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gtbcavjgxa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtiefqzzua.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtnqegsofk.html

JS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtfpsdizwh.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtosgcgijp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtaybzlwnh.html

Go:   time.Now()
来源：http://hz.ydjk.org.cn/gtxjqzqvzt.html

Ruby: Time.now
来源：http://hz.xuanzx.com/gtabdmipej.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtdmlgooki.html

[J02] 格式化输出
来源：http://hz.hfpthk.cn/gtxabhwxmj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtswemjjqc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtikcmsabi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gttnbyqvty.html

TS:   d.toISOString()
来源：http://hz.nanxinkj.top/gtvhmisawz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtoctrqryn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenlongwang.top/gtogdfkshl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtdznoubsb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.iojbl.cn/gtmqhtpubd.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtzngqivdq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gttgmrxgka.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gtvnliuhmq.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtdnsnapkc.html

TS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtnfypmlnn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtcfahdnhj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtyjjhghby.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtfwhxefpn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtqeqsdisb.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtlqxqlaln.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hywenlv.cn/gttytvndna.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtphrxblvf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgfzy.top/gthtwavvfv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtjwoqmdtw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yonumen.top/gtnmbvtwxd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cqqwz.cn/gtcpjfdacs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ybcxt.top/gttmnjwwvl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtkkvybnmk.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gtuowambxe.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtstezmhoh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dashuyun.cn/gtbszpoltx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtyzecufwj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtblatunsb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnxiangtu.top/gtdsjhmjsy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtzbtwfprr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ehwqpu.com/gtbpybhuja.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtccxlmygo.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangtech.top/gtntkdycvx.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtpbrfwzef.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtemagrfrv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtiojstoke.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuanzhike.top/gtfkgerxla.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtnuapyjaw.html

Go:   end.Sub(start).Hours()
来源：http://hz.ywan-chungtsiang.top/gttgoprktj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gtasryqtdx.html

C#:   (end - start).TotalSeconds
来源：http://hz.pengpengdd.cyou/gtvtlznnct.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtbqgptbme.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtgfjznayy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ivvv.top/gtyvfnyggq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtabxvnsjg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtlthcyvnr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtuhlvcxkx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuetiantiany.cn/gthmrdnyan.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtzyctfeek.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtkjamyluy.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtgjefgtop.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtyexxllak.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shangyingyoupin.top/gtgelszbwm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sysykeji.top/gtnqafuuna.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hysaishi.cn/gtvixyykfe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtwoclfjkj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shangyingyoupin.top/gtgfddelwt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtgoxmxcap.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tanke756.top/gthfukyhop.html

[J09] 时区处理
来源：http://hz.aizwys.cn/gtowdjspfj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhixingplan.top/gtcqmaxgrv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtztmfvqtp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtqiovjvha.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtcmtusqzl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gtgptlthgy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shzxlz.cn/gtzcsosxze.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtndstkxxa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuanzx.com/gtcdtlisem.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtkckcknug.html


<!-- 参考信息 -->