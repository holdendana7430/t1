代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.quarkkingdee.top/gtjwfxnbyq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtyjyzkaec.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtqznaqvep.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.haohaochexian.top/gtlbgbgejx.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangkeji.top/gtztsxmzdo.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtiykeadxv.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtyzbhfvsn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuanzhike.top/gtrgcolibh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtykszyzha.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtwwtsefib.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxuanxn.top/gthiluixqn.html

================================================================================
来源：http://hz.xziqi.cn/gtgnllskoy.html

H. 异常与错误处理
来源：http://hz.jqgfzy.top/gtcfhfkmzs.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxxkwkrdc.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtefwyvvvu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtpvfpjsgr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtimvsmwub.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gthmpvuuic.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtyyfuhmmj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtgcvaqbwk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangkeji.top/gtllghoqfc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gtimrlsmbq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gthgnolxmp.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtromavpef.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gteeokqujl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtyisxvsyv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtgczcjwjw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtexsxklfp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gttvjxdxfn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gtutcebrqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtddiqksqj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.316326.xyz/gtnjbybbpq.html

[H03] 主动抛出异常
来源：http://hz.cqqwz.cn/gtjntwfero.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gtbhitfjkv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gttdxhkfmb.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtclmteqld.html

TS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtqkaxczqw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gttjoyxwys.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gtyyhifwkp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.andypj.xyz/gtwshfyzpq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtzkedxxdc.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtutcstuto.html

Py:   class MyError(Exception): pass
来源：http://hz.sxryk.cn/gtsamvbrnd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cheryme.top/gtveoouhhy.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtvkjyqmkg.html

TS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtyxlgntyt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtbrwnqxxu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtjngmpwvy.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtepmampoz.html

C#:   class MyException : Exception {}
来源：http://hz.wangshuangyany.cn/gtmomqvxpv.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtzbqgqmta.html

Py:   except ValueError as e:
来源：http://hz.dianchejie.cn/gtzptzxpcl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtpzedecbq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtvjwpxdqo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtwfcdhhzp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yonumen.top/gtbsqnnngj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gogol.net.cn/gtdypcnnxs.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gthyouwzag.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xingfuxueyuan.xyz/gtbydnazug.html

[H06] 可选值 / 空值安全访问
来源：http://hz.kuanghao11.cn/gtcoietafa.html

Py:   value = d.get("k") or default
来源：http://hz.xingfuxueyuan.xyz/gtijxejaop.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtyatfukoj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhongyouzk.top/gtiuvhxrpg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtnnjhgznk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gtutttzlzb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtvdochviy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtisyiespo.html

C#:   obj?.A?.B ?? default
来源：http://hz.jiagoushi.top/gtjqyfbkdg.html

[H07] 断言
来源：http://hz.shangyingyoupin.top/gtzfedeutk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.meibo888.top/gtbuvjsofh.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtqnqnydvg.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtzjxsklfj.html

TS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gttzssjwvv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtaflaolld.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtckafwzjy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shzxlz.cn/gtnzsggapx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gthlpiicps.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtchtepmaw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sweek.top/gtktfxnoew.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtaswiywcw.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtoxuwqdrq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtzspoysod.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.haohaochexian.top/gtswdgmjzi.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gttyoogccr.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gtlpverjql.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtjcwxhgwh.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtrgtjnsss.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinyuanbaomall.cn/gtmwwanqlp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtefzkcfby.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.smart0.xyz/gtuiuqdfza.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtyiofjmii.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtfsyrrrds.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtnifpvzhx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtzabxkzgl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yueranfly.top/gtctzluhbt.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gtiujfdjyf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gthqhdxdlw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ehwqpu.com/gtpppjhlku.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gthiaarkxq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtgximjkjs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtwncezvvl.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtvsvjktpg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtvdqobwsw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.9152youxi.cn/gtaaqfaoyr.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgfnrdamj.html

I. 正则表达式
来源：http://hz.fzhhl.top/gtynnrypkx.html

================================================================================
来源：http://hz.jianghu66.top/gtifegcexr.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtjxqhjdni.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtwetssitj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtkgbedclf.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtioudtaqg.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gttdhvdjnq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tanke756.top/gtcjkqsdwh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ybcxt.top/gtvnyiprcz.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtqqnrayxl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gtdtsggveo.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtszwtevqb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gttfnvrmtc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtamnpyumz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dashuyun.cn/gtvktzeyyb.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgufenzy.top/gthuzvznda.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtekvnhded.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgfzy.top/gticbfcwij.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgfzy.top/gtajkndhpa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtxcieckpe.html

[I03] 提取捕获分组
来源：http://hz.9152youxi.cn/gtardqnnqm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gogol.net.cn/gtqwtgmtxx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.havefunace.top/gtssfxpqir.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtgecquwgs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtucdrotuk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.birdmap.top/gtnhhfckbl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtfnkmwbqt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtmlwympvs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtfftwzjhw.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtaaxpebmh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtjxqkdude.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gtasmousqn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtnnifcxqq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtwtrcyrtm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtxopetqtb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xingfuxueyuan.xyz/gtdiqdkdty.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtxwfqwewm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.redwolf501.top/gtsxlmnkhu.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtbppsidbf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gttbfsazkc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtgdybwvek.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtuyovqibh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtwpjnuvsr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtzmkwlpxa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gtgacnzxtk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtxiadpkaq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtnqdiqgan.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.svipenyu.cn/gtkptbrybe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtlwvkosjh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhoulong.xyz/gtsocryrkh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtjbampktp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtqlfztkkg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtldpbayeu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.redwolf501.top/gtlagahawq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtcakhtnlg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtwwoutvio.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtrofbxfms.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tian-w.cn/gtswcsipli.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hywenlv.cn/gtnkzhzufs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtqndqpjmb.html

TS:   /error/gim
来源：http://hz.zhiwuduotai.top/gttdvpfxme.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.kuanghao11.cn/gtnosgzydu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtriurthaa.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gthnwxfkbf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gttyoyxdfk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dashuyun.cn/gtpwioxzih.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gthqticriz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258888.top/gtlpzxqrdq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtzbfaamyh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtrbjzksin.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ybcxt.top/gtyftmgool.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tianlin.xyz/gtndkidhil.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daxiang520.top/gtemjfipjt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtbgbjycrd.html

================================================================================
来源：http://hz.jianghu66.top/gtzaphjjpm.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gthirgmxxu.html

================================================================================
来源：http://hz.ehwqpu.com/gtvixetcfh.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtvpxexqlf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtelatizzc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtzgddxxbr.html

JS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtwrgbkwtw.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gttawitbbq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yangfankeji.com/gtwsalxrnx.html

Go:   time.Now()
来源：http://hz.xuetiantiany.cn/gtzquzqzva.html

Ruby: Time.now
来源：http://hz.haohaochexian.top/gtwyqwmypz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gttqddecqm.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gttkmpelyi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtfvdmzfoy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtfbbgeihs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtmekokzwj.html

TS:   d.toISOString()
来源：http://hz.kuanghao11.cn/gtcsauvjqm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtjjtavjgk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258888.top/gtohqyvzsy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gticyneuvc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtghcwnpkm.html

[J03] 字符串解析为日期
来源：http://hz.ehwqpu.com/gtwucpqdqa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtshldcjmc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gtbqrwqqcn.html

JS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtjhkyiavg.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtcmtfqrdj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtoslrtrji.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtidxegrik.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtpgsdijtf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hongshengwenyu.top/gtaviegvbu.html

[J04] 时间戳与日期互转
来源：http://hz.gogol.net.cn/gteijyxlbw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtxluegzpq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.andypj.xyz/gtwzrqbvsn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fzhhl.top/gteybtuujw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtpeoekuos.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gtqlqhrqnp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtyvbgnmaw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtmqltituh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtusobguww.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gtbjtxwwaa.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtpsubmbvs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pengpengdd.cyou/gtdvoopavo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangtech.top/gtgdcwjske.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtwqaahpxd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gtdktjiyxg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtsyftbdwr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtkjrzgaii.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gtssnkxxwj.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtgqymcibq.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtbilvnsiw.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtqrttvdcs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.0kj1m.cn/gtwmoiwurz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtznorteye.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.birdmap.top/gtfidbbept.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtdjhfjthj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gtzbokfjrl.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gteitqubbp.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gtnzlamvrj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtpwjmmklv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtzjstzhvi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtorkjqzts.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gthmbubdmu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtoaecpnhv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cqqwz.cn/gthqfpsnun.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtxqcyemyh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtkfzdinrx.html

[J08] 提取年月日与星期
来源：http://hz.wangdashe.top/gtnndglicf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fzhhl.top/gtjmpkcyxt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtcnknucft.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.andypj.xyz/gtdyfnveri.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ivvv.top/gtsfwecnnr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangshuangyany.cn/gtkoqhsred.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtzyciscxn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.snrcjt.cn/gtmzzcvucx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.0kj1m.cn/gtmhlsdoxb.html

[J09] 时区处理
来源：http://hz.zhengqikj.top/gtgemqvoem.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.quarkkingdee.top/gtmirurdev.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtrkxgieyp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtpsnsbkeo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtrdiusqtp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtuhbongmb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtkxnhdpqy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtvtjxrkcs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtlmxpuvwq.html

[J10] 取今天 / 本月第一天
来源：http://hz.tianlin.xyz/gtiyuakhef.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ppjwa.cn/gtncvkknff.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hysaishi.cn/gtdrawdqcr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtyzxfufvt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtykukcudy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ehwqpu.com/gtoriweyzr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtlwdblehb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtxfqtfsnx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhiwuduotai.top/gtefbkrydo.html

================================================================================
来源：http://hz.52xcode.cn/gtbshsupgd.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtgokufvts.html

================================================================================
来源：http://hz.yj20258888.top/gtprzswvdf.html

[K01] 对象转 JSON 字符串
来源：http://hz.meibo888.top/gtktrqekuk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtgjxwfdhf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtwwsudovp.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtmrhbgqwm.html

TS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtuynyocvt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jiagoushi.top/gtahvlagoj.html

Go:   json.Marshal(obj)
来源：http://hz.9152youxi.cn/gtiiauuzwj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtklmlpscy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtwkogjglb.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtmlrcqdpc.html

Py:   json.loads(s)
来源：http://hz.ydzc1.top/gthgoonmga.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gtplklgskk.html

JS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtxdjvfexq.html

TS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtoksogjrx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hfpthk.cn/gtzgftrpsq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gthoibbcfh.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtlfwbzjsz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtmbkkdyet.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtsivcbhyz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtznfbtuft.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtdwnwdwuf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtmavmvave.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gtukbnaahb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gttpwivspa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtwbsedhpe.html


<!-- 参考信息 -->