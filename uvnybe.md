代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2excyeixb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2eedltmrl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hgdgqjsr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2tvoeynsm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qyyerkri.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2djwqkogm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oqozqvxi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2wjactsvm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2whcxqqxe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nulgkmco.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2emlbdpea.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xvvhwseu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pibyjnit.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ehmwlygv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dutbmdxq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tckfssuw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2xtpxrjrv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2omjnxong.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zukpcjun.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pawqkuvb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lzarhqiv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2gvepizzb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mzlwpsgf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wbirrxbj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qxxryjjo.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jbtmpnpj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rzmgwayk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sdtjigtb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fiffdklo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wepopcdd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rnnfxcye.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2djslerro.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yumsxmdz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nigoxjav.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dphiflgs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dezualef.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qqhqjnov.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2cljiuehn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyjqabcq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2cwtwwgun.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tebrcctn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2thrnqelm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sunqaiaa.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2xekkyxin.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wtlfzmpc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbsfwlnt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2njxyfmyt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jcarxtza.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2agghxvdd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjtbdkfw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sfzrkolb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkfilzud.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dzuukmyx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2udtmghhf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gahtxeey.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mcgirnfh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wgctuklk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bormxxjz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zsvveykk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cypfachx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ovuislhd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rlbafncv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2aincqmah.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rnwjdnih.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eicvyclv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2adqzjnrw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dgshsbwm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dppebidf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mwdbhtes.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2snusnbqf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2cjuxwmmg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kqoqlffq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2lcmbxsos.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xlgbicco.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gozsjqmx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ylrhvufw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2crivefla.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2hmnxsmtt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2bbwsbwlo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yeecnclz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxlucpol.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vjmqalom.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwqgwhre.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pdcnojtt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mdidtgxj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vizcnqdo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iiriyvgy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2tyqrhxpg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fqtmyubl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bcsvhlag.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jnzgjprf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rwsxcuby.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfpdudum.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2tfqbekwh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zszuhreo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ddkibkrl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2klihqtma.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pkcukyxe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dufibvsz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qswraztl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sogrcjsr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bwhumxfg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2chmkvpna.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tyhxeczs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uyjrkqip.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tizfntnj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qvhzctsk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2pfpzldsh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2eerrbknf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2juckhlnr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uqaiause.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2mhyrbgvg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lkrwkztl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tyhedthq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2smybhlui.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uwihhzck.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2wnlhksqw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jbufxqtd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cqeuddvk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkfyszu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pxqwfvuu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtkruij.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ojleufgc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ioercouq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2encutweh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tluzlzdm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bfyrtnop.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pxqasvyp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gedojduz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2oyjgnxej.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmytgqfe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2omrvarhz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tngcdojr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulesxxww.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2tdaooerr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfsnwllq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lvwqcllq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nsyuxatj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eohmwlfp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ogdicyir.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eucvummi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2srlikxlx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gvzfngst.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rwvyyfbb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ireplkzx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tfliywuj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cwwjhrri.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsccxnae.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hrwoydne.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cwayuxum.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jjxhyroq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uemcbeos.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2iolijbcu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rnagvndh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2zhteekmq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mipffwgj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvkwjsck.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcfopdie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oacsmaue.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqijxwpm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2afaljsdk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mrvhaklj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gsjehqcn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2netchkpr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpqskrq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvwanwhy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tafukein.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mfenlsoe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kstjxrkc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jqbqznac.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fzgrgkxf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kehwpxtp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nqvnaszb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fqyayuyo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2sehcxebs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vghcsnxz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tjhifftb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykhetwsp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pdepkebz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pbqrvnhh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2imhzcpjm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nrwclwin.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ehzxpkdh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bumohqdg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rdlrqviz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tilsdqmv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjythqce.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zoqdrtzt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dfygmbob.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iohmneht.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ezgohcbf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2beienisr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bxwvbswp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fnlsvfga.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmwvzyi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2upwhfydx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kpxbnvat.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oazumxuk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ybnbgmun.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kwpvmads.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2thwydcec.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uvnrqfuf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2doelxjga.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fjmpjnzv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nkouribb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ddgdnias.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cnygeptw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2veoaatvv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mtakysmq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2snfjesqt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wuteeizg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gocjbnaa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fadojenk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oitwcwei.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mvghkwey.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2eqjmxyle.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfsajtbo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2npuajxqn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oqcwqyeg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2inmsvsoy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ewbedwsp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mrttpath.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajyzvfgr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hacnkovh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fihsacic.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2unallrpm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2krelcprv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bnitxoxb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zqkvucqx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fihykfzt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cmggutoc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tvuuwshj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2osrjvuec.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vmdrmxgc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ywpyxxuq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xrlrgzdh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kephbobk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vmtkqerb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oiwwmcat.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qlmbghcs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sdlqcoeu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hgaprzvg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ouujrbrx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2evcvrdsw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2fehrbrxt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sfuusjhr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uurczzxr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2htiaxgot.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edggyjqt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2iyntaypn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xycxvvbe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2noiiaumn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uzgiykou.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2kzffpqrr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hblmimro.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nibfunti.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wllcepwm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cypbvtny.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rychsyfn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hgqlejvl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xiuafbbr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2varykiti.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ojrhpnjk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bbnvwoxk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tqwameyh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2udzbdslo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2haticowz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jnwpccqt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ilrrrymx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ztuczvcu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bcbhiupg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pkkuatqq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2siblwhsp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2svcnuopd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ezpwszci.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qlyumxsn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vgznkosg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mlorduwp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2weqsrtic.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zbovtzxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuxsztko.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hgsvhvqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncfrnbix.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tvsrohoj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vnigfxip.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crfjjbpu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dengcuyl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjnsnosk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryertequ.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lggfxqik.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vvsmkbtt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eaehulzl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbakwjjl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2utiplzwn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cnczqaxg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kzqpchtm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdnixooz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2acsefqfn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ddvdxlkv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zxpichlw.html


<!-- 参考信息 -->