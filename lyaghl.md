代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3veiptdeu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wnhuqtlb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3autysmsf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3sdljdckd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yptgxzfd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjlhvifq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpitklp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dusyqact.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bmrubwqg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mxbiwtxm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jjklxnim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfmngjvd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yrztjfpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avwzlhjj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3raxnimwl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cfspxxzz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3paiijjgy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrkqrrne.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sqdcfzym.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ogimpjeu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dxwtqylh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vmybyvqy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qecbnrjo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3csmxzquj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3fxeddmod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kildrbhy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gotxssys.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ujyhxnzd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qxmptnmw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yslbjyra.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3sehxcqaw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bmbnzrlw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jjzfxamr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3htptypod.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3opjgwugi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhrvaaxh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3htullljs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rzzdkcaj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3weexwqjx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nqzmyvlh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rhdviusi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3evnksycw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ivpcbthb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vvwatlkq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3igpoludv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqqsnlor.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zurzsyqp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jexaftgz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3aibbyokq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dphjfyvv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ncydqsvf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hbbqfuek.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3xysvmefy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cvdupyby.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fleklheo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ffmotpyh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3vwoxmnac.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3helvdfva.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbwlbayx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dqqpvqni.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3hqwqfgqh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fncqsfgp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qjeawfuj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wcczbvkb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3eshzfcub.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3gwycvfmp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zfhqqxnr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xlzswuld.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hebruolm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3baiylach.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3izykgxkj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wmpominx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yqtoplly.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3yxiqtjxq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fgwfgscb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3bwizpvui.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dredniue.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3irfsayzy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3hdbyfmbn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3wgnutvfl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3muxkrspj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tbrfzprd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rgebfprr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kmrfrikq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qyslgxfp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3esjwmnpu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3eykgclqu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dgxfdrfj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ffpkdzlp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wbpvrmdm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggmooexj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kgjktvrd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3irnxthpt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3mkzdjxvj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3gtuwcduh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rusvrhut.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3slstpzdx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jqwibchb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3btsyzmne.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fqfserdy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hqojaqup.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3mrmffnll.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rrsxtckj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvnwpacn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfbuhqgl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3uhzyjiqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csmmhcni.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lknwzsrf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hojkzjev.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eaufjmhb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftxqjofo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfhnlvn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3kqdnyswo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3npnudjkc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nwbinvlc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3faahmeoj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3elqelvih.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjyyfln.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3trsnxqye.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3taniwgfw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3hdljbila.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3njuglexh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3reafnmtv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ewnlmimy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bayginck.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3hbfpaktf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3jrqpdsqm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vamprkxd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dztxgoye.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mktcbatv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3bewzvpsd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vkgjadpa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3caqywicg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3qsgmreis.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jtqgfruu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrtieep.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bdlcblrm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3wuwogbwb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qnwdmdis.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ifyygrog.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zktbgbkg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vypdtstb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ttquuabd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sbcccfuz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqdaaqtp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmvlsupt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gcxlzvam.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3slzixlwq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3hienazxl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cohqzyal.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3yutvnjet.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3zbekmtbn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3miioncpc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oafndckd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xmugifky.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3uebvqlhj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qyrdntuo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ckcwrmof.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3hggsfdoj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ffudaiux.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vbzynell.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3fyirkvbi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3lnvmatbt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cilawvyq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3tcuifunr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3plnlxkat.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3txskwzxb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qddjydwa.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3fursktwo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3jmeoaygj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3waovptwb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3frhmbafh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nbykgfen.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wdqtmiyf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vbymdrha.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3birelvjt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yzxvmncm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvipoqz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3occnizch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xottwsdf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3dlfhpplg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcwuigpm.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3plrjlkrl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3lulvpaez.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3atjrrczx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ycjekrke.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cqblwbso.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3blqzrjgy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vntnihew.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vgaajjlr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3atrftwzm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3njteasjo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wtwktylg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kwdfwscb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xtpcgujy.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3hpoxzspj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3qwhwxqgm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ikhkkrro.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tbfjprhy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3yncmsdmy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ubeyymih.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jkoikiif.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3asnawfno.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kvhtnebs.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cwurflox.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3outsksgh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ucqyaxxw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ejmjgily.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xdhsehuc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3pibgbjds.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tmtperhb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3idgzkhxg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wieyggvk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdaswan.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uctanmae.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3tewcuroh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pwasuehx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pacltcmy.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3egrjbymm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3tcpsqvuw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3sgzgjgec.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hvofqfll.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jvbldwgv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vxgqytva.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tedwyosa.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3fzmpsmyd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bopjkjxm.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3avazbqax.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3gidurhpm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wjecvubz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jvebuzvq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ljbaoxnu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mdvewwqz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3dpqztumu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xzgeicty.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ujugrlws.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3pprirrqc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lxyvlpwr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3nxsmhpbf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dyddufgg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wcknlukn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3pwohzzkg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrueykk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yjceyars.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tecnytiq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fxhrlgii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3pcotugkg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ooybnzmr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3yvuzwffw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3nrntljjk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3jlfijefx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3izvfaexn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qownpkjo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ghnoogke.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3nzxalrwo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kcxjrxes.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3qkvzstiw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtjnmhp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bjyryujf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fivdifnv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nldxumoj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3gnzscfmh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3vvkcfufc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3egrhmmso.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3pmryejnk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3siepktxs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbnxfpwg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iqfcmwzl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ltbmjgaw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3gsgowhvb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3tqneljvs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiviqqsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otvlfeup.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jwjcsnqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kncswrei.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gezlgbwl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mvkoeshr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vzzifqno.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3chnptwgs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fqckuahq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3otthuxmb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aybtrllb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lzusslol.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qefnttcg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3nupknklc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlpahbdb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3myfbtwkg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wpivmuvk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gxyejjuu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3txbzybip.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdkymnn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3isuxpjci.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unhobuls.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3tikvbupj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fuluwsxr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jijpkvhb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ssumwuft.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ombdnsli.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3esciecfn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3nguyxprc.html


<!-- 参考信息 -->