代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pyjlvihj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qxzrqucn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xihvnpxx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wshcaclj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bcsuxdjs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xqmfnlue.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3akraihnd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ybitpfal.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vahsuzwq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3unczyqwq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yextlviu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rajntahb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vqdtzepj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3edsjbvvr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tzclqfpu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jwpwklgx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bzpuwbaa.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jdzvmohs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3spztfemj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gikvvrvm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mjqgyvsc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xjjjgfiw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ditgflac.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eqzjrakj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3yjlaudtv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xvsmrjlr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xpsmmieh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3badsfrst.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3evchrcdg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bfnlxegz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lkjltsnm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fgmsjqcz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gseuupnf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3krerwwrk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yogbhazr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bjyuyrou.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3npmkoecd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zrycsite.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ndsmjtin.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3bezcvdot.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hsxbcdfg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bepkuxxg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ngxzaqfs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bbsmlpnr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hgjtvyhb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pcievsdn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foqtydiz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jigmtknz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dbwzwcbq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3igxamddt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlqtmlpp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3szestpib.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ajbpmfws.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdjibfdl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vglesdlo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kwegpetl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nzxiiqkn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mdvxaxbj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3whxhfcag.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3svazrysp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3bnizcgkq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vvreyyrr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3umadzess.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hmafkjtl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mqminshn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3sdziobrv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hvcwfich.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wtvrtfvn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ftbjivra.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtyayqyz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3scpkhxau.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xgaxjjpb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kqausykp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jijmaqkx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bgnnpkva.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ppksvueq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rjykibhq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gcxcrybr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3peaynpyt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vkxocqnw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3wjnrffgs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ovmqtwml.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3cwfdqtia.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3sribesyg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xbllabca.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qfdktssf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zjbumwpa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3yqnnqrxi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3neivdyjf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jcgndddh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kqinuvlz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbhdytb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjyftzq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ctmtlaom.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uqpiodub.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3exacuscw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ucjaokdo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3zzysfpoj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3cuarheko.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3drxjblbw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3okchbash.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3cuowxers.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xerlongk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xiuwofwt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3garlmfyi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cticmpyf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uxakjhoz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfgoqwp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pnhzzitp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mzjokppj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bphnygby.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swybwjte.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kkvkmxae.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pplqyeav.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3nmuhfwfw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lmnbecqx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkhdmazf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fubqvzyr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wueelzkg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3dyxbkzwt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxcrehhj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lpnbhtpm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rlwkaqjw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cspzaofp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tzxmnaww.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuzwryu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3iqyncack.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnrymynf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwgtabwv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mxvyhjhp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gqxqusnd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eofpnwan.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hnhgsvkh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cpdzvcef.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfvzffk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vtofskua.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zqkotszx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ywtfplvj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lmwrmkkc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3npdzhkvz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nheughiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzfaxgje.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3urvtunax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjwdzbrw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3dhrfwyyw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sqaopvum.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tbtyumag.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ikgmvvoz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bkpkyyki.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vjznvuws.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3scqjydnh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ssduqnfs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rblldhwm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qvpusymo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yntgbemv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mzyfwxoz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rmrmtqqg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3utzhgrhn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mfiicezt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xxmaluwq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qjyhaznw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bsztuxyq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nfdciwcp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ovcgezwk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulzrmktv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mfsprsjc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfsspmav.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cwgfrruq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vmpdhkkh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3atmgeobh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mnzqiwoe.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3usadkfvn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vzylgvhm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3padheati.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lgahyidk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkztbrhe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcpffnmc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3izclwfxz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nntdvqbv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yqidgdgm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3snubfgxo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tgfdvqds.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hzpvpell.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3igmtcypk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vtfbjbtp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxugbnjb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bjkojadi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hztqknrc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3oezbuwvp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3egbdecrb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mfxjdasw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bhgflahm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3igyqzpnq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ykxxbwqt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pnjygpga.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pciaykfq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sjxixhgb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3poyoccpi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xjcfpjse.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ttfnwfyi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpcwaqgo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggrcvjrt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ndsxuvoo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3txlprgkg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ywbffjvq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrfncogo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrcgvtfx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kfjduffo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rcrehuun.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aegpliqu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mpgfqpna.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3thlrukfb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xtgoznvv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrafuof.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3brdskitj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cpfhuxbl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qqfszaof.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfbfjkds.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zkwvaslr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcafarsh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yjnlmmni.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qwrsdubw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zddgxzul.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mquvkvnl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkavpirp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uhuazqoz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jhqtrruo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuctmxha.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nhgbsztb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bycccabr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dmupqzcy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qvxltqbb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qvzgbkkj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3npdqxswh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hkavyckq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jdpxezdl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3frudrlub.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tprkveau.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ipyaovco.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3apexmmkg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mgygdsbl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3fdjsabhu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xeasytjn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wjdpasrr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3frmlwxyj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nseghuvx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3odjanqix.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nehbetbq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fzagwmna.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3znuytjkw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3yqftarec.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wrqcwrvi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3iapszqjc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wkjhrsxp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggdzcpxs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3abutafpm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jodibtjf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ouvcmmmf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zsxnxduu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3leveujgz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xmwefxkq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tjzmhrir.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xbfmyche.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fhxoesyn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gfbvufvx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dikgyako.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nzuohyic.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3trghmdzm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjqmntee.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zigidzzl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3luxbpgvd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mskytsiw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vjvdqwyj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eosuynty.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ctiifxyg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3smnlmzes.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fiiylyaq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oovhsyuy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qjkczhts.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bkgbfzjh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bkgnwgwt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3epnozikb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yachyxcz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zvwbving.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3evgclnwb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3smamcewp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3sjqxgxmz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3avqqyyhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioplezjy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3evhbmnng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfeprcvx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3udlbtfaa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vccedfcs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lunajqqt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lplxmlka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mynozbkj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovamlcef.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xejfjger.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jmcxdxxy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3quflsmho.html


<!-- 参考信息 -->