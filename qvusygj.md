代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gdntaijeg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gkspbhscj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gqaxbptny.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/ggthddamo.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gabnhtcwb.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/ggxolfubn.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmveqykwm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/giegwadcb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gmayuqnxs.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gynkhzyhc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gukqnczsq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfsdeoyii.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/ghjkhixjk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyrtixoqb.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gbbqbnesc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gwuauzeqk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gexntfdug.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/grdldfwux.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gtunlyxol.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gcofavaig.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/goqtppwzc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gkuzackap.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gdebtkupb.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgmvcun.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gwzcoekin.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gtbnjxygz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gjgwaerty.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhaakuiw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnyatyzjy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/glrbhqcis.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gbyzsobfa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gxclwfmer.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gtkkimecm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gmnnyqbdu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/giyaexevw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdbmrdmof.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwjbfwbfy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqtkaqcfn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gniljcxcd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gxkrnrtpy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gyzrophjk.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gkrvnqjao.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gprjobbgu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gjseeowxh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gwhqroqev.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/giwzcsaxq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gsilegmkc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmqypqu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gkxycaiey.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/getezwrto.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gaufxyyer.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gugwxbgpk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/ggqgxtdlg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gvtkxhiyq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gpoyufqmy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/guxvmswbk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/ghsqnfpaf.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/giqeuvups.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gxpxgyfxl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/ghzxsauzm.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gxpvrmsde.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gzckqgdqu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gkxycpwoy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gslwqlrtm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/giknvnkwp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/grpgehzpv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gmfnmappe.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gznahzmes.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gtzywxufl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gawzttvry.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/grypovurq.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ghgvrpcee.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gcznnbovq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/ggfqargzl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gnhxybmqd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gdihkucjy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gzuejrpoj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/glqotkzbf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gekcluedh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gdhyfumir.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gdwykicmq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gnginijyv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gigsjlqvo.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gmiplgsjq.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gwyvxcdbj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gplbtimdc.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gdvlveltp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/ggefcelhb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/ggeyghlhj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gzfchypny.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gvmytslnr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gqalilshh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gjkxcmuyb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gvelwuedu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gyszbmnbo.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/grfzmfbrq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gnblitoxl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gykcdvuci.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gsfdvakwx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gammmrtjj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gcybbhdzw.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gxrtmorrr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gvkhpypqe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcnmedozv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guyinsftt.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gkelnfbsu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guesmowyq.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gnkelptpt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gahcjgkvz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyaqqukt.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gawgqzfyb.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gidrknqme.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gdhyodpyv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gwsdsfsuy.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gnpnoeqln.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gjrbhzxta.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gbqqxlrrc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gdqdkjllr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gdtzlajlm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gmmybtyyp.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/glabbelvk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gxnybnrbx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gcuhjvhwz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gfhnxbvbr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gitymgvtl.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gigszjhqt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gmtpmyetx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/glywcsobi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/guxbyioll.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gytashwgy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gqzsfhvqe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gachriprv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gchmgmtsx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gzsxahttu.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/grnizxhtl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/ghyeolmff.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/guzeknrpw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ggmigjbqk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gddklmbzf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/ghetwidqn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gjeowkmhi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gnjlidweb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gsdiqlrjj.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gzepqogsv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gwbnfwibg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gllhpdmas.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gnpgrerqm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gftbebnke.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gcxonhxqu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gqmzmyepc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gkaaobrul.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/goduewxsx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gonivmepn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gwwelnhpt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gcdhjecab.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gfwwculnp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gkhziaton.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gpfwoalia.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gobqssgoh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gahrppcdg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/grjpjxubq.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gtbwkonel.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gmfszpquc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gsusloojr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gnxbhhyjr.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gthasonti.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gppptwfrr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gxkagoffl.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gmjsktzfb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/ghzirhraj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gntgafwgo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gechdfsao.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gjwloahyh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gctytmaes.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gdvffcjin.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/glfjjcdxo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gsbnbibpf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gdvhjtepd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/guhvfqsej.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gielsztmh.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gpmlkosxn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtbiomboi.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gnvpzjckf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/geblsipbf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gdyiuzpco.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gkebtckxv.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gmnbjnasb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gizsvrojh.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gjmftdzgu.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gkmhevwzr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gcmilsjxh.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/ggzsfevtf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gcuvlxern.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gbrbsevtd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gbakonrei.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gdcrxsqcc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gvudmnikb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gnrecwftm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gpmwtlfwy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gmtrzkqox.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gyjauymou.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gkauvrlbj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gilydpbvs.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gqhofjkgm.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gfutxepzt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gysatrixr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzyupfyi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/giestdnor.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gykfkwkwa.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gyrljzdvz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gpeklfppx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gbaexzkaa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gvtnchnkk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gyvvnbuel.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gisdfcmun.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gociayhkr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gfhemutfr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gcfuvgjvu.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gufhfqxuv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gkrzeomzn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gwgxtxewn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gofwsjbht.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/grrpcqoii.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/guqewlsbt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gsfkutrmb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gotferqvg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gplertsnw.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gxgstbthk.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gxjrolded.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gsezxtarg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/guqhjqvsf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/grgrfhttg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/goxftmcbj.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gtewlkcmy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gsdjaajov.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gruovcghc.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gpzxqgxmc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gfuvmnmaf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gewckluty.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gatvjnvoo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gtqrsczdk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/ghbmlimba.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gjozsojdn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/giogzedwr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gfbbvqgfi.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gkckvjlyo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gidxbppwq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gjbplofok.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gzdgxqmyu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gjreiuhbh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gprxceryo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gxgbnrbaw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gcvbvucxv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gpflypksl.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/giyizcjbb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/glifitwbb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gjmzbedck.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gcoxlxsnq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gmvuwtxqx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/geymgkfco.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcsrfeq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gvftlqusc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/gicjxxivo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gullhfuuo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/ggkldiagy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gfhancfpi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/goanbknyg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gpzhahkjb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gmajiacsh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gkzqpozxq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/ghciorgqq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvdfgauqj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtxakqxna.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gmwiqwfqt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyshavcyx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnqiccfuw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gsgrmgynx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gqpejrqff.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkjgbmaw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyjvjbvnx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gyiijudot.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gqxjijxyi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/goolhpbix.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gphxohcuv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gqrdmdlzn.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gkmmgnwgr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gwrfeadqq.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/geyuhluoi.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gbvjfgnkj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gyzogsidy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/guaccaiqc.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gkmppzpfe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gnngepdup.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gwwgpjxeg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/ghlrmwbvw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/geuefpvoi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gtglaiutf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gvblzxksh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/glwzscuwk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gratrbadx.sHtML


<!-- 参考信息 -->