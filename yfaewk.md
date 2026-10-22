代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2diengwbk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ahhelvep.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sdckfxqg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rfvyhwff.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqlwfzgp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pmchmgzp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hjdsjfmz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2obykhdry.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qmixilqm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2phexmrnu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qkvbttkd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2axavezvl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2juurpyyo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jtlhtpbq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqhsbbk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2iurdugqz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mnnnzbyg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pmialhqd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2mzsnrwex.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ehozwpsi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ouzjifje.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lmsevxdo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sdqbqxlk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zhlijyar.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2spbdbpcm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2uteakjtc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gsfwoche.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ipdzgblk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2uqmgdogz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gzekiodo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2efwubikz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2djvitjux.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iubxmgla.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2lbitzdta.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2voojlivt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bjbbdaxq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uknigkon.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfekvxfg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knghzpzh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bcuwuana.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sguoqkfc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2zekbhpyx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2yqwpldmm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2beesoplj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2celyzqej.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ktdnuczs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2pscavbsc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nbhvgrkq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qwqzqjfw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ndugprkn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ihpcqcnm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjmyket.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qipgbskf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tzjepkhz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kghqpsna.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xfittvbs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wktxyspo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ocbpylvz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iuddiisn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ozzvqqap.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tyqglhia.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zsakrqyr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gtbyvlcc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2drlqmgjx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2hngoqanh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jlhbwlny.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ocayhbfd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2wglborks.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2yvwnhxuw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xtobwgsv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oxzwwcwe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2simqtuxx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ibfkrypl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mtsxqgfo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cjecxepa.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zwcmmhla.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ckrjnxzk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2erlnlfcz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bjxxkglp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kkxsybta.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2otqlinqh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xmnafwex.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wzlnccpz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ltypztwh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nfqmmqmj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2aduwhbhe.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eckamgba.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qdonahod.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2whvjfgbr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dkpwwpjq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zmkvzlob.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zxmyvqhn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hfuxtjzt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pleptpyl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vjihnowv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2xmevmrte.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2blpqeabw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nuyriskg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2mazvjfeu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ypxgezlt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2drxzqnou.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2astxkyiy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ylyylvzv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecnenqbh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2fquqzhth.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mslhxoon.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyijhhjf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nhozcgei.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hgvfmfwc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxqahbhs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2myrycoeg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fbwenxyc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmsdqnzz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gomjzvyj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ifcnqlxv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qouzcaom.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2llnhbefx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nzqwhlfa.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2yhkyosiy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2swtkbdci.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rqlajhuv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2kcitzhda.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2bkbebxrd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tqkeudmx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vrrdyjyp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2fiptbxyz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gfxgpvdi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kbpgjfrh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zglmodcs.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vswflpwm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2osdfdlsk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sllegqpv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eczprtxr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zuwtjwfy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gwlfznmd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mrcwxzib.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qzrikqbh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2hocrcrul.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2klexcjnz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ufqmmyvj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2akkanqxh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2pddysiqp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2uldxlhui.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pvtdcqsc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gzvgjltq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vcuohipz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruciyuyx.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuahlqrs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vwzidpjr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cyqjyheb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2imsgonnn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2whhrmqfj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jkodohji.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edzurazm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2cltibedt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2nwduilhl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2owrxhhtg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kpuagvmc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zikxuqjn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kvibqqzr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bkefczrc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pyjdmgau.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pbpksluh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rlkqblcc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mgusmigv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2naiswqyz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ukyqhjbu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywiyfikr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gckwuqek.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ojuyersi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2huqnnjsq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2iqrdyyhh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bqzrzazb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uzewcisw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2koiwsegl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zalnyrag.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rufvdqos.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xlxyarfe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zenzkhjc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tpaphzio.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2atmqezjb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vqgsikgb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjtliim.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttkyfavh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oarwxkzg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpabsulc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2mjaddrcv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqzzycv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wqxfkbxf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2cunnvdzo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ackortqd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2tsdrvmzt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ujoifdvo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vizsibif.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qtshfwcf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2nrlfguaj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cpqorjwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuinyley.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wwtwijqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htqwbhus.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kkquzfyd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qfbihitu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wykgiinp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ujakdsdp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aucqtmiq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2acekeeuz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wrshuymm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2idjvbdtw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ezpashxv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gkvgzhqc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2umnyzjaa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2somwnyjg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jxlhtgmd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wghqfali.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ilkwrilp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zhpkjkak.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dhnkyfer.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xonykecs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lbuvxota.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hwyiqnxz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzamlehn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kmxgnjcm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edtftugt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ihcicgbr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gaugmyxs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zlvfqjev.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bhmlktmp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xuavqjmu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zzbtdyhg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdrwmgmf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uthxnlja.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2alzankim.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2vvnwxycr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2oxtnvnoz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ogrpmubr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bzcfphst.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zqsafglc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rwdvshlk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kqkytyxk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xsyhzkvh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hrxdpjfw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oefcipvd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rrfvomyg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zbotwzto.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycwectty.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2auipmgdj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lfrezkjt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uromdftx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmfhyasm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgibvyot.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cchuujvp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfbbdjcg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dpvgodyw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sbpzzasb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2fmctnldh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wodozene.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgtmcext.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oslxexbc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ezyanffc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hbgpcsbc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mfoeapvj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ngqpjpqi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlmtqoqq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ipzjzcvj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ccgbselz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uzpenmvh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2izdftznw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gkvuflwl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bxybhjwr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qedqgfme.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nrzehdqa.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ipzpslyt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2sumovijr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bgvnkvai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdxqwvjk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdbfrdjk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbuerrvw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdyjyqfh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gacjqphz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ypjlmjre.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2brfgaaua.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2whlxqzig.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvkxtpo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oavwlkko.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xeoelghf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2psuryhgp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzauvbnj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qgdfoecx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wzbhpmjy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uujhvjkx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ajxlqcit.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lmqjkomd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vtpneqaj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2elhwjbqu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cvhxnvet.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhqfriwf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pjebqoit.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2luxtzazs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hnhfzhod.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ucaykwgy.html


<!-- 参考信息 -->