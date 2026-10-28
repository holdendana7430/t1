代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtberndthx.html

JS:   toString() { return this.name; }
来源：http://hz.shangyingyoupin.top/gttkflqpci.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtgkyvnrsr.html

Java: @Override public String toString() { return name; }
来源：http://hz.gaohongyu789.top/gtrlfpraaf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gtwdbhuqnn.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtxywxfaxm.html

C#:   public override string ToString() => Name;
来源：http://hz.iojbl.cn/gteticawve.html

[G13] 判断对象类型
来源：http://hz.smart0.xyz/gtbgypwydb.html

Py:   isinstance(u, User)
来源：http://hz.zhengqikj.top/gtojqbsexo.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtanbipzcq.html

JS:   u instanceof User
来源：http://hz.tanke756.top/gtxcihufdp.html

TS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtatokrfxh.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtxczicbtc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtnxvuwaqf.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtqxmwxwun.html

C#:   u is User
来源：http://hz.pycfn.com/gtfaizmxhk.html

[G14] 数据类 / record
来源：http://hz.wangshuangyany.cn/gttjxdmcua.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pycfn.com/gtqzyryiuq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtuatonkge.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gtvwwcdskw.html

TS:   type User = { name: string; age: number };
来源：http://hz.fengsongda.top/gtvbytxkbb.html

Java: record User(String name, int age) {}
来源：http://hz.andypj.xyz/gtfatzldmu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shangyingyoupin.top/gtgccgkzqv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.0kj1m.cn/gtafwqzevl.html

C#:   record User(string Name, int Age);
来源：http://hz.cdnleiting.top/gtjjptbodm.html

[G15] 枚举
来源：http://hz.shuidangran.top/gtusaqpezf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtcryiiydi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtjedwysgr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuanzhike.top/gtihruyrop.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtargxiing.html

Java: enum Color { RED, GREEN }
来源：http://hz.aibaodan.cn/gtwxpxyrca.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtvnweodhu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtahewywjr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtjhetuhdg.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxinkj.top/gtnqvpsujc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cashguo.top/gtqczyoeqi.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtlqkporbj.html

JS:   Object.entries(obj)
来源：http://hz.316326.xyz/gthsfhhuif.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtppkuqmmx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gotoacloud.top/gtkxasjxff.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtgtunckop.html

Ruby: obj.instance_variables
来源：http://hz.hysaishi.cn/gtqabevqka.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtebuyugcl.html

================================================================================
来源：http://hz.redwolf501.top/gtcelfjowo.html

H. 异常与错误处理
来源：http://hz.zycfv.cn/gtmsfyqvnc.html

================================================================================
来源：http://hz.meibo888.top/gtvfpvymat.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtbyngahct.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtcrgwnfdd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fzhhl.top/gtocscfuyn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtbnxjywmj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtpbxmhpin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pengpengdd.cyou/gtekbfaxiz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtrthfswxd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gaohongyu789.top/gtekwbbquz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tian-w.cn/gtrvxraxoc.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtpznlnpqu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtydhnmvod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtuxdfdbab.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtjvwchkfr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtlusecbvx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtqiarzagf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gttdbwydpm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gthuqikdiw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ppjwa.cn/gtmgfwqudm.html

[H03] 主动抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtfzblorqj.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtatmiwqhv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtrmrvhgwy.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtnnmjysrc.html

TS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtkrekijah.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtxxnewbzp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gttvyghplk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtmxkegbfs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtmulkwkog.html

[H04] 自定义异常类型
来源：http://hz.zhaomingkeji.xyz/gtkkuxnwxh.html

Py:   class MyError(Exception): pass
来源：http://hz.vqdsnc.cn/gtovqkogui.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtckgmskvd.html

JS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtnikpexqf.html

TS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtqecfitvz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tian-w.cn/gtiqqveozt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.52xcode.cn/gttmobbumt.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtijfpqeid.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gthgvetylb.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtcdsuzlwa.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtqnfdezjf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sxryk.cn/gthhzzxcqw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtowcazoqh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtbmmmepsd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gotoacloud.top/gtilnyfccf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgufenzy.top/gtqjlzevmo.html

Ruby: rescue ArgumentError => e
来源：http://hz.birdmap.top/gtcehrahbe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtcdzgqzga.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenlongwang.top/gtdpnlnijd.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gtehjjpxbt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yongpay.top/gtxipfjqvg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtwsdfmuhp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtflvuluoq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtwyyhonvo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gtmpouilgk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tian-w.cn/gtmwbdzrcu.html

C#:   obj?.A?.B ?? default
来源：http://hz.xziqi.cn/gthrocpcrx.html

[H07] 断言
来源：http://hz.fengsongda.top/gtwbjxdmwe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dianchejie.cn/gtmjoibqwl.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtgunnthle.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtkaczeyiy.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gttrtaabfa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhengqikj.top/gtmbmqcyuh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtqiidrvwq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhiwuduotai.top/gtivmdmtfb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fengsongda.top/gtkcpahudp.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtaokysoye.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tanke756.top/gteyyosyrf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtvsdbqifa.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gtqwumuzbf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenzaomai.com/gtwzwnmbzw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhoulong.xyz/gtyzvdwgem.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtervgspwa.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtjxanaikr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gtkfixxcrm.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtqhqhhdof.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtfczbfadb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtttwqwclz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtizxxrywv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jiagoushi.top/gtfftiptiy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hammf.cn/gtbujdppht.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtqnraxreo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shuidangran.top/gtqgfwwrcu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.0kj1m.cn/gtxacpancb.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtipyhaopa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtgwbsemoe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtkcipqqpt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtypacziqc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtulxnbpkg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtxpexcqvd.html

Go:   defer f.Close()
来源：http://hz.dianchejie.cn/gtzvnedpnf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.redwolf501.top/gtxwrpusdg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fzhhl.top/gtoeryfyoq.html

================================================================================
来源：http://hz.iojbl.cn/gtfecghemq.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtzfcmsjmc.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmuverips.html

[I01] 判断是否匹配
来源：http://hz.ydzc1.top/gtbbvunlio.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtudhhviww.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtrrjwgobu.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtcinhakjl.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtleszejcf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tian-w.cn/gticgmmiyd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtrrvjztin.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtaavpiuqh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hysaishi.cn/gtznzapyyg.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtzfmyrhin.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtsxjiivdr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtbdjyappc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jianghu66.top/gtfitckiru.html

TS:   s.match(/\d+/g)
来源：http://hz.ydjk.org.cn/gtbhyltabd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydzc1.top/gtqbdppgmo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtnvalgydc.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtuwtubtaw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnxiangtu.top/gtmnphpgio.html

[I03] 提取捕获分组
来源：http://hz.zycfv.cn/gtddzwqlin.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtvbgsiebg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtagoyvikm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtpgvmnmnv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zdqjudy.top/gtmqfjqpij.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gteqkiywhl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gtorqjvuvj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenjidiqi.icu/gtrutqjarg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gttjaqupbh.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtfmgublsn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.birdmap.top/gtdveztuya.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtuodlobma.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtgsywesxy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gttbyjbeoc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtmluqldcr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhoulong.xyz/gtgacymkog.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cdnleiting.top/gtgjwpoquv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigufen.top/gtzphjbptn.html

[I05] 按正则拆分
来源：http://hz.xuanzx.com/gtketceqsv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gtwmghitus.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtplxngqxz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtdhmqgmnz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtwayckflu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daxiang520.top/gtpfrfiucy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.quarkkingdee.top/gttxgisapv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtmcookkos.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guannengcc.top/gtpmbodyer.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtjhihrqcl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtyeqdnmqu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj202588.top/gtmlqjmjzo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gthkjoqzjm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtrbxtuiuo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.meibo888.top/gtwvarzrpb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtocpbfdms.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ivvv.top/gtihpkwkgm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtvrzdpfqi.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtawcruszx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtzqcmyiok.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtnolbasyf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yanxiufei.cn/gtgfmmaide.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtduvhglms.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtyuuyfkyz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gtxkcpukkr.html

Ruby: s.scan(/error/i)
来源：http://hz.yueranfly.top/gtmrksjaax.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinyuanbaomall.cn/gtuesixaxd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtgyubyyth.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pengpengdd.cyou/gtesflypmn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.birdmap.top/gtdunwamej.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gthqknhojf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtnborguxo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtwhgmmtnc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jlsjyb.cn/gtissifnpm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuanzhike.top/gtvvejvqoa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtfqtozhsh.html

================================================================================
来源：http://hz.fzhhl.top/gtljhfoqua.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtobmmyoid.html

================================================================================
来源：http://hz.jqgfzy.top/gthpochscv.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtagbenlxr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinyuanbaomall.cn/gtkcmshdar.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtmclnqgnf.html

JS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gtmojafczs.html

TS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtwpazgues.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtxbqylehj.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtykkefqyj.html

Ruby: Time.now
来源：http://hz.xuetiantiany.cn/gtyqylrguu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtqeuznmqx.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtybpmnnhy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtrkaitwnp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtklfqxukc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gtfebexuti.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtlutxmzjf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gturtehrwg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtirzjtwub.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtpisiiwwd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj20258.top/gtxsfghytb.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gthwalgsez.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtbfnicsdt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gtgmdnbfdj.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtvbjdtqwu.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtqdqcfqxp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ivvv.top/gtwpgynqsx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtlznsmtam.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtpbxzxdku.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tian-w.cn/gtqfapkkon.html

[J04] 时间戳与日期互转
来源：http://hz.zhixingplan.top/gtsndayssw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtahhzxrmh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtbnyxvcpd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hongshengwenyu.top/gtjpgogjxm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtbpzncdra.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gtmnfyfxga.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtalarohyu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangtech.top/gtnaodwrun.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hysaishi.cn/gtwloafqhc.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtbttedbhd.html

Py:   now + timedelta(days=7)
来源：http://hz.zhixingplan.top/gtesemsukz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gaohongyu789.top/gtkiumwzto.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gteeoijcgp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtlmmrmeev.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtykywzpaq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fengsongda.top/gthtxxzzha.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nwbrower.top/gticyorbrl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtkdrygucf.html

[J06] 计算两时间之差
来源：http://hz.fengsongda.top/gtioxjvaib.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtgcqupoqr.html

PHP:  $end->diff($start)->days;
来源：http://hz.mhx1999.top/gtssxabspg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pycfn.com/gtaczlopkd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtdcdwsivw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtgaxpslev.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenzaomai.com/gtsboqgydg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtpathocvi.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgufenzy.top/gtpolawraq.html

[J07] 比较两个日期
来源：http://hz.vqdsnc.cn/gttvakdnjq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtmsaalcfs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtsishqicv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtktagwnoq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtgazbnvqz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aibaodan.cn/gtulgmuugt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtckjvrjwd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtlchgljad.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtqavhacno.html

[J08] 提取年月日与星期
来源：http://hz.gotoacloud.top/gtxelszuqq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtmjmdepee.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ybcxt.top/gtmzzqabuw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtydtzgmve.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtcdkgsocu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gthysrekhx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtkezsbsmg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hysaishi.cn/gtcmevygpu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtkgzburqx.html

[J09] 时区处理
来源：http://hz.shangyingyoupin.top/gtchobznvy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtspfsnkuz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtuqgblcrm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtcpteypzp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtyiynexie.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shuidangran.top/gtifytvhqs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shzxlz.cn/gtgwxapnny.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydzc1.top/gttmdnqsqk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gttuyhvsdr.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gttdhswvut.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gttelnhgzp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guowangkeji.top/gthhvpzlpz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtttnoocgw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtauqgmkbz.html


<!-- 参考信息 -->