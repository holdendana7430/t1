代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.zhiwuduotai.top/gtbevzoikp.html

[G15] 枚举
来源：http://hz.shzxlz.cn/gtwkrdzjjy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gtzrlfugnh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtjibtsxux.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtxudiaqqz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gthojaztwr.html

Java: enum Color { RED, GREEN }
来源：http://hz.hywenlv.cn/gtatbhleko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtpuvuuhbo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtnzniepfg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtjnyeayli.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gteefdrpxg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gtjxpvzvjq.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gtdqtmzlrx.html

JS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtqibbetfv.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtvohlntet.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtbvphspkg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zycfv.cn/gtmqiediyp.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtxovpeqmy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtnbnkenhd.html

================================================================================
来源：http://hz.gzhubu.top/gtnyscqqjr.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtbfulofrk.html

================================================================================
来源：http://hz.zhongyouzk.top/gthlxehmvp.html

[H01] try / catch 基础
来源：http://hz.vqdsnc.cn/gtocdbziwk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtlidkcncz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtdrrbdqwo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtmtdceyjo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtxctvykoc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gtyhccqyqf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtrhbekbyk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuanzx.com/gtfhjvorwi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtfcswfbbl.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gttddylyqo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.svipenyu.cn/gtefcxhmrr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtxuhzqlxw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtqfosmpld.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtkgkussbg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gteirtkzui.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xinyue.icu/gtndaqcvfj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nwbrower.top/gtsyqnnsow.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gtkbsdbvgg.html

[H03] 主动抛出异常
来源：http://hz.snrcjt.cn/gtdzimjsgb.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtssfkmcnn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtaepstvre.html

JS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gtwcvonsyw.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtancnscnx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtdpujwgyt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydzc1.top/gttaxuxyro.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gtjslajhmz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gtiwhrieec.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gttygeumxd.html

Py:   class MyError(Exception): pass
来源：http://hz.redwolf501.top/gtmoakfvbb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtnpgoulor.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtitokodso.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtlhvrxjxp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtllqmcxqz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gttjfftimc.html

Ruby: class MyError < StandardError; end
来源：http://hz.xylfe.cn/gtgmmqqjiz.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtxjpieuai.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtcckmkzok.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gtlywpessi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gtpsxjfjeu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtziqzhllc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtwulojbbr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yonumen.top/gtzvipchrj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tanke756.top/gtlgfywsko.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gtcecgmzsk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtirgonoak.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ywan-chungtsiang.top/gtkdyljggq.html

Py:   value = d.get("k") or default
来源：http://hz.bjfxy.top/gttrkenoio.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangshuangyany.cn/gtxqgvuxan.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtuwrwdrsp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtmlssgvyw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.dashuyun.cn/gtnctpnsvw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.vqdsnc.cn/gtpphuvmwc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yonumen.top/gtbwxxlmau.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhixingplan.top/gtgfhjbzfq.html

[H07] 断言
来源：http://hz.yongpay.top/gtyzctttob.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gtlgmqhaho.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gttplvnsgg.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtkyltqopa.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtcogjihha.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hongshengwenyu.top/gtlfpmfxdl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.c1oappe.top/gtiznyorfj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtjqjltlyi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtwqzcfqxu.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinghuilouyu.cn/gtssgmdpmt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yanxiufei.cn/gtyyufpbkg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtcjcfivfd.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtsepxnebr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ppjwa.cn/gttxnzacda.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gogol.net.cn/gtbwddlykb.html

Go:   err.Error()
来源：http://hz.andypj.xyz/gttsojspji.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtytuxdrms.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtkqbrapyu.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtthgjvfbz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ywan-chungtsiang.top/gtmmsdtylx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gtjjldayau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtwpnpyjeg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtdeceuhiz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.smart0.xyz/gtjrovgutk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gtwteolixj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yanxiufei.cn/gtvzonqqxh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtvecwqqyg.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtwpwuimlr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnqzz.top/gtmkguxtbu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtdgvntvmk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtktkjtnin.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtlccvcnvq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtgjfkojyx.html

Go:   defer f.Close()
来源：http://hz.zhijiandao.cn/gtimrjdzts.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gtppfqywnj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sufxvd.cn/gtzergnrax.html

================================================================================
来源：http://hz.jlsjyb.cn/gtnupzwuoi.html

I. 正则表达式
来源：http://hz.gotoacloud.top/gtttvbgflc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjgkestce.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gtisxxwdxw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtiitnojsr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shzxlz.cn/gttcfmkebj.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtiqtqihys.html

TS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtoxguhemj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hysaishi.cn/gtjazrozxt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aizwys.cn/gtzxhcglne.html

Ruby: s.match?(/\d+/)
来源：http://hz.vqdsnc.cn/gtykqsfmzt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.redwolf501.top/gtormqedxo.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gteshvepkv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtsxxwygpr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtppmbesic.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gtbyfbsxvh.html

TS:   s.match(/\d+/g)
来源：http://hz.mhx1999.top/gtfhrnfurl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtwvlnwxaz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgufenzy.top/gtscffzlxx.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gtrxjropbo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtrvsiuqyp.html

[I03] 提取捕获分组
来源：http://hz.cucudq.cn/gtumqaddtd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangkeji.top/gtykrxjpyo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtzuxiuuov.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtghejefnq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuxming.cn/gthcvrfmra.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gtgtkaiqwg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtjwqpmrin.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aizwys.cn/gtymiltlbr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnxiangtu.top/gtwgyuxylh.html

[I04] 正则替换
来源：http://hz.nwbrower.top/gtjpiyyqog.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gtnfvtqqrz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtkpmjfdba.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtubknakad.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtlsgwksri.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuxming.cn/gtegzgbewf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.redwolf501.top/gthkfjwzrb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtxraqqwks.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.redwolf501.top/gtyupxmihr.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtuplcedzz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxinkj.top/gtbxolbyak.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtfygnbbvv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtcaalmdsx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gteuqmklyf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtmlekxslm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtxaqnrwff.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtzvvcqedi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtdeggsgvm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydjk.org.cn/gtqswkvycp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtcfplzfjx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cashguo.top/gtigvmckek.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtcfibtnyr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtkzkmtdtd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtkmwbemna.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtnvgeitqk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtfdtcuwda.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gthakkbsww.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtdaxinouw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gtuppnqtdv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gteoruevyy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtencdeowu.html

TS:   /error/gim
来源：http://hz.jinqigufen.top/gthwexkzxh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ywan-chungtsiang.top/gtuvwxijqf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuxming.cn/gtlylibiad.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangtech.top/gtngptcsmt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pengpengdd.cyou/gtsmijdbqp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.kuanghao11.cn/gttuukyeph.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hammf.cn/gtysshosnc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shangyingyoupin.top/gtfefmihef.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtodtcatfr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtesodjole.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtpwtnhevp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhengqikj.top/gtnekvlpfo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangkeji.top/gtywnoeace.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtnebhjene.html

================================================================================
来源：http://hz.0kj1m.cn/gtgynoccrh.html

J. 日期与时间
来源：http://hz.gzhubu.top/gtfjuhtzbz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtaiiuxzdv.html

[J01] 获取当前时间
来源：http://hz.ydzc1.top/gtsbttedfy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtbkrikcyh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtjrxfoggv.html

JS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtkfwnoldr.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtwdvpnkyk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gthkcsbvrk.html

Go:   time.Now()
来源：http://hz.ybcxt.top/gtndpucfdz.html

Ruby: Time.now
来源：http://hz.jlsjyb.cn/gttjmvkmgl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigfzy.top/gttcxmrybc.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtiptsamvs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtqsqmbojw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtbpvgyndr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtcsoxmnli.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtbnkznnrw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nwbrower.top/gtioeyaumi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtjrbrfuqe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtjiodpwqh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtknqdngve.html

[J03] 字符串解析为日期
来源：http://hz.jinqigfzy.top/gtterrqlsv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xziqi.cn/gteefnpaxv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.feifeiyinyue.top/gtyjhiqgrc.html

JS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtmlcnllst.html

TS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtuwmsacpo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtdrrnhxsy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtehrmmluw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtgejixxnw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtlexuqlff.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtzqfzwaku.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.316326.xyz/gtnyfffiwt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gthnespneh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtrsdvkyvl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gttgqrlceq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.52xcode.cn/gtlwtvjwdp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gtnehuzfuh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gthkqokmbz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtjsrcsdod.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtcgaxvijs.html

Py:   now + timedelta(days=7)
来源：http://hz.zhongyouzk.top/gttacmgtgb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhijiandao.cn/gtdesgvveb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtrkvhuzth.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtwgfifkms.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtjzcjxjho.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtkymholga.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yanxiufei.cn/gtyesdeslu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtvbmgjjur.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtpfdllgbc.html

Py:   (end - start).total_seconds()
来源：http://hz.shzxlz.cn/gtqercflea.html

PHP:  $end->diff($start)->days;
来源：http://hz.redwolf501.top/gtezehfukc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtivdoavqx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtyyxwvepd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pycfn.com/gtcgsaowcr.html

Go:   end.Sub(start).Hours()
来源：http://hz.hysaishi.cn/gtwgapeihv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangdashe.top/gtzxwckcuz.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtnpmzgauu.html

[J07] 比较两个日期
来源：http://hz.chenjidiqi.icu/gtthejdytm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtwhvpjauk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tanke756.top/gtckzmxpfz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtnipbsvgm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtjpurvpnt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jiagoushi.top/gtvxsafjps.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pengpengdd.cyou/gtqscrprco.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtosuublpt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtbaeanfig.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtuqdfyfew.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jyoumei.cn/gtenerdkjy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtiaveysti.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.birdmap.top/gtjsnzeqnw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtjvkxpnnp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gttnhddssj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtjjjyopwj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtkhgrkijm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtgygpteve.html

[J09] 时区处理
来源：http://hz.gzhubu.top/gtwfsqvwjh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.havefunace.top/gthulcvtev.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtubttfbix.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtjbteocjk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtlqtivwsn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aizwys.cn/gttjwiyfsd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yvedp.cn/gtmxwwwtxz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ybcxt.top/gtamkvpzjq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydjk.org.cn/gttymzbciy.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtxfnnapyy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtevdhtrgo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangshuangyany.cn/gtpeaizuio.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cqqwz.cn/gtmsewixco.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhoulong.xyz/gtbkqlgdhk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhiwuduotai.top/gtefbwwmqx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jiagoushi.top/gtbwethykd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yanxiufei.cn/gtumebycux.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xingfuxueyuan.xyz/gtkjbukmbj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjtbwxmau.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtzybadtqf.html

================================================================================
来源：http://hz.jinqigfzy.top/gtihztzhjd.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtitydbnjh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtbgjqazfo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gttsyveksc.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtqvrnateo.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtzvoxivpn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.redwolf501.top/gtoktrrrgb.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gtcyxelzeq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gttuxhhgfc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtbkgwjuzj.html

[K02] JSON 字符串转对象
来源：http://hz.316326.xyz/gteuumneoh.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtzyydjxfn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gtfjhowfwk.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtvezawccc.html

TS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtlpmfqeso.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtyfjwnzzr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtrtesaexh.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtdczyjzbb.html


<!-- 参考信息 -->