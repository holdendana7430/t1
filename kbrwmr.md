代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3obtigcts.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jrfhtjzp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vzexvzhw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzbkzgoh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rqvcbdfu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iygsobwq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtmeimq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ivnzdfaj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3oikjeizx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3irrihlbv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fnpjoujw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3auaorura.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tywdfyoy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zcadxhuo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3efldtnsr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3iomfnhbe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mlsopmyq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zjcwfxtz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qvcdrdza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbmlbblw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hdhitmey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ziuaozdq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tmxjubnk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hktsunkj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdzmtdfb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vwoguhfa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jawlzidm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzfftshm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qvezbehu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3smrtugip.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpieuqaa.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3arpohpfg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3irfttoll.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3faqgwcld.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eirwwwwm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kbywphof.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lfllblls.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3buhrfhpe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xwigwawy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkxssbir.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3swtuhotl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rjuekxdx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gukbumyq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3owiminrr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kocdmtou.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wschedxt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3knmajgdx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3itlxcsgu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3arzxpfic.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3phsgxzas.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3slxscipn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pvoqhfkk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gxmkzbmz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zejrkjrz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wciwnogy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jmqydifu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfofddbf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mtlugbtr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lmgbdwzf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jrwjnjqn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bpydrvyl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuueofwk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgzeiiak.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3iastbkdb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hdmtssgj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kluamzfl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tqkatyeu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bchaglyd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3mpsqvash.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uebtdpoa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rlcackvu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ndvetcdw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3iflcbpsv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cvvdyybu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzufqkob.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qgchqhvg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xrvpfkyy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nznzsuwa.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dnpxjiey.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cghbknbs.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cnfcidng.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3swtsiywx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uqgafgdc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3oxqbkiwq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3altfkifn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xumoppqd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kfnkfxbq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rnnltzom.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gdtihgwa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxkitls.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wddiynrt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qbkpmwkl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3fwpfcoyu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3tpeqdtiu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3awyvdbwn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vdojjvod.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aysyysxu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ssbegfjz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pralfras.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ejxutven.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nfwbnbuh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3sodujyhq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3hrcgmolw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wetcwtmw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ofzeaqol.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hzufqybh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3czlfxzza.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ltzjcwjh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3avrovlwv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3baoclnyu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3csrpdyet.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gamybxzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rirwmzak.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3exgnpswy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olmjbvxb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3fjgfnsvw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3poxzuhbw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yzqgofvp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vhamissi.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hetpkzyg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qfljacea.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jnlejxfx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3drssmxlg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ikxsgttz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3cmhgkuqd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xtpeqzze.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ehohxoas.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3faachzdm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3byydyffg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3suwojzco.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ivnuwiob.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uqymqlbo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kahdhfjm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3cprgdleg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3dtmeiimc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3lgxidalj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yedyoxch.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pufavtsw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3abyaxpgo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ibkefsgx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ofmiafnu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3kysnunip.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vjryffdt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3itrnwvtd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbuavxuj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3znurkesi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jwfwagtw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dtapapjs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fgioswso.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uufjugku.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cbqyyxtz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3dprbiznc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vuyhhtug.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sawesrsx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mlqvqtep.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hrssfvyh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rxpyfxeb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ffgqmrvg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jpmtxeqd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3phiitvlf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3anbelnop.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ablwhckh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3znekmptg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3btarfkby.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dlhjlgot.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mkdvpsls.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3mquwghli.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3dqexsxjv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3teyctqka.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3yqwtqjaw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3gjoqgufb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dhpsgnfs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3hosxvkir.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3pountyli.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3fdkkfelr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3hgirhaee.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3vnrfxzqz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ikpcrjpp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3tekrjvue.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qhtjyllm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3okeutjyv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqzfnli.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vjpeueny.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dmchltio.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3tejwyrvu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3jlmzetnh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zghhxlso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgcadrxs.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bzbsyrya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slpgcysx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gmzrfevz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3znamnimt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3dxibljau.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uorsdsrp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mzoklwzg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yeromris.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ngsfnnqj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3sesmiftg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3yjsvvnqp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yicikpbt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3osfvzaim.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3csyidcet.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3rfawkniw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ojhybevq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zujshryx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3guhjkudm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yjuvgcol.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3eiocqdhi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3tgjoqxlm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3rajvkjnt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3fqtlvond.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rqbzkouj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dgayhbeh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ffsnbtbm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wgdtdlgl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lsdoaojd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcowahy.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3icvtqmyc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqhpiww.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3vidhqmvh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3kplzdobw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fizzvvpr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3adkchzne.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvzvqea.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3camxjkpx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ejrlvnnf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3paapvgfv.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3pyumvosl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3vmpplaef.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qxkpisjh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rqjkzdpl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wyiuectk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3dmkqxrqx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3conbfzla.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3wbtvwaml.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ieruauih.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ohvmvreg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kozvkgng.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3hwthreia.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3vhplltac.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vavpwiov.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ktzeldxa.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3etvxmgzn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3pilbznqe.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3whamhtqb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3igdjxdex.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3mkbribhd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nwbuozyy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3asbuixqa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfjtpyrg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdocfhd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fqrjwttx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3aspfawdt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3mojcnjbx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3kwxoluek.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3lmyqpxbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3awbsdrcd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3abeoxicq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3lbtbltlc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ekphpojl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3pisljeuc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3dprrxxic.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3fyiryxoo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3vxspkhvt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mizrimim.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3nilxvizl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3esuivnbk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3sihdnffz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dadqtbxp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xocecolg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3iizzznah.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3iemjqwie.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdtngyp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kirkeekh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrryhkxp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nhpvnmav.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwgxgcv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vlzwzkea.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3objenvtl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3affysdrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puflbzhh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3jphssmkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtxvulol.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dehnllnd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yfgklfmr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ajcnmlfb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewryfjjp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ekzablgo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3odoggihx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3nfjpieom.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sznnvjxj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hzdwvnym.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pfpeivbi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmkurvqz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3etuozeyw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dncjljlm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjsgkdn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqhipbu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dqakvwsi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtbwhxw.html


<!-- 参考信息 -->