代发 wailian999

TS:   public / protected / private
来源：http://hz.mhx1999.top/gtzaaqeeob.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gtrrhrxlcd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yangfankeji.com/gttuxcdcmx.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gteehgszbj.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtpfjnamey.html

[G11] getter / setter
来源：http://hz.cashguo.top/gtnlckwivi.html

Py:   @property 与 @x.setter
来源：http://hz.xinyue.icu/gtipllixfu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtitgsaurm.html

JS:   get name() { return this._name; }
来源：http://hz.aizwys.cn/gtedvndmnu.html

TS:   get name(): string { return this._name; }
来源：http://hz.quarkkingdee.top/gtaaakaoum.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtbntxyrqi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gotoacloud.top/gtpbsjjhfa.html

Ruby: attr_accessor :name
来源：http://hz.tian-w.cn/gtpndkirgm.html

C#:   public string Name { get; set; }
来源：http://hz.xingfuxueyuan.xyz/gtiaaivqnr.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtcbkcuydo.html

Py:   def __str__(self): return self.name
来源：http://hz.yj202588.top/gttabjssjy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtfdwyqnev.html

JS:   toString() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtealdcgdy.html

TS:   toString(): string { return this.name; }
来源：http://hz.52xcode.cn/gtmbidrkmq.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtziviskos.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gotoacloud.top/gtrfgzirgd.html

Ruby: def to_s; @name; end
来源：http://hz.sysykeji.top/gteumjboso.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gtqwhgjyyn.html

[G13] 判断对象类型
来源：http://hz.zhoulong.xyz/gtrjjhwzhd.html

Py:   isinstance(u, User)
来源：http://hz.zhijiandao.cn/gtscehpuwe.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtwzjzblcp.html

JS:   u instanceof User
来源：http://hz.chenzaomai.com/gtuolrwryz.html

TS:   u instanceof User
来源：http://hz.guannengcc.top/gtixddgqxd.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtyxjsokjn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gtcmgimkcz.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtuvkdyiyb.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtccydpeav.html

[G14] 数据类 / record
来源：http://hz.cheryme.top/gtldotfalg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtuuhnnhmk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtpwndvblu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtkbeikczz.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtyayojzaa.html

Java: record User(String name, int age) {}
来源：http://hz.hysaishi.cn/gtouueatfa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhixingplan.top/gtxpdqwpmg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cdnleiting.top/gttwsywnlj.html

C#:   record User(string Name, int Age);
来源：http://hz.yanxiufei.cn/gtzfudmtnx.html

[G15] 枚举
来源：http://hz.shangyingyoupin.top/gtstzsahta.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtlywantru.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dashuyun.cn/gtliwsmjan.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigufen.top/gtdathizlb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtladbkwfx.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtdtehsfxk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.haohaochexian.top/gtvhxsmlgg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhiwuduotai.top/gtqasqbrsb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtbvotasru.html

[G16] 对象转数组 / 字典
来源：http://hz.guowangkeji.top/gtbsrhveov.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtwrlrhzku.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtcljpctrr.html

JS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gthbdzcglv.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gttcuhijwy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cucudq.cn/gtlefbvkdi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yongpay.top/gthzoksbfy.html

Ruby: obj.instance_variables
来源：http://hz.fengsongda.top/gtakkjmivs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtzjidawut.html

================================================================================
来源：http://hz.chenzaomai.com/gtlgqwjvwl.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gtffihgxxp.html

================================================================================
来源：http://hz.nwbrower.top/gtkyaxvlfd.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtrnnislty.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtzrjnvwtr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtepwkjzry.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gteuiajdat.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtrmqnnaym.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtxbzyvdfh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.c1oappe.top/gtrcwscbit.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cqqwz.cn/gthqxuhwuu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtcpzqwdis.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtufqestxa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtwstqjciu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtbwoovjbj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtnjazrsfk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtsvdwaesd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gthbwxseuc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fzhhl.top/gtfsqnbgvt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gtyrzvyqtx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xinyue.icu/gtfpvblakh.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtllhsxebo.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtithhyafh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtlugbzemq.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtpghuiqmu.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtbgasqwlr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtkbwiegsa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxinkj.top/gtcmghkrpy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.316326.xyz/gtnewhckse.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtznixcbdu.html

[H04] 自定义异常类型
来源：http://hz.chenzaomai.com/gthcuwudvi.html

Py:   class MyError(Exception): pass
来源：http://hz.xuanzx.com/gtrmnpftwj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtozhyzrig.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtipqzcokz.html

TS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtverjstaw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtkbdekhnf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gtcxyymygl.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinyuanbaomall.cn/gtulawbxjl.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gthaistxav.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtcqgcvhkw.html

Py:   except ValueError as e:
来源：http://hz.hnqzz.top/gthrifklqt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cheryme.top/gthacqlnyo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gtvoaqgziy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtarbgnoli.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hammf.cn/gtzzoztnbj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.birdmap.top/gtckwgabog.html

Ruby: rescue ArgumentError => e
来源：http://hz.hfpthk.cn/gthlsaqppa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtuvnlflcy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gtmgnzaddn.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gtmbkaooym.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtfdxuagjo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtgxeyfbtm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtnscdtfxj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtbxaaeysu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenjidiqi.icu/gtkqsmjctv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtdkdkbguk.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhijiandao.cn/gthhmybugc.html

[H07] 断言
来源：http://hz.hfpthk.cn/gtletrtfvu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtulopxqij.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtlksnmdqu.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtipupsvwr.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtavpzitxg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtolchkjye.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tian-w.cn/gtgpjspeje.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhiwuduotai.top/gtebcgfltv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xziqi.cn/gtgwyfrheo.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtnweoeupp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuanzx.com/gtfjusvhbj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gtjxcdtwyy.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gtoflucnpf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenzaomai.com/gtetdljtmb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtjvzlgnnv.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtgtanegzv.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gtypzezqim.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtjasrgsyx.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gttjavehse.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gthgosnxoe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigufen.top/gtmlodadce.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtbyyarsoj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gtazbliubc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sysykeji.top/gtezuentrt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtlhkpeiau.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtyrjlratj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtqdmfwpbs.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtoheowzft.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtfznqcibc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtyxpiqwel.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtrqteftvr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtdcbauors.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtfauzezud.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gteursawfy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtxxnosneg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gtsghyqfwm.html

================================================================================
来源：http://hz.jianghu66.top/gtxjskqsrk.html

I. 正则表达式
来源：http://hz.quarkkingdee.top/gtxibkkuue.html

================================================================================
来源：http://hz.xziqi.cn/gtysvoscml.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtckdabdcv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gttetjdknz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gtcqmooxqu.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtrkswyvwf.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtasvzagfg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pycfn.com/gthnisygbn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yvedp.cn/gttvenomjm.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtifsvfddx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.mhx1999.top/gtzdadjapx.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gttoyynjes.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtejhrjtgy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.feifeiyinyue.top/gtydfmqfgo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ybcxt.top/gtciporqnz.html

TS:   s.match(/\d+/g)
来源：http://hz.wangdashe.top/gtpcuwcbac.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nwbrower.top/gtrmbxigqi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtujddaeju.html

Ruby: s.scan(/\d+/)
来源：http://hz.jlsjyb.cn/gtejajxcdb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258.top/gtxgzjecxg.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtrozhecbb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtzulmjkeb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gttcsqhgds.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zdqjudy.top/gteyzbwnzq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daxiang520.top/gtpecnxtgz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtejggzqjb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.316326.xyz/gtrzbwgvgd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258888.top/gtejcxrimu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtdfrlvfrx.html

[I04] 正则替换
来源：http://hz.smart0.xyz/gtlqifliqu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtiwaxxgdp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gtubqgakpn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtgvrkykhf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtlsctxnfk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xylfe.cn/gtiqsijbwe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yanxiufei.cn/gtbeqjbhkk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtndbzflcu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtzvbrmmrz.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtyinkwybw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxinkj.top/gtpghpfzrg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gtqelfwdgc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtapqthkxe.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gthxdsqeot.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtfxigkubo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtlycqdxtc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtepwqplpp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtepsttmxn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtkfeioark.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtqxsdqfjd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtsobqapio.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtwwfnccck.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtmoxqiycw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtopscayla.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtodldkaia.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nwbrower.top/gtkikopnuk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtvoojeqxf.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuanzx.com/gtyzllwckb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuanzx.com/gtdyyawabk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtdjgrsiqq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtbtfhgraj.html

TS:   /error/gim
来源：http://hz.yuxming.cn/gtqzamjalp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtzrazwsiv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtxenkqmsy.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtawcdrdob.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gtbumlevma.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guowangkeji.top/gtkoqoavjg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtyqfozozw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cdnleiting.top/gtlbmsxpxo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtdsezyglf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtlxwzrebp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gtrabdbrlk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gteerptkzo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhongyouzk.top/gtumdhqwgk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtwwvijayl.html

================================================================================
来源：http://hz.ydzc1.top/gtpqftudys.html

J. 日期与时间
来源：http://hz.shuidangran.top/gthqdihhfi.html

================================================================================
来源：http://hz.sweek.top/gtmecqjbwg.html

[J01] 获取当前时间
来源：http://hz.zdqjudy.top/gtopkznrjr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gtxufsqaec.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gtktcczpro.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtbppedyvo.html

TS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtbdnzubum.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.meibo888.top/gtkqaxnnsn.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtlkzgrwju.html

Ruby: Time.now
来源：http://hz.sweek.top/gtyxnpubxv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtqchoiaja.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtiaryofdo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtjnqvtgab.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtfohrunug.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtcbwbubaz.html

TS:   d.toISOString()
来源：http://hz.jyoumei.cn/gtwwttiqpi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtgdggorkq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xinyue.icu/gtusvntpac.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtydzpfzjr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtqzdvrbet.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtlitjjcaz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hammf.cn/gtgaooqwrk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.mhx1999.top/gtdyjkorsh.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtxyxfpqpj.html

TS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gthzbwvfus.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtfwqiklsq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258.top/gtsizedxfp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtutlenyqz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guannengcc.top/gtakdxccwu.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtiyxifunl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangtech.top/gtgyxvypng.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigufen.top/gtueicpzuu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gthmsmxhol.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtwlwrumlh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtzyufzvwf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinghuilouyu.cn/gtdumveprr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.bjfxy.top/gtofnomrqi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtvtucaggv.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258.top/gtcuezyguy.html

Py:   now + timedelta(days=7)
来源：http://hz.wangdashe.top/gtgqznzmcr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtxnhdyjwm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtilhlutnd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtamszjozu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtbqmvjvwr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtnezgygns.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cheryme.top/gtylgwdkxx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtqtpxqlqb.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtwtdpzunm.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtozvfldfx.html

PHP:  $end->diff($start)->days;
来源：http://hz.sxryk.cn/gtbuavfefe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hammf.cn/gtlbdnqynd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.c1oappe.top/gtqubtcgta.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtxhgtbpjg.html

Go:   end.Sub(start).Hours()
来源：http://hz.hysaishi.cn/gtfmeimult.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gtfqctuyab.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangshuangyany.cn/gtesdilrog.html

[J07] 比较两个日期
来源：http://hz.cucudq.cn/gtduucspft.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtekritazv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sysykeji.top/gtvlzmatrb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtqgkgnvda.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtbgeriivd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtjlkxpreq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtuoiqdatg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtldlrifxb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtmiugsvcz.html

[J08] 提取年月日与星期
来源：http://hz.ydjk.org.cn/gtuceihvml.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gttutkxutd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtjgybflvi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.9152youxi.cn/gthjvzaxfo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gtcaeuudrt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtyarsydls.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gogol.net.cn/gttndbjjmh.html


<!-- 参考信息 -->