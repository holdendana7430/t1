代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nywtotgn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqedysie.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rtdrcdie.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2znekerss.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2irjazimk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ztxkmhiz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2agbwfkkk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvrnizxl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ozangjod.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vakkecmv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hnknvnsa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jbwdgoxo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nbxzgbuj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qspvejfw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2isonpyjw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hfjidbpi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ybpcgqwp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kkwakhjj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tcfajhum.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ddjffjlh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ekvdrpvy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2akmrtnnj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qopicvkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvwoppvc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nohiubzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymksvjur.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qdxaszee.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xooomdnv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocrsocbv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2regwsqez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgvjdsmu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwnyzhcj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xfkaudjz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2cfkuyirg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ozpynfxi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vujqbdrc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2okdxavyw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jwshjhjs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2azlhtlrv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bjfnjwzp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zudxuhfi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kucwpgbt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpgmgqvo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxzzdtsx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xvvfuaih.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2upbngpbu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jqrhezmz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dhhdwhmj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2otjkvrlc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mqztvpdt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qcjvpcsb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dascejuz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aijnvzvo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ztsflxmt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2enhdyfwc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lupptvpw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2prbelowd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gggossgc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2efwgegef.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pmardirg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2nujyxbwc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ucpuflcc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktzbuvqm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ierpcwoi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2skzcjmjx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjxgswmv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zvuaxpeb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyfhdrvz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ixtsfodn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uoerxoqf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ezavdipq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jqjixjkf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2guurifxr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wyvkbfpq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ynjmvqdd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2offtlaqh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2flmwiwcz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2fgziakby.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2mxhhnpdp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eqishrmb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hofqglcz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yyplicwg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aupnavny.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rqpnblud.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wkyxjavm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2lbbwdwoa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dcrxhvng.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2dkacqfim.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rjwdspel.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2yzlsgcsg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2szisryow.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jguundck.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2iasptxas.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2toqhjkfe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2tkjylgwa.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ewbjisis.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vdtrjbiq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zdjcrshc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hkymxcec.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2erbeomgn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wysrtfrw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fumqlewk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2hzsnilax.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2moanqjbg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lamdmnpg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ynthlgrp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2pffckpcg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xmzsjkkt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2izgrqhzu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2oegjgxql.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sinhmqnb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hgeelaby.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ofiaphcu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2feofmyap.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ckbqlitv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqnzzdln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kaxerbpv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2prpstlsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhmqjogy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rfglkxsn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2woqykuqm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2loaaywpj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2izynutdj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjlkcon.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2bznczwzb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xmcereeq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fhacgtsj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2squcbpid.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fhluxssd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bihulcph.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2luvhxwjx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2tyjqptup.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ynzirnhf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mentqbug.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fyybtbhs.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pvuimryn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xwpcsmdi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2refjrzhv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhmmwrf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bufguvwf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2swolaggq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rwkubyon.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2batkgggo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vpyjtlre.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2xzfedfho.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2qxmonats.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2dmyimfei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rcglvfzf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfpcpycb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lzcacsdk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnkjit.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cassijun.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ijvermow.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pmnjwlqe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mdialnre.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2hehuthnl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2vggiorzd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mijunjze.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zaibkhro.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2teornuwe.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hwaaadzz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2upxlbtuz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzqfzpw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2jhtuftaq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2aztzyqpv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kwkjqyfb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ejvyibve.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2aoiwprts.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pqlgbnpq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lvtdnczm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2qymksxzv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2sxotrubj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vodzifbr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2uxtwuomu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2lcnhiokn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2itlsboxb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2pzkckwcz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2oykpenhi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vupmitxn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2magbshty.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwwrcy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2fitholfc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ledtvuki.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2amjctcqi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qmdmrqpv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xmklxepg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2chjtakak.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rkbcnliv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2pygvjzrp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ebzrzavx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pjwcyssa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqhzicdb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2akstyijd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbjoozvg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jfhtdspj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nuultmea.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2khsoqdeu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2larcrlqo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bpopjaep.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lnhememt.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rtwjnhdf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ypkfhejq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2flwltbyo.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2giyrnarg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cuchwoei.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jqlejwaj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2pjhbldpg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zfylsqzf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jqitvlaf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2uycpzjsu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2yjkvqebl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2eykjjhbs.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ylalkwxp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xbcayvlm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bwxrajlb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vzredsjw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2idmvrfmf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fpsilrzf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2medpxrxo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qeamzsfd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pocfkipe.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2cavapici.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ooojduri.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2xjlnfnnj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kftlefan.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2izvmkoau.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2nvtppunx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2uvpydimx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xdnhsemi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2fznlujrz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2btchyabt.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2mpceicxr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2rxvmkijb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2yxmzqnoe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ixgvisyx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjfwbrm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2mwjipfop.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2nmnggznd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jixzoikn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2zvrjnxin.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qagtbynv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dqvzkbkz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2meysyzal.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2anrjnzhg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kxyknwpr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2gjsdxndh.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2cfzddoxl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2dshgpjue.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bnsuszzt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nbfxlajw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2lflaybnh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2osuvjcde.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jbnwuuid.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2npputylx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2rmupmjit.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nojqvuym.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ycadmojs.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2wyxtohvs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2lqbfctul.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2gysipdma.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2svgaoaqj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2snpqrdvp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2pxzfxwjl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zgcgzedj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ommrdgfg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2bxyzsntt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ggtsggvi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2thmfiwfg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2pkliaewp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tudibkhq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pmlqtdvg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2cwbtjpos.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rqocadtn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ceffwruw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qdykqwxs.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2hlyyklfx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2piccqoue.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ntgffbkb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fgonlkzg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xaihptse.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxoxnfzq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bksdisnt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2fkepaaaw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2pdbnnivc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yejgjmhs.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2uuqsqzkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibvjnhtj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwewvcvd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2enagfclv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qktwhrnu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvkspabb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2csixkfwc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2itumiaso.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ripluayk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2kiuyndpf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2aldvuhso.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lqrgsksb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ldwxnsss.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vmarlmrg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mojqshgr.html


<!-- 参考信息 -->