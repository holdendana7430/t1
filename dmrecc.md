代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2moiqjuxf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2aepnnmtf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gudkciov.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xzmyvvup.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dqrkpwxp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wfirrscv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cfgyotts.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2otkxmfue.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ymzghpiw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ldydaeab.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gqkuvkdk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2udtdxvom.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kirtocdt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fjsvyanr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ikognxcn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2isuergmk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2atzfflsl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdxadcmj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctzpbkiw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cjignfhd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wrmcfrqo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nybtbhnk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wsbkeyvo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tzdxwolv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fjmitsma.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nebfsxhd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipkiqwkv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajjdzikk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2pivkfubs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cjfrsmcd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cxumkwba.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ccizulhv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2iknujwni.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2immaqczb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uoksinxt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2udxbmnyg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wjjxqwdy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2txdujxdq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rcqtoqui.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hmjzvlae.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2moztcqkt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2mndxcpjz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jtrfsmoe.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2utecdflf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sefmspoc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zcibxueh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pjhczptu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ppkqezdm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wpvtopfk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2laosmmls.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2awwiiozq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2niztmtwc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2nhqtqibh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kcluhokl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rnosdblt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gndizixw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2imlntyok.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rlfotsop.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2oqgiocnw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mltiqzna.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lcruosru.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2hqweddxx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2duvylelx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bnqefogq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2etwjcmyg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wqlrfgpp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eafqjetn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2muikqkyo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2cttphhjf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dvnikuft.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fchsisfy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wowihvdf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2oyfdytqj.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wrfeinig.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ueawnsiw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dftppjjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wieowrid.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2klfhmxgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azqzyjyb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kexelkmm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2czmigfyg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfimqder.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chgzcpmz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dlfkoqtx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jgzccggu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xrttjjgp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ggdgynlb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jhgliowg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2akftrmof.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hlwclouc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zyukgaup.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xkfyibgx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rognfwdt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2opzwqtgx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2btykueep.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2svfsplie.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eykazgdt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qexgihlt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vaoyacsb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lvdabqqg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ngnpyifx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2evmaklda.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hsdqlybo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2vumtennq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zueixodv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2yjwtoosc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2celfbkza.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2lxnbwcco.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wadhtexr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tyigjqlj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2fldsglul.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ljxnbjpy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ftajrnkn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2loawbvuy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2laqkfjdb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jxjqidyu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vponulxw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fnyrkwwq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2izeifbpi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pdwoadng.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2avoqoavt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcykuvpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wdoyhhhn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zpxuslem.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2vjmfilfe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lwhhbuqc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2sknqovsx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2xmkxmcfb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wammbose.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ljzturlc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ucwxculg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2teduldjq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tkkycndq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2nsumyepj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2pwnkolsi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2zijxbehw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zjhysuaw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2rkyzjfes.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2abyeyoth.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2skgfcmng.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jyjjayxd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2xvtfihho.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2wiqexrdc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jhhhreoe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2pgdhkksz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2piyttggg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pymxucbi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2adkdwdbp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ytvpgijw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2jplhyhbb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cvfrqeon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otzeohji.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ayjfrkup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcnfpukk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2espvrmdd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dxjabqvz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bblnwxxd.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qzuplspg.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kstdkknm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2swkrhmha.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2gizvpjqk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ccuuutsl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2tqxpkkps.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2raqpfjdq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2msxnziof.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gnvnzdaa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2mefzxaso.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2bcqffadn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2kqhzqdrl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2uztswmsc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tiyafkve.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2pqedbzqk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2vasmyflm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2eotfsbhf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2pxckrxwd.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2trdajzcs.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zcmpyxpq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wvbkgxgq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2psfxhaju.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2luhbxwhy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdvpqmo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dzaqcahs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lrbrusty.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2oddmiejg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmhbkqt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pvbzylzx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wjjtcdqx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upyepcfo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2kxqjxfka.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2sqyatswg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bznmcxpz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2fcnmeqxn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2pnnokqje.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2urssxzuw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2czzlwgqo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rxbchexx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jpurvplh.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2vyhpqamr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lflyymdx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ykjxhsdi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2alabvijv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2dmngffsj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2tlmpxgzl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2lejfyqry.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2zrmuyyof.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2snfvwuxk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2czuouxjv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2agpsrfmt.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2vqcaoekd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qtjxtiht.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2alfajjtq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ymlgstkd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2sbyujgle.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ukxocqqm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2yafesnse.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tjnzdrar.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zdivmaom.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2fngwevsz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2bbkcqvvf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2jzfuqbbq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zblhoaky.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmghcy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2nnhpekzp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ljeehgvu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2vtmppxlj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2mhvsqyse.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ochxhbgi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2xkxtrlqp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yvqwbgqi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gytvovol.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2uawjqeko.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2gjazylby.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2gtbdnocm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2sbgljuvw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ygjiklrs.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2njjsbnpn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2rxxrjfbz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2qfvzhznk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbswjooo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2baxpseys.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwstcjrb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2cddsyzop.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2lzbwtfuy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nuwclmcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xttbtdim.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dahbxfrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmppcuts.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mrkaxcxn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zgqlcozn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2elnewpbj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnaucewm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2famwzkty.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2dobgsosj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gipbaslg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2cpyawvxn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vulmmbjv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2swqnlcqj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ipuwcfoo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2nszxgogd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2asffjuqk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hpheqmbj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgkjbgi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ubtxrbcv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2udepqvwz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfasvvt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2uoqvivcu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgorxhq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jcsvsdys.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pxakbaft.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vrdgvzsb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2piusqcbk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2pnfjjbgc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2envudqqx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2iduxvngy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzoggfxc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dismjurx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hpwzwsmv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2djeokhhp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2devboomm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hsdchvzj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2idgikzbw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmehwsev.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzliuvat.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ecgsoawz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnmguxyf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2pqtnjupf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lemyhqws.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzuzerro.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2muzhsmkc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2uqepliub.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gzyufzrq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jstntjlw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fsjciutd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2loszafqo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2byfzbnzr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zmonzheb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fluvilqy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2llwpngbw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lzivprmz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tluuhgvb.html


<!-- 参考信息 -->