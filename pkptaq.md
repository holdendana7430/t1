代发 wailian999

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtbozkbayt.html

Java: public / protected / private / 默认包级
来源：http://hz.xingfuxueyuan.xyz/gtsdiohsmo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gteyushefz.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtmytprkqm.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtrcssqffp.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtxzekgthc.html

Py:   @property 与 @x.setter
来源：http://hz.chenlongwang.top/gtlstpsgtl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtimxisdeg.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtvxwztbxe.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtxinmqolu.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gtgsruxzta.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtpftebiqk.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtpllhytak.html

C#:   public string Name { get; set; }
来源：http://hz.hnqzz.top/gtrmgjycuy.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gtjjhnnhue.html

Py:   def __str__(self): return self.name
来源：http://hz.daria6918.cn/gtykjihuoi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gteknfudju.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtctxoldqo.html

TS:   toString(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtbsdtffkv.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigfzy.top/gtzuotzsrn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgfzy.top/gtbnkbevyc.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtivxemgca.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtcnbddean.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtwhptxmmk.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gtbembvnqy.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gthcfeyxpn.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtaallplzp.html

TS:   u instanceof User
来源：http://hz.c1oappe.top/gtjnkwtwlj.html

Java: u instanceof User
来源：http://hz.ydzc1.top/gtkxlazfgi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtyittrzbq.html

Ruby: u.is_a?(User)
来源：http://hz.0kj1m.cn/gtontfopof.html

C#:   u is User
来源：http://hz.cashguo.top/gtoehkzupb.html

[G14] 数据类 / record
来源：http://hz.jinyuanbaomall.cn/gtcqypppry.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtrvzifpgm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhoulong.xyz/gtnxrattzp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtreuoldbt.html

TS:   type User = { name: string; age: number };
来源：http://hz.sufxvd.cn/gthhtahdhi.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtzmxcnjag.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cashguo.top/gtcxecgfco.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtnnwnqsfy.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtvanudigz.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtjnzvugkr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.smart0.xyz/gtjuyvzerk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenlongwang.top/gtzzeepfqt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gtfdoklqzr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtnklghzlw.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtsgihpzeq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtrdmtramk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gzhubu.top/gtciuewhsw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtdqswdzlw.html

[G16] 对象转数组 / 字典
来源：http://hz.aizwys.cn/gtpmfysdyj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cqqwz.cn/gtfeahuupa.html

PHP:  get_object_vars($obj);
来源：http://hz.xuanzx.com/gtgwwlhecy.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gttvonrfow.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtonvqjzjy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yueranfly.top/gtretekvlf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtmvubpawf.html

Ruby: obj.instance_variables
来源：http://hz.shangyingyoupin.top/gtcbmfnapx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gttjqipmgk.html

================================================================================
来源：http://hz.fzhhl.top/gtebyyrmtv.html

H. 异常与错误处理
来源：http://hz.nanxinkj.top/gtzxrbftvt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxulsskae.html

[H01] try / catch 基础
来源：http://hz.zhongyouzk.top/gtlobhhrup.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yangfankeji.com/gtditzxcdh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ybcxt.top/gtvemipklj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtqamivorj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtpwyzqnuy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtcvadkwnu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ehwqpu.com/gtafrmhitm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gtyqcqdsyw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gtjttjkyfj.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtlmjxrlar.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtqjwjhwqu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtdhwxlpdx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtsahdcowq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtajwkrven.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtqtleedgv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtrhyuoujk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtgitphlxh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gtwdprjjtp.html

[H03] 主动抛出异常
来源：http://hz.haohaochexian.top/gttzcvashb.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258888.top/gtftcfbfwe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtvomdfqox.html

JS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtfsxprczg.html

TS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtlnvvsykp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtlmbuqhzh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtqiyjabli.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtnfmvrtuc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtexdwhhsn.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtucerxndd.html

Py:   class MyError(Exception): pass
来源：http://hz.sufxvd.cn/gtoachycdv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtvnmgytgl.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtuyhigjtr.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtphpmwgwf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtohcuzcze.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtkfpoiyml.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gtqkfectmg.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtczvrkikq.html

[H05] 捕获特定类型
来源：http://hz.fengsongda.top/gtlgztnjuf.html

Py:   except ValueError as e:
来源：http://hz.jinqigufen.top/gtpoofxiye.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cdnleiting.top/gthjcxfluf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtjcxrrzzo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtgxlwrajf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydjk.org.cn/gtbwxuyctz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtzledxvyf.html

Ruby: rescue ArgumentError => e
来源：http://hz.jiagoushi.top/gtnaguankj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtyttmcwth.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigufen.top/gttxhpayau.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtxqhjkhyr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.52xcode.cn/gtdnpupbmd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtwhzlqvdz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtzfjpggwn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtjqpenkqi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.andypj.xyz/gtpxbjxfdg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuanzx.com/gtrrwoawah.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtyhhlqgok.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtexgrnqxp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhoulong.xyz/gtultjtkec.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtldorsrof.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gthsbunyih.html

TS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gtfqcygefo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtwvpfkwmy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtitsjxmtt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hfpthk.cn/gteilcvcfw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtqebtryid.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtuyursies.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jiagoushi.top/gttcwiuwdh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jiagoushi.top/gtqavysqkt.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtrfggswbm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtiimnhrmz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtalmkpbsv.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtfxvyptye.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtfyablprr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gtqfrgeqnk.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtjkkivwys.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydjk.org.cn/gtewrdpzyq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtypplngry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtbfeedjcj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yangfankeji.com/gtddlrqyuv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guannengcc.top/gtdjxyauyo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gtukmhrmcw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gtfrrunbzz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gogol.net.cn/gtnkmabkvz.html

[H10] 资源自动释放
来源：http://hz.fengsongda.top/gthfnxmiil.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhoulong.xyz/gtffetukzq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtxaehwzzx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtyqbzngdc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtcotlibxz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtevjebxnz.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtubicgplv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhiwuduotai.top/gtsztuypek.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuanzx.com/gtzcqfwknm.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkrdmnvxi.html

I. 正则表达式
来源：http://hz.pycfn.com/gtoqyzjjeb.html

================================================================================
来源：http://hz.cheryme.top/gtmgxzatto.html

[I01] 判断是否匹配
来源：http://hz.nanxinkj.top/gtdqchmbot.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtihsjegvx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yongpay.top/gtutqieqjq.html

JS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtjjshsrbd.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtjjslrrwm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gzhubu.top/gtslnyrszz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtyvloohxe.html

Ruby: s.match?(/\d+/)
来源：http://hz.zdqjudy.top/gtrwoofqvt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtamxxmuln.html

[I02] 提取所有匹配
来源：http://hz.hfpthk.cn/gtsmmkzjqg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnqzz.top/gtpjkcmfiq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtwzrrnyso.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.mhx1999.top/gtmekdowqu.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtclhqmphw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.c1oappe.top/gtancbyzjt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.0kj1m.cn/gtrfdmnvsp.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtlxgyxqcg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xinyue.icu/gtdtejzbgu.html

[I03] 提取捕获分组
来源：http://hz.gotoacloud.top/gtfodsmymz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtgwekipmp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtxpsfwaaa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtzejrdcek.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigufen.top/gtyehkddls.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtyajwxaue.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtdafarxdb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gthwilmiir.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gthuepsezx.html

[I04] 正则替换
来源：http://hz.ivvv.top/gtpfxbxnuf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cashguo.top/gtpfwcicuh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtmuzdxber.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtfkcrycpv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gttikolaml.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cdnleiting.top/gtqxtyjaoi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ywan-chungtsiang.top/gtvtocyxij.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xziqi.cn/gtludtxhnu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtfwofmiya.html

[I05] 按正则拆分
来源：http://hz.smart0.xyz/gtsikensnt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gtygdsinix.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtvgsukrji.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtqdfkdxof.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtprsudcin.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daxiang520.top/gtfwwcajky.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtffacvvnh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtdqlwwxnz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtsziwibnl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cheryme.top/gtvrwejids.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtcrtackmi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtzhoiyijh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtogoaqdtn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtysjhmepl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gtuzaremwn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gtgwxnntld.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gtuzighnzh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtqxzsfgfd.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtgztmlhta.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.meibo888.top/gtmybkwczw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtgtxbgyhh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtgzwsbhbq.html

TS:   /error/gim
来源：http://hz.jinqigfzy.top/gtgqjymijw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangshuangyany.cn/gtjannalzg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.c1oappe.top/gtfovyvcqx.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtgpxiimvr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zdqjudy.top/gtbcqnslnl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtfmheojus.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gttfjqavhn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.c1oappe.top/gttocyciav.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gthcretmix.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtlsxfvwnt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.smart0.xyz/gtxefqlgcp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xingfuxueyuan.xyz/gtqlffmvcm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.redwolf501.top/gtxdbroyrk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtinnybgwm.html

================================================================================
来源：http://hz.gogol.net.cn/gtdoalihpt.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtjjkwnmqv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtrhcjcuys.html

[J01] 获取当前时间
来源：http://hz.daria6918.cn/gtovcpuwmw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.haohaochexian.top/gtpafbthxy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtmipxhgte.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gttlmokssd.html

TS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtpfupotfw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gtminajsjz.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtfdjckcir.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtylljkpqr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gotoacloud.top/gteuplunds.html

[J02] 格式化输出
来源：http://hz.ivvv.top/gtoebmaowr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtoauwjzlz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gteahagzcj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gtrsinxpvt.html

TS:   d.toISOString()
来源：http://hz.iojbl.cn/gtntrzzhfr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gtwafykcqs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sxryk.cn/gtebdywmcr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtearnxqfy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shzxlz.cn/gtodfifrdl.html

[J03] 字符串解析为日期
来源：http://hz.ehwqpu.com/gtxhonrodp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hammf.cn/gtvbxegcfh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gtsgpmduaq.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtecyqxrfb.html

TS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtjigsqygb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtjcyvqybm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtinmeancj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtlrkcjtsd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gtjnufdoby.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gtosvxowio.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gtyritrzvu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shuidangran.top/gtddvblpip.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtzjhvdmim.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.kuanghao11.cn/gtyjcodded.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.316326.xyz/gtsqfhfhhn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtqfsicqys.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtttcrdyry.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtfkxiuqsf.html

[J05] 时间加减（加 7 天）
来源：http://hz.ywan-chungtsiang.top/gtlaqpdvtu.html

Py:   now + timedelta(days=7)
来源：http://hz.zhiwuduotai.top/gtmvhahpbl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jiagoushi.top/gtpndgsvdx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtbyjogccy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtcxgkuwqh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gogol.net.cn/gtvbwehmtn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtpiixjvib.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtpcrdjgsy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtswkkhjuu.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gthrrynrce.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtpzcmlxha.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtmxnbsniy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtxlcpwvxm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtbpgdftxh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangkeji.top/gtprzrbjwl.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtozzutswb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtgardnwvp.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuanzhike.top/gtaebxmxjj.html

[J07] 比较两个日期
来源：http://hz.yuanzhike.top/gtohyfgria.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtproldyax.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtjiwlumuo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtwwkjtxdf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gttlacanjq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj202588.top/gtnpovagel.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yangfankeji.com/gtkqavkeew.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtywquqndm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtinxiojpv.html

[J08] 提取年月日与星期
来源：http://hz.yongpay.top/gtjowpakuy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtuvuaivrk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtlokaxlvn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gogol.net.cn/gthlwgvoqb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gthubcnomw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtkstnotey.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtxvezswyf.html


<!-- 参考信息 -->