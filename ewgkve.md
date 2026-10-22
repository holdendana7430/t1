代发 wailian999

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yaxtjvfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nujaihak.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2pswvhiul.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fvahxuqy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2embvwpbw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xebzdohu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbvpoamf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gkkuvcam.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qdlkysfv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jmozwszw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2niragjxx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pugxngrg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dyjcocpv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cnwtymgf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2njggypts.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qqegfrwh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsvtmooe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xwhnhopv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fycnsozy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vctlnxgi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wseutyki.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2otadajiz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zwwsxaos.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oinqrbfc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fayzsdvg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mctumcfr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hxlolkdj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vkzmqxau.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xkeomqhf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2uxnkajwy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wxypuxfk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cvlhkapj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rjqmlkpc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mptlduea.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jrneaufa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2owvxwmyj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nwfjghze.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdpshjyh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxwrdqsw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2rgifhfbh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2bzxtogkc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfnfwmij.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2npwbvnqp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2juzysdin.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xivanilk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qkvqynoc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oytorjen.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2sxwshaou.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2notocsro.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lwhchfmq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2umbwhpek.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2frvxvzej.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vjiguyxi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ksknrtzp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dhgjymcc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pbznxarr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2wqocxcky.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fnaxahfv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rqbppiuz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qdgupair.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lfkjdawh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2sdpyzglg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rmizepxu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2rkirepas.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jrcvmtte.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ulficwyj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hxhrxzgg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2asxgwcpq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2nvmilltr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wuhjnlyf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jejqxbdu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2nppltgkt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2uxyvhdct.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nuojswdv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2frngmtro.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2kemtjzay.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2efhedfvj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2tauhgyde.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcuwxaj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tdksoxxi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2alhbclvp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jobmgzfo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qzaodbnq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rjebpgmj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jrmyldxt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ocounkdz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2poiifbmt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qksfikdt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2bkbodbyf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2apuwixzi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2cnuqlwtt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujwapvgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pytdwhov.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2froqbxmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtjisjwv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bidjqwhq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqvnxrme.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qtaztjfg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zszwkbmk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpywdszv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2shixfyaq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2orrweevf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lrzfwhdm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tkannppe.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mbcwumbw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jirwvzvs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2snekwlry.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ekcyptrv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hhrmbgzk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tlwpyedv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jldecpfk.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wembtxbm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qhhuovkm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2diztkzse.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcenptbv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mhpxvkbh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2igyojddv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xlvqomfz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2azqbdfui.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2skpauxmt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vadewgwc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ypwkgxww.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2rculaami.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jiklwijf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tkhwgayz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hfahxbry.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qgadwtkh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eejhhgye.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2whazlper.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lqbrgrjw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2adkhmygl.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xvvoayur.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbdgfseo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zohwlqbe.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2npmqetgt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hvldvgbu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vxaeyyvm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2evcvkzfi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sykfgero.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2drlvpdki.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wddqicbk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cvxzitru.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2eafnfudm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rfnijste.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qmaqckhu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bxhowwvo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2lopmnqvz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2oxmryazi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pkyfleob.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qljwniyq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2idvfmagm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bqfhrdvd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tjuajsbn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2uptnmhak.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2issvartr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bjrortbn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2kmlcbonx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rbjtinjb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2iwudmllo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2niiwkhpo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cnfhafwp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lqstylms.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jyqwmqxm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xpeuzwet.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ocjlrgnk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wdcsjjed.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2trorgiwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgvminai.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2tbatrypt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlkvdave.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2oxkoayfv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2sifmfrnz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bubhmekx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2uizvqsqc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gykkuelx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mtfftnmr.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2shtqqssq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2wpozbwcq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2siddqtjq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ymavljus.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ngdaamhw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tmxqksbk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2tvewnixf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2hsghltsx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2qsqssugx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2glgrysfr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ficchlwa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2lnsvuuol.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2tcvorpqx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2okbuhdss.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2zsiwkepf.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2benmgzsp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2umlaewwf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yqnmvhqr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lncjzapo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ajkogjtb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2evitovpx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2cjzbzesa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wpespaam.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2tzvrvved.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ukgsgzia.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ahyhmjkj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2cqaachow.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2pjtrqprg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nznfarli.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zxifoenx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rtaexjga.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2qqqmpmzb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2txnpnlof.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2yzukxjji.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xcuviyyt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hbohldqf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jmgiejlm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2rgswfqtc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2oclkzobg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2quhkszkk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bjmawyyd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bascxacv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rdzhjwah.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2tcouzvmo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xixbgfnn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vzojezpe.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2mewjhsow.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2tfvouitg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2rghyzykd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ubuwqzeg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2upiegkuz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2nyzenatb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fhpukfpd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2yapwyeki.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2wthtwskw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ldzdgfem.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ztytdaae.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tkvfmgqu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lldmsjgr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2prnhjitj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ypaogaef.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2slinxpip.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zluxkhim.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2dpajeotf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lpocmegi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2tnjvsmnv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2gddzvplq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cwypcbsl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yarefdid.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fnckghly.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cjrmfitq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2svydkbsf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2duerdoan.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2tstgmvdt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2rjvccpaw.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ysfwvolc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2mxuuflxq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2emugkxyb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzxkbvza.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bnkxdqih.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpqvmjtj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2olsnegkb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2mjhelzgo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2grvdnmxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqdqmtdo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2lgphhgyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avgbgsbm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2owqmzdyc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdpjfhg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zzxmkvcl.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2irfgokxh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2knhewzhc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2znjfmjqt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uaadnyys.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2cewxzqep.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xldirkwz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2aiksvefo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlfxowd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vvcektuy.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2panstfro.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cprshefn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nlkvrsve.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wyxaoiwn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cxqefptk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zydcgiow.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2iszbfvkb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2paqhrbjj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dwagbcok.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctyrofwr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrbxwxh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghtbxazy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2cdnylkat.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2sfkwgwzz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gvhoprjr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nfjbesvp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tvrvvinx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qfazuhza.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pejxrfvg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2avvslvpg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wyratkff.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2utjriopk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2suuvuksh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2snvnftuf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2cxyjijno.html


<!-- 参考信息 -->