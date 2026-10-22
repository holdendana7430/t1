代发 wailian999

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2prbiqoug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqtavotv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2esruilvl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrqjwoe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vpgasloi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzucksdv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pepfpwmw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lklufphn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2bgwicmef.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipwiffag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ohtckyey.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qpnhcnbt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xvpszuts.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvlxwiuk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eouwfelx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzlndkwe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ilxizfrn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vgyyzpeu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hoxyiryq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkomcwxb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kltffxax.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qjxhbnmr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2trqyhdtq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bhdszick.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mxquexlt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wbbtgeey.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xraisuxi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2uckheagi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jijdndnz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2eiglsryl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wkjbfuqr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldbppwyc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wsjglkcq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tchmfxrn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tzuvqgfe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2gzrppkep.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2canusnap.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2otemhswl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdqtcerm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ajqtrwtl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2alggmywx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kiqschsz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipuceyzh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssufkuif.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ukiiuuza.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yozngndp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2gvpnzmyg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wqpptklw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pwkwlzjv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jyruomne.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uusdltdh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rccoshta.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qldudcjo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2khxqtlvp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tnbpvggm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mmvvpsct.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cjlltwki.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gjridmwo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2otwxtlut.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zbnfmshe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2venrlptz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2osjiwycd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jzznuggz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lsrxoecm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hcmhsalg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2opypzqci.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rtauxofa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xlwizung.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ffbmwbmd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zluqvbcm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2cnrtjrrv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wmwmfkca.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vhcvbeeo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2uouwkwnv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xgiavguz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ycqcasvn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2iiniewcu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nvhaqtwx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2kilsgutl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsampwgn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kyaleeui.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2soswrbaz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ubuhjvxu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2sillwyap.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2erliejlv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2tzzyyjpi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xmzeoqru.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2unqndlra.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pvkohrni.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2atowrrxb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxyswnf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2azkeoonv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktdwukyw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2djbzfcvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kspmswsh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cpbgnrrm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbkmxopn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2icljpgni.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjiefas.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ufbueyhq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2onypjkzs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rnlmoqwy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ewhgpygl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bkumlnzw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eszavyna.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lspadbnr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2aiqtkzgu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2abafmaks.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2lwiezeqv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nhrxlcro.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ojzvuzap.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ztwoxgck.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dspheeam.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wqflchhs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xivarqlt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jjmnppsw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xwzdscyn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pazjrqpc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lhsupdmi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2exabwfds.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ckkpliiy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ywcisiug.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2avjcyccz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2rlesrjwt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rlxksqco.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jcqhsiqf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2syzwzicj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2srtuekzg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qcktljsl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2uhxulljy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sdqgyned.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2hcbmhuxb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytqsvoct.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rqsudfwc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nwrlsvky.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkiptgn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dmoedhiv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nregmygl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cigteczv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cpaoylaa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2brrtlfyk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ksyqqbsv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2hhmgveir.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2uuncpqtt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qpucyvsx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2milhhgvj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gsmetbfj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gvlfubso.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2txoggzxk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2voeoisrw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2jormxhnu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cjzukfke.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2kjcxksdp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2fvilgelw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2bdbsgkep.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2nrdfyuek.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2vegelwnl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2uxleeirn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kxkunjuy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xycnfnxa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2atjjvmmh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fbyebhoj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgqbgpk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zkcgrekc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ndblxrzn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kmqbkeqv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ywruahiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfeecept.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nnpjrycq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rerymtru.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2kqkoklep.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2djcqqqkx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zecskxde.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ypjyqafg.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gadgfyog.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qljlumzh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mkvndowz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2pzbgmfoz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2buyrjgbi.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xsgozjln.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dcuagmff.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pznlbybx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2xxpmvmzl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2qpxngdvk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2fldafibn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2acfkobjs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iuxcqagu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ezlzaaqt.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2hdlqpitv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2apjkroqy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2zfswalwb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gdtkvlwd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pxjgewss.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ocnxxzmw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fzbwrfre.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2utzsnpwy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2axviwoct.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2fddyhrae.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uperfdji.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hhzbtzml.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nahskudy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qravedpl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2wcifljfa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ecblkmwu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jubkduhd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ngviszth.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2pvebhmna.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bfqcvyhw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2mznramtk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2whzpsahq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rzovrfry.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2szygknxr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2cxzfdldu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xxuhrddd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gjybnlmd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tvupargv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wjbojibx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dajthmka.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2oyebuszh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rravvpld.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nizvadvl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2cavrynye.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ebifjjyx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2oxyylkge.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2jjyvkxex.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jfkrkxuq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2eihagbeh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nqjcvpal.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uaxmmegs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2hwycnfoz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lopkegly.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rixphwmu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2brrzcdhs.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2oikmejga.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yolqhukb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mddxrypk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2aqtfwgwc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2wkyxsyjw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2krglonag.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jkdeuwbh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2byngurww.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2vzmtejke.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ctxmgkua.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nqkxpfld.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2etonlhvo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xwjjdwbl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rgfexqta.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rofkmfgy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2vsjzsphb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2lkcqjsxf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2nbeafsjf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2vsnvlobc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdietwjn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2zrslidbw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2troksdbj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdwvaoud.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2radpwztl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2juhjmxis.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2uklxgdze.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfjhlnap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evudffsg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2gqyzcjsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffaetqid.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2azdbdqtr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bdmtrqke.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jekreauz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ripeiagr.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zudljxym.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rvyliurw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uibtfcgb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2stxqxvii.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xowydbff.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2limfclmh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrslqgx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2duhtjpbe.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvzhflpv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrlcufj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2irpbjnsq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2twdcowat.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wnommwwy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubohshrq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2hluiksqt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qsvmftcg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mxjdqlgm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jciujbjx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vcafkzfd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2wdfxbobn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qrggbign.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ynvzjuey.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jkgirtkn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikmpnfjc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ifjinzei.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ckoayqew.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dlizdssd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iextryxl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lkjxgwrt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2btktsifp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vepqboiw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjztrpwo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2dohdzqkg.html


<!-- 参考信息 -->