代发 wailian999

TS:   public / protected / private
来源：http://hz.hnxiangtu.top/gtptxauzci.html

Java: public / protected / private / 默认包级
来源：http://hz.zhixingplan.top/gtiebgwasl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtyseuddsa.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtwsmnocyy.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtxsmadxsf.html

[G11] getter / setter
来源：http://hz.shzxlz.cn/gtisuxycps.html

Py:   @property 与 @x.setter
来源：http://hz.wangshuangyany.cn/gtdnensuul.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtlscexioa.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtrtozaxqw.html

TS:   get name(): string { return this._name; }
来源：http://hz.cdnleiting.top/gtlzkxblhy.html

Java: public String getName() { return name; }
来源：http://hz.havefunace.top/gtwghfphtq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.redwolf501.top/gtvyngeyob.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtovrtetmf.html

C#:   public string Name { get; set; }
来源：http://hz.ydzc1.top/gtgyxonwkq.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtjksqsdsm.html

Py:   def __str__(self): return self.name
来源：http://hz.kuanghao11.cn/gttmfrfghd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtxcsinegh.html

JS:   toString() { return this.name; }
来源：http://hz.dianchejie.cn/gtmwjuktwv.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangdashe.top/gtifflxqxn.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydzc1.top/gtfadmggqt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dashuyun.cn/gtwzxtwypb.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtngzuogkc.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gteunjlvwj.html

[G13] 判断对象类型
来源：http://hz.aibaodan.cn/gtsevmkuaa.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gtewknokkm.html

PHP:  $u instanceof User
来源：http://hz.pycfn.com/gtnuwhusay.html

JS:   u instanceof User
来源：http://hz.birdmap.top/gtmdiolujn.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gtavcnhvie.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtnlsnpcnn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtfwyimteu.html

Ruby: u.is_a?(User)
来源：http://hz.shanyushiyangtech.top/gtccdukprk.html

C#:   u is User
来源：http://hz.hammf.cn/gtqlgsguiu.html

[G14] 数据类 / record
来源：http://hz.redwolf501.top/gtnrjdzgmz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtsvxnppxg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zdqjudy.top/gtohpdenah.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinghuilouyu.cn/gtotwabfeq.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gtnwgyjwof.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gttnrjdadg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tianlin.xyz/gtgdjjxhqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gteshgyygr.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtmdwghtrb.html

[G15] 枚举
来源：http://hz.vqdsnc.cn/gtsjydndkj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gtexpxcrys.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sxryk.cn/gtqoamwosw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gtackhuxop.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtrfjczsgl.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtznvquyht.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtnqfoqplc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtohwdllio.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtlxsodjam.html

[G16] 对象转数组 / 字典
来源：http://hz.xuetiantiany.cn/gtjzcuqooz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nwbrower.top/gtpeypumbh.html

PHP:  get_object_vars($obj);
来源：http://hz.c1oappe.top/gtqjzoluxl.html

JS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtrequtgpj.html

TS:   Object.entries(obj)
来源：http://hz.nanxuanxn.top/gtjfqgyspj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gogol.net.cn/gtlzkcwncl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ywan-chungtsiang.top/gtbtcpiqij.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtiyhodlot.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhoulong.xyz/gtockwmmvs.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtylppxzcp.html

H. 异常与错误处理
来源：http://hz.316326.xyz/gtcxyrurjq.html

================================================================================
来源：http://hz.guowangkeji.top/gtsfngwezz.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtzaxycbbo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ivvv.top/gtbankgdin.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtxmxxlwyv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtdxsfdnnr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gteplskniu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gtprhpkzau.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gtvnzspqme.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgufenzy.top/gtfqpegupb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtbxbagotl.html

[H02] finally / ensure 收尾
来源：http://hz.smart0.xyz/gtlfiwjtdg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nwbrower.top/gthuplxuth.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtrgalvxvu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtsztmntcd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtmsfocsoi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gteolvvfcl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtrczdzfpw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xingfuxueyuan.xyz/gtlwpsqtwv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuetiantiany.cn/gtgggrlvmp.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtzsxnyxin.html

Py:   raise ValueError("错误信息")
来源：http://hz.jiagoushi.top/gtwdvpskxx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtclyisspp.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtxubxpnxq.html

TS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtafsprtit.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtyflutuwr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pycfn.com/gtwralkjde.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangtech.top/gtvanjrdtz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtudscyqkx.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gtgrzewlcx.html

Py:   class MyError(Exception): pass
来源：http://hz.gogol.net.cn/gtsmvzchgy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtwthbhmbm.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtoolwnwjv.html

TS:   class MyError extends Error {}
来源：http://hz.hfpthk.cn/gthuultltp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nwbrower.top/gtfexxrmap.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aizwys.cn/gtslwzkizw.html

Ruby: class MyError < StandardError; end
来源：http://hz.vqdsnc.cn/gtintfunpq.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtyrwynhgx.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtrqwupxut.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtlpwlflzs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guowangkeji.top/gtlndptlbm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtputtcyvt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtbktcyjne.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtzopeggob.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gtmdvzeyfd.html

Ruby: rescue ArgumentError => e
来源：http://hz.gzhubu.top/gtdgntkdam.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtqykctvna.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtsficecyc.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtalhtsmmg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhongyouzk.top/gtdbvfnwpo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtklzcnymf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtwhuxosfm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtdbytcqrd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtahevaraw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtwhmrcvkh.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtuzfbdsvl.html

[H07] 断言
来源：http://hz.xuanzx.com/gtlqkzqlvd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gttcuosdii.html

PHP:  assert($x > 0);
来源：http://hz.shuidangran.top/gtpnkltcou.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtidjillqt.html

TS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtwgqtlzfl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtbpqhueqi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jiagoushi.top/gtkdcdgofb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtixlnwgtb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aizwys.cn/gtfbuzugje.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuanzhike.top/gtxwxcakuh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xingfuxueyuan.xyz/gtdfldihln.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinyuanbaomall.cn/gtmtkxrrtg.html

JS:   e.message;  e.stack
来源：http://hz.jinyuanbaomall.cn/gtcgpdfsxh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sysykeji.top/gtlhruljxr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuanzx.com/gtfnqbzwmi.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtimpkmebb.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtzezflcpy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.feifeiyinyue.top/gtgsvmielt.html

[H09] 带错误码的异常
来源：http://hz.andypj.xyz/gtajfdyrmc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtpnltpldv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtxxdtktrw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuetiantiany.cn/gtmzndomrk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtzhrsojsi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gtcuitkrsb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ivvv.top/gtusmqgauz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hongshengwenyu.top/gtudngfhkf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtahpahzsy.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtwasgmibu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtuijuxkqb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.birdmap.top/gtazylfozt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gteqkfgfio.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtzvdnjekb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gttosmbmfl.html

Go:   defer f.Close()
来源：http://hz.yj20258888.top/gtqtcgacep.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtkckmdyeg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gthuwxueav.html

================================================================================
来源：http://hz.xinyue.icu/gtmkiaroet.html

I. 正则表达式
来源：http://hz.quarkkingdee.top/gtuthfoejf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtovjvnnqz.html

[I01] 判断是否匹配
来源：http://hz.yonumen.top/gtazrxjecg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258888.top/gtpnvbhwcq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtlmcxnbbp.html

JS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gttlamthdx.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtxeylhqwi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhengqikj.top/gtykhqruso.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuanzhike.top/gtxpaoxvxv.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtfgxqwybo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cashguo.top/gtzrybcicg.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtsdwprbnw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.havefunace.top/gtwsdjkpkq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.havefunace.top/gtflohqjtq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gogol.net.cn/gtseniclgh.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtxnjbyipj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtbxkjikpn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtvslbaazq.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtgnvxvnoq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigfzy.top/gtuhjxxhts.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtgmdzwywq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gthayixqyp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gtyvueldzt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shzxlz.cn/gtpmsqegcn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangtech.top/gtaoimsrtv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtpjekmqtf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuanzx.com/gtwfoxtesp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtpvpcrzti.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shangyingyoupin.top/gtbuiwhjyk.html

[I04] 正则替换
来源：http://hz.yonumen.top/gtuhiqlcav.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtytlzydtg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtebnjfpen.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtitxzamep.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gthzzihmhs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtexoixgyv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gtssozcoum.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtslsazuqe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yanxiufei.cn/gtekjkltpc.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gtjusorcnz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dianchejie.cn/gtatzepqjs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jyoumei.cn/gtegpgyxlc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtpghbawtu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gttfmnbaog.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuanzx.com/gtzbttvmbi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.snrcjt.cn/gtxeyabnhy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtjhkcuhho.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtkqfuoxfa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yvedp.cn/gtbiaqehvp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtrzeherja.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtjieggsxs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtvgraullp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtcosdjxts.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gtakghxhxj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tian-w.cn/gtuakxpinh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtuelyvzjf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtoknjsect.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtmyavpnua.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtlkhxhpeb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.svipenyu.cn/gtbsyjzkzk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sweek.top/gtudpaovnj.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtovruibxh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtbhliqzog.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinghuilouyu.cn/gtnzcbhbsz.html

Ruby: s.scan(/error/i)
来源：http://hz.aibaodan.cn/gtprtnhcar.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.kuanghao11.cn/gtmbyaycle.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtkadzmcch.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtxniytdip.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shuidangran.top/gtktfkvffd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtqngggrzl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtzkpvrgbg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuxming.cn/gtwxiaopol.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtjxavgajb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtjjjppxnu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gtufxwcjgx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwxluense.html

J. 日期与时间
来源：http://hz.xuetiantiany.cn/gtqtjmofww.html

================================================================================
来源：http://hz.jqgfzy.top/gtdgodusyg.html

[J01] 获取当前时间
来源：http://hz.ppjwa.cn/gtxxuzylrc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtjilwhaov.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtvtdrcmum.html

JS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gtbdzqjnht.html

TS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gtckhrjegp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuanzhike.top/gtezoffaws.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtxpmrgrie.html

Ruby: Time.now
来源：http://hz.hammf.cn/gthfzmiwlt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtvrknigya.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtcrlwnbyr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtbeppkogl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtylpjlesm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.9152youxi.cn/gtpmmptjov.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gtfucplezl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shzxlz.cn/gtpcvfvddo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hammf.cn/gtgvjtydls.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtcteczmtc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtbyghaoss.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtwjugfpwj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gtodmdbhqt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtbwnxuryl.html

JS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtvssxjamm.html

TS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtzslfmvhy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtwrvhpsfa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgfzy.top/gtvndfvgvw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gthhunkhjk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtjhtiimzj.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtjkmirfgt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gtdxauhtci.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtmfimxkyu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gteytxsoln.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.iojbl.cn/gtxicbhtac.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cucudq.cn/gtahjdqmrf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtkfvmgdac.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cqqwz.cn/gtykvvnzxx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnqzz.top/gtweiksouz.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtmfahuxgq.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtwmrvpens.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yongpay.top/gtxknobasa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtxrwbbnrb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtrkmampmv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gtiojlbmbc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtlxomixht.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtvxkbrcfg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jiagoushi.top/gtjucyzcsj.html

[J06] 计算两时间之差
来源：http://hz.xylfe.cn/gtgsevcgdb.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtqvaikapn.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtkxoitunu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtvjkdctzv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gtebrzxcbf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.svipenyu.cn/gtkgleqxer.html

Go:   end.Sub(start).Hours()
来源：http://hz.9152youxi.cn/gtdvcrokjt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtsexnrwgl.html

C#:   (end - start).TotalSeconds
来源：http://hz.cashguo.top/gtqissscpf.html

[J07] 比较两个日期
来源：http://hz.nanxuanxn.top/gtpdsfnpkw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtanfwsilt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtxravvhag.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtkhzhbfnp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtdaefadxy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtrcjumcic.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxuanxn.top/gtyturszcd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtsyclevka.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gttxxertzo.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtgibfadgn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tian-w.cn/gtcxmofqwk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtppzufgvt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zycfv.cn/gtfsinbyxd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtufnvhwik.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gtnckdpoeq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtjvvhosip.html


<!-- 参考信息 -->