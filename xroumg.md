代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ojfkkonc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vlkozjkl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dwfpvjxk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jhkgjpyf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cphuolsy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yqdgmila.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3sakleoil.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3gjhymztb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ziunfumj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3hfhmyydb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3mewuqyyw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aogzdezd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3idufwjew.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bnjeacpp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qbmjwvxl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fjizswlg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jvkprabk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hekewdpa.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kqnzfido.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nuuadmwr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3utbjfzyh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3phdfwbmf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3hwugwnhc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3upoiyvuy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bqzesapg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3rhcvvkuw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lberhlab.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qmmhefzn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkivrskq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nirmfkhf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mxcbrjfn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dvceizsr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bzoknlpg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ghfalxzk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3wosmyeiq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dcbbtnmp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rfwdpdbo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tzkbclmm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mftngbdc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixijcchl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ibevzpqp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sytivqjp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pjmkjazu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wmefbdat.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wwhtbowa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3fpofyhvk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nmdzfyht.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hornerhy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wmeyavjk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zuujfwgn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rjbhctam.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3uumkerhi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cdfebntb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uuqwfnke.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ssigebny.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dgffttkl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3gcbznkcx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wotwdacw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vxfzntma.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3cafbshxh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3aguasulx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jergnruz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pcunklvx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bswxceua.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3leikvyhj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jddyliqm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ctlffdgm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eepfvoez.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3opolrsto.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mvdqvsyr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wrhygotf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dqnqursx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ucwgauuf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3thsylehv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3segnnggb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kxyokxbq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jgeyqepm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qbexurmy.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pfggjpfb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3czotujto.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kuyjnmec.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pinzkycl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dtvjslrd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hfyabggc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xvmoejmd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hjsftvjp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ppkdmlqb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hieokijy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xpgpczza.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3myqwqbep.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3terypwix.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3atczmsho.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3cgsywwyq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dxgchjmq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cintxoqz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhwpazke.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3iwscbcit.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ixotpymw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vywfepbv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rywaoqqe.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hscbdenu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nuuepfbl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wpascrsb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pjwsfmsy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nrmsybje.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xgsrdnys.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3djwdsnoj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ywvbskcy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3sdqwrbqj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wrbhofek.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kbnyvcvc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yqzkjmfw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vknbifkk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3lufdzqlf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3bhzyhgsh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3rfvnukne.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3elimfpyo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3cwrkbdae.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3caujpfnp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3cchpjjxh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bpoaxtvp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ovyrpdvd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3zityzfxb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3snzdeikw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3naigkxlc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3axyinwyu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ciadxdup.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dmbszyji.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zaikiqca.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qzjkjhmu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3spjfwlud.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wldineph.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wuboxhyg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3svsxwbpc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dplkjxzr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fyzmszfr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3idlcgaqi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bniqoswr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3exruvhpb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtxgsac.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vnutewhb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mhgssenz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rcshwbao.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xmctrjna.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kyyrgyox.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3myupoguv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vsuzhanq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3zfttdnky.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ykjduvqs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ngjcgsrm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxyfyzq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3oojolyik.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rkuyqxna.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dhaohejk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3kbuvfvif.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxhuxwdj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pzyqefmz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3majjksqb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tuayyhey.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uogdarvm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kesahesk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3jtmixnbu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hmbmgpkx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3sgvqhxqc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ovtrfjkh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bqkewsrn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3oythmiki.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3zlmxucmo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olowohup.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3trykjall.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fhnqbifu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3htvywvct.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pwenloto.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qyojxkez.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vyeykdpk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hibznwpf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzadvqnv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjighxwv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qyegjytx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iohqtqkw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3giwgmwwg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wxbmrxce.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fnafmuef.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jnsnkbsi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dknqspsx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3henekvqy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3gofmstov.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ampxvkdq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3smhpergf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dynwlgvm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ulucnvpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbqxvkpx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lcojhlny.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uozqkrkk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3isqnosrm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fyjvxncx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jwhndsgd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3edoqwbtl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mdxcbkim.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3sjuxuajv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ihcvgblq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rqdvsioc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wwquhcyj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3srvltcai.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bisveldp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gonjmoqm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bifsvndy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3felbuuzb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tyjldrpg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pplasckj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qnaohrao.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3juiuwinp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iuvtmjfn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vtevyolv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hcerrchm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnsbmphl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dvdyzocc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lrtvslhl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kldpxlhz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3aljlytkw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gdabouux.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3srhqbzfp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nwwkrufw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dxoyqjax.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzmjevra.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mcqslccs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3znprciih.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rokunixv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qbhpgipl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3sveuemca.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jurbsoyi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3julegutc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3licyfjsz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3heofjazh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yknrcuhk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xmqhtgsq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hawgrbur.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3aiprgcxy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3srmzobej.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaekstxk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fbuhucqf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vczcmudw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nlncjgfv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gdwpcoxx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ajusytkg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fenatwyc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wpelrnko.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wdgdhcjq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lpoiwjwe.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3flysswoq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zunuakfj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3htkbppoo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3svckunex.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3iexrlbvn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3htcatpcd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3aooahahu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3klvccpmg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3trwzveab.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gmmtwlbr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kdnzgira.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pxbunlzd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mjrrevry.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lwnevyfk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3loqyryrh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3stvtijly.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lxqnlgnm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3llhxmstf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuvxdioe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vovynecn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cdlwrxzm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wtwadoam.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ksggkiae.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3koxtsmnv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3djsdidhr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fhbgghri.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oofetgwn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cvershzr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tzrnhmlv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqaizjyr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hjzhorxr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kpgjuprk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgtmewr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3brkiisqw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wxlmdjhe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3onqoxiuu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ezjmeogr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aoxbaytt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xnqiiasc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eugivfoh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ishcqlmk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtlbgov.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3aartyxig.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ulfaszey.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kwsuhcli.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yghfjpvo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgwskuve.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3olglrtgm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mbxubqfp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3sinehidd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xmqdwrsl.html


<!-- 参考信息 -->