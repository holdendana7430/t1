代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vhnzzkqa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sijjhvhy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3igpqecgq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3lepcpljn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jeyakiyq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wjicqwje.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kdoirmeg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ugslheze.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3eldgbjdg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bqxqtmys.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3menrzhig.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3cecfygnr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bjaqbcev.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3unvfzmvl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ujamlart.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3imxtvhpn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kidogdgq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wfrcpyjv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nmburbkd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qwzddskx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ybwaxzls.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3sagmgrpc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ypaxkxsj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gjsmnabl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3umselsfo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3cusmksau.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3emugamgv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cxluueqh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tpmdtzrr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3tkzcckav.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rtjyvmhj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3usigrsfr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lfcgawtp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ctcozmxi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xbbcqukh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3pwhnwkoc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ivqtaleo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3sizdzatg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3qhtfteib.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ogahyaqz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3oojzrein.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3gqvglmts.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apfclguo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3imprrtds.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ebbcxuwc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gfexyibs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwmmecvy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zkmettnp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ffapfvpb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krxkuaan.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dmlssilb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cpoerwvk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3osseajfw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dycluzjv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpujbzgo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcimxuaj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3aownmxxj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yijsrpjm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cqychsgt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ppiknhqz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rwdyrtqq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3tqbjmbzv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3eteblxrb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jsdstvsn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3dkqchfmn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3vnvjlnra.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ifjhxdki.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vrmqluvz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3frzajxtj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vtwqsbnj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3lfebaefy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pbfamtqy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xykokroo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3pbkwuncc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hblyzfrb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3oapdmddy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gjeitmcs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3zlmqjnag.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3fpjhnwnj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3muzahfpk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pfcipxjg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vopmfvyw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xuivnyzt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3innmkcnq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ctwsekjj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nvsujcjc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pqststuw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vzvnajua.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bcdtokeg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ghwxfogp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vircwzwq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3uexiwcav.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sdnegiho.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjtdjrzj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rkeyjjls.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3badopzzb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3saqyxlbw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nbultbpc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xuddxnqk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxlgdrxv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jfzfcuym.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3aszpxjhp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3bfzwllmd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3bjoqahef.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lwlnpusn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3osmllgdf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3oggkilvi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3emrccrxd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3sxlaojjw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3jahjuqzv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zrlntsbh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kmgghodx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkyvlkkj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bsogxdra.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hqytjwei.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3baamhwmt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ktzkerca.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3otqztvwb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gdxztzjx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3srwyvtuz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xdanobvk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3aklwnjij.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dklzlcoe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3efjtrssp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhnqhwe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aedlfjzk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3sdmriiep.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3omafwcuh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3sawghvvq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vxmevhvz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3xdoodovm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vafuudem.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3uyqknlks.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jsexjdgr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3chsbttyr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3raxlqdcf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkznhzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bitwaaus.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qxdbmqeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyifmhox.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3zbqymijz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xdxblafo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bxzifjiu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tbkpzptl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3djdeitom.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qunbtjrj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ozyzsmrp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eilwbwbz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wfwmortk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qmzgpdbl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zqdilqod.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3pginqkur.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vkxkdeja.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3faceihai.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uihpnvoh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxjqbto.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3lvjqyciu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jdombyza.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3isaiarbq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3aqacouhj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3loxyjrmk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jgmxvlcz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vszefqkw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uubmrahl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mabdkkjm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3eenhyjgp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3izifoqlz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ywqwvovl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lreurpmu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3agtnvpew.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrtplyg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbkcwhry.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3clxuunfj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sjthgzgi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3gqbvxsyb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rwikyzhd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kjuicjfj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qtrvvnei.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tdehbpud.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ermeqzal.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpycglns.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnvylgqh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3easxzqhi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xhbsggwd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jsogmlrl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vjzrdtsm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yqbtxjll.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dahvpldr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3waxcovyq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yucfimll.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyyposwp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3aigsbpmo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rhdkfsdg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpxgkhix.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lckckbpk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltdghdob.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aanihgov.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptfyhvyy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hagawwdq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztalefcf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dcjakhnt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mztlqhnq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ugskwutu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3whqgxxuz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pqqpuwjg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dlgkphbc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3smiuypgo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zihbkadl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pzxvitkx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3biychayu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3witmyoxl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sybaufwh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3cnfcrmxh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tcuwotgg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kovnwcvy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnmnbzdp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhcgompj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gpnhauem.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jdgcffqf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fvnblwrx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqwkfri.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nwvceqdc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3plfpacci.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qikpdhhb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ayinqsgt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sakaaywq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3jyarewow.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3fmczcvkp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oucobjlu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hozwggvo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rrxtucwu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mmdmkhmi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iuscwayk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cyihthle.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3onznpqxd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xezdgadj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kytmkohk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ykkihevh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxaoasq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pssoquuf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ihypfuqq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hgqwdzpn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3henersbp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3suubievi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3goziydet.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ulozagts.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jwhmxege.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lemjuawl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3bddcuzcj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jkwawrdd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wtbipzmz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzzzkbay.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3stqpisdv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ebwpepvk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jkdnihgr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lytiowfw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3pjirfsmn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3doaqlkel.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qnpsptjy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jxllnnsc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrijzble.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbjmzgml.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aowefqpu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gnlrukhm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pskhricc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3elaoierv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3utxswpew.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jbruyaip.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zxfihxsw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ugbipsbj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zfqtbiod.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dirkzltu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3obnjugqf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gbncfydg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hrvkczud.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fzrdeojc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yccdkcdp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3krwqudai.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fnmipjed.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uhsxvdms.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3egtgjszk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ikzjmvdz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pvuboubb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rkzcvgei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiylqwnu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vvsswtic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvkmugwe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3avshqsxx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3adlookvs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ttnzwgvb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lzonxqyt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rmynnunm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsiwfxzz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3rffyivtb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uecciqhk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwrmhdlr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rinnldkp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rclgtljs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yfsekomj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cponczaf.html


<!-- 参考信息 -->