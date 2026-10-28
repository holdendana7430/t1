代发 wailian999

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtifcpnbcn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydzc1.top/gtwzzedfvp.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtxqodysty.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtihdxsrbf.html

TS:   public / protected / private
来源：http://hz.nanxinkj.top/gtllsgafli.html

Java: public / protected / private / 默认包级
来源：http://hz.pengpengdd.cyou/gtxqmfqtag.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtvmksunog.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtnbygnqyk.html

C#:   public / protected / private / internal
来源：http://hz.gotoacloud.top/gtpskifwad.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtkjpmypsp.html

Py:   @property 与 @x.setter
来源：http://hz.ppjwa.cn/gtwaekzkzv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtweviyhhf.html

JS:   get name() { return this._name; }
来源：http://hz.hysaishi.cn/gtbkwrqsxi.html

TS:   get name(): string { return this._name; }
来源：http://hz.bjfxy.top/gtquwsheqd.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtsbklhjvb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtrmjfmgmu.html

Ruby: attr_accessor :name
来源：http://hz.yj20258888.top/gtboouablr.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtflelasfy.html

[G12] 对象转字符串
来源：http://hz.cdnleiting.top/gtcpbkkcjn.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtfpsjxumv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtmspyopdc.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtbnckehix.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtioejbpln.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gtrgwkgequ.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.bjfxy.top/gtugjvqadk.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtpyphdbie.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtplsqjzsb.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gttntcvrwv.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gtpuldypxp.html

PHP:  $u instanceof User
来源：http://hz.hywenlv.cn/gttgeqjhkm.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gteuuoehze.html

TS:   u instanceof User
来源：http://hz.pycfn.com/gtbiaupjmq.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtpbqazuji.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtcauvzheq.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtiybdyqou.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtmujxmrra.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtnobaaqxw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gtknpjjmkv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtvdznrldt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtypggfucs.html

TS:   type User = { name: string; age: number };
来源：http://hz.zdqjudy.top/gthcpnlhkw.html

Java: record User(String name, int age) {}
来源：http://hz.havefunace.top/gtupotodpb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gtctvxihpa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtwmbfrcci.html

C#:   record User(string Name, int Age);
来源：http://hz.snrcjt.cn/gtwehuljqk.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtmbrvokld.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gtncurfyjc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fengsongda.top/gtyckwqvhi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinghuilouyu.cn/gtszpujvrc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtmtlzjlzg.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtmpudjxny.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cheryme.top/gtfqsfitks.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtedrppabb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtolltjfom.html

[G16] 对象转数组 / 字典
来源：http://hz.gzhubu.top/gtxgnomfck.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gthfcqydaw.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtlvpjluio.html

JS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtywprjyca.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gthjgomnbe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pycfn.com/gtmtyogjsw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gtikgxhuqn.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtdivwderz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtjgwemvgu.html

================================================================================
来源：http://hz.cdnleiting.top/gtvjudujbt.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gtcrsyxqzs.html

================================================================================
来源：http://hz.guowangkeji.top/gtpirsezgn.html

[H01] try / catch 基础
来源：http://hz.dianchejie.cn/gticaunigw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.vqdsnc.cn/gtfsudhvpq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtsigswaqy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtonsrsfgi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cheryme.top/gtacfrxeoo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinghuilouyu.cn/gtabndvnky.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhaomingkeji.xyz/gtegbksmzm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zycfv.cn/gtkwyumspn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ehwqpu.com/gtcvnhfcwr.html

[H02] finally / ensure 收尾
来源：http://hz.ybcxt.top/gtaapdlsal.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangtech.top/gtwpxzybqe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtpeabpoxv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtynswzrcz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gteznexsnf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtuknxlldi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hongshengwenyu.top/gttsgnmxbo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtzqmpabks.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtrsjnkngc.html

[H03] 主动抛出异常
来源：http://hz.nanxinkj.top/gtjjimfofg.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhaomingkeji.xyz/gtwvqxsvhp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtckvxavsu.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtxvwcslnf.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtvtpduwpv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtislsirfc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtldndhtrw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.0kj1m.cn/gtxjzjnlog.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gthwtjhhgs.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtfkvechuu.html

Py:   class MyError(Exception): pass
来源：http://hz.ehwqpu.com/gtjhyvvlaq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtptmpaymq.html

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtymrywkvg.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtpfpwqjjp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtaunglawm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtyqaiglup.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhongyouzk.top/gtjqshozgz.html

C#:   class MyException : Exception {}
来源：http://hz.hnxiangtu.top/gttbrzfoxo.html

[H05] 捕获特定类型
来源：http://hz.c1oappe.top/gtsdtnojxp.html

Py:   except ValueError as e:
来源：http://hz.9152youxi.cn/gttgjxyrrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtsyyeydbb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtzvdkqkcu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtzwmhbntz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtgdjhwrcb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gtntpyjajt.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtvejvajpo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtnwwcvffr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gtyhwajzix.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtznwaquuh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.0kj1m.cn/gthhjnvope.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtqqjlfwzl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtqfnyhrzg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtqqeevcfe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yueranfly.top/gtvuijfwxv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gteyvbywax.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtqpqwynsh.html

[H07] 断言
来源：http://hz.zhixingplan.top/gthpjenvvu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtwihyabyh.html

PHP:  assert($x > 0);
来源：http://hz.hongshengwenyu.top/gtbodzckae.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtvgcylwvh.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtkgtqrimw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtytvxqcrb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinghuilouyu.cn/gtdvrdlybk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtksiofapz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxinkj.top/gtdvmgbnmj.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtahlgyuyq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtrsntohqj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangdashe.top/gtkxeqwrcn.html

JS:   e.message;  e.stack
来源：http://hz.cdnleiting.top/gtuqzvmvzf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gtkcqbtuoz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhongyouzk.top/gtzktuhvnq.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtilloagam.html

Ruby: e.message;  e.backtrace
来源：http://hz.haohaochexian.top/gtvczycqqf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtdrpzgzqy.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtgojhdfyu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangkeji.top/gtuslppigi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtfoicmpho.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gtdyptvfow.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtbjhsxask.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ehwqpu.com/gtxpuumise.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.vqdsnc.cn/gtnabpjbfd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtejqncwmm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenlongwang.top/gtbyokqktb.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtrqanreqn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cheryme.top/gtoxqcxagk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtxmyxwtgb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtutdbmmcb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtonshqyao.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtkmldezje.html

Go:   defer f.Close()
来源：http://hz.shangyingyoupin.top/gtbuqckqym.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtpperquyn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuanzx.com/gtuyzbarlu.html

================================================================================
来源：http://hz.gzhubu.top/gtpvbhqnco.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtmvzhoeqm.html

================================================================================
来源：http://hz.gogol.net.cn/gtrthlteyw.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtjendgctq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hysaishi.cn/gtknsfwdyf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtkfpyvuxr.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtznvmkeqb.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtikhxuixq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gttmxtqely.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtarzgsyup.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gtvdysmfry.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.mhx1999.top/gtswkcqwru.html

[I02] 提取所有匹配
来源：http://hz.shzxlz.cn/gtjgtdtujq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gtczuwdkbo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtfxusrpmd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtlttokgwt.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gttqjkgtfs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gteeaffvgd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtimoyudpz.html

Ruby: s.scan(/\d+/)
来源：http://hz.nwbrower.top/gtntgtiwgf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtflonuyrg.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gtgryzmhsl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gthbbucxxh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yangfankeji.com/gttrqulunl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ppjwa.cn/gtafxzwsrn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hywenlv.cn/gtifyzbyex.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtpjvqhpmr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtnnxqikpq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtgdiczhdv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuanzx.com/gtudgtzbos.html

[I04] 正则替换
来源：http://hz.gaohongyu789.top/gtvkmuosyp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ivvv.top/gtkzucapdl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gteorlurdr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtuflyuivb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.c1oappe.top/gtdathnxxf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtlsupjxhr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtptfoompz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtosatgsxq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtciqqydpn.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtdkdiclgn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.svipenyu.cn/gtjampovvy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.snrcjt.cn/gtnqxijvmi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtsxrgvdvc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gttgdkfnfy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jlsjyb.cn/gtnzcdxels.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tianlin.xyz/gtmfaranej.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gthwkjdvvn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtzpdbeomu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtzsgupjxf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtamdbhmnn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenlongwang.top/gtzhkgxzvt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtkcbxdycl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.birdmap.top/gtvcqdqfnq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gtobadrvax.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtubslomrz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtudjslggt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtzworetae.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtfmwyguoy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtmekvwhgk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtemmkkljr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtymgeauku.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtvqhcmldr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hywenlv.cn/gtgrjqxypz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtnvtylvtt.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtuejstbaa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gttvtufuyf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenjidiqi.icu/gtqqjlwxik.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtckbvnaks.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtztsdxgsa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gteognamsr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtudjqmpsy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtkakksgqm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtsfnftbxm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.bjfxy.top/gtwdzyeved.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gotoacloud.top/gticlgoghr.html

================================================================================
来源：http://hz.jyoumei.cn/gtpvibzikp.html

J. 日期与时间
来源：http://hz.hfpthk.cn/gtvvoanatl.html

================================================================================
来源：http://hz.hnxiangtu.top/gtexnfcoul.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtswjgbnnc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtdbidxhyr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtdliedhxo.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtscmoupkm.html

TS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtgcoqcbts.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gtznahwzzd.html

Go:   time.Now()
来源：http://hz.cqqwz.cn/gtnfsyygpo.html

Ruby: Time.now
来源：http://hz.hnxiangtu.top/gtntbpcggv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtgtjgegqd.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gttdkqmfcm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gthodbqpmr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gthjtagnmm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhaomingkeji.xyz/gtfuifdtsi.html

TS:   d.toISOString()
来源：http://hz.dianchejie.cn/gtebftnhif.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtjratsyem.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jiagoushi.top/gtszoxbybc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtrvxgyavx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtrgackebr.html

[J03] 字符串解析为日期
来源：http://hz.havefunace.top/gtzdcucckj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.feifeiyinyue.top/gtrdtnqvjs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtsnusvoda.html

JS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtpobolxac.html

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtynsydorf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tanke756.top/gtbyissbng.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtfjiidrjv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtnmfcxysn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhengqikj.top/gtrwqnwkmn.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtdgkzbzxt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yangfankeji.com/gtvsjnjpga.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yongpay.top/gthycffezp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.meibo888.top/gtxcwbjjns.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtpfstwwrz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jyoumei.cn/gtweyhsmsv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtgiwdwivg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigfzy.top/gttihmglon.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtgxffjimq.html

[J05] 时间加减（加 7 天）
来源：http://hz.cheryme.top/gtsxxzaxcu.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gtkhimstlf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangshuangyany.cn/gtmdtvkkde.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtswdpuqmh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtszsivvgx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.0kj1m.cn/gtqftrqgir.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtfvjtvbrg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.havefunace.top/gtakfwzrhv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aizwys.cn/gtxbwxjuoa.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtajckvxdl.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gthunfzklk.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtltahrpes.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dianchejie.cn/gtgqaluvvr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cucudq.cn/gtzcambyis.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtayaxwool.html

Go:   end.Sub(start).Hours()
来源：http://hz.tian-w.cn/gtvcjrrziw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtuskmrzer.html

C#:   (end - start).TotalSeconds
来源：http://hz.xinyue.icu/gtoqnimnoh.html

[J07] 比较两个日期
来源：http://hz.smart0.xyz/gtqqrvxigd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtxcvdepqt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtffixomva.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtuwtixjkj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtovyqoste.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.feifeiyinyue.top/gtishusejr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtndswazjl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtxjewsjzn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtpdylqmiw.html

[J08] 提取年月日与星期
来源：http://hz.jinyuanbaomall.cn/gtgbrfisgu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gtkwmnhmwj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtmoiagteh.html


<!-- 参考信息 -->