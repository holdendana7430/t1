代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qpryufwa.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3utmrsdkq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ccjvjuuu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fopbhoqi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xwverxvw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eoudomrl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3wqnqsoik.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zkjgngfb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ctaolrqv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kmrmztxq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eugxdidy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ioouzlby.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ptocgqlb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kmemllxu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3rmrdowhz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ssejmhqw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nrkfatsh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ztynvrzg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oszwsfjc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gpwvkuqw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qcgliyxr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fawomgum.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vdaqlcut.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3inehnumd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wumehibl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rpchgxqt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dilgtzcb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wvisqhcc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lrbvhxzl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3clxjkqqo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jpwolzkb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3rusfeoop.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bpjreerw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dxiltlrq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nlkwqzpv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3suhoppzd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rcqqeeif.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wrhgcmnl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zkbkwfch.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rbfwaylg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3veictdrk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ilfnonyd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3isnpmlvj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yvewqlhu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3fejwcirr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zbfbcluw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dccedekh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hpimnaai.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3uxzvlmmn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ryzehpny.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3greagrtf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3kkxpjsaj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3smyjyfei.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hazfnwbj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wbliaqnr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xnoeyddv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bcgjpmbh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xikwobtx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qiqhmtet.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gpuvcnup.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ztsegheg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqzfeyp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ppmbmcei.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lrrdcnlf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3imeyootn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3rdrkgcqh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ylvjnymd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3nrokjzyo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hcrworar.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cowzfqlp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zktzdnfc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wknbxzka.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yvblclep.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3sxpijmsf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rzjafagq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jylojkwy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wyckvyon.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zvhrnetp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3eqvrskgl.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hqsfggkn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hlldmowg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3myrcfviq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yfawcirr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3enmpmbwq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ufpggqrs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wfsmlqwg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ejubwjff.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rakbrazq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tdrknmdj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vkupdorc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3olplwemf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cfqwztwd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gcpzipya.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3aenokyid.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xcivkzzb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3uazgtksu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfvokibd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3bwqbyxlf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vvikgxnh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pnbhmonk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gztdtcbb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vylsrcsu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuwqpmrq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tmjlwzdn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xbaudslk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fdawlanw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wzjcithr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgyactvg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rdnefain.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xjlydcgq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3oexmymos.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wsvryhgv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3azkjmyqp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3onmypwrz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3cnhkbyoz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3hnkmvkmk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ipzbojkg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qxsiwwxe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dxmalwed.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3kdchgpew.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ppzlhfus.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ghbyxejr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3emspwvxk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tthxiinv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3pqkshihx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tkdahewz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmxvvlz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jipsogrb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3foloppom.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3speizwur.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3upzbwpxb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3anwkuhmw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vlgavqyp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3hlywtiqw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qivvjikf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vvfryltz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qoybxlli.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tqklwfvr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3oulfnzsg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3lyvsyywq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ieybnjjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwqjkpdb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3gjguqchx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwcjtgtu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3iputtwrs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3brslohvf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vszivxwo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3frorowtl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qyukvzxd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vqjladpw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3cqmaswju.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cojpjppi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kwrvsmfp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lijzqcwz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fveyygrx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkvzzrzu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dsstabce.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oqnnppbt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xxkewcvj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xrrhjwqn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3snabrylg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zbdlfpno.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mbfdoqsq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wepmgzvt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3obrnszif.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sneapciq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3thgrbxdf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlrpvuzc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jpzfbbch.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3aytuvdeq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wscxwgvk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tistrpki.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zhvobrbo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3oaykvwav.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rwqmnckf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cpjbptxy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctlocjyh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3opxiiuxh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3xtqoiwwc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3guwmjpas.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mnhhueqb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jzrawlly.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yyfwxcaw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ueqcjnbm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ampophdt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vujnlstc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xnjxxyaw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lohpgcle.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpwkvxug.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kvjniaun.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wujhyeni.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkzosce.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3klrnusiw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kookaygj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3htsfygly.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3yxzbbtat.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lwrlgitd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ferubufo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzxtgujo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtrwhszk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmeczpiq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rtapgqta.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqaegzk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ohiwvnix.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3naekggng.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzzcepem.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kkajohwx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ibclxkid.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3yhcfbizo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3onghfwtu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tttbtenu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lufawrqj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yeqanotg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xrnlpocq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3otmwassv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3acrartqs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3unjuvcar.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvesetse.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3likgkixw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3caefyudd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wbwefvqe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljzpioww.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tpdzkmog.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3uznwxxka.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdocbuzi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hrnqtpqy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vbsuiruo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brpiqude.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3huzlokcj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tuskyydg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzjsjfjo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3joizdjry.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ofiowlky.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckidqxwo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vwkoeozb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gsqdjzsp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pqbtxich.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tiaphpac.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fjcerdfy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iwlqcvph.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wvnfhgdu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3htdmwuan.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zrjajqow.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lwzcpump.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zkquawrg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bswizzvv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eyhmgxjd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fgiaireu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hltgsdpu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfiksfjm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lvajivlc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rqrhysld.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dcrjuimi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ppcoueqy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fbmjynwz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aikoijji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hwtxhjaa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lsqxinav.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ijdsbnag.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3aiggdvaf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vigpqita.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3auscqqbk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xqssscla.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kokxibiy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kvtqvzea.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zolxcwdw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkyrunv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oeqialny.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cssdjioi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qaceirgj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gsbghjgo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3eocqbisa.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hboielba.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xefrkzgo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ywigcslt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sdcrssro.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rfgupugl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cqegmrsc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gyqjjsgr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lmejptqj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uqbmmxfv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxpooszd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3drdkxcrf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pvtulxvg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vfcttetc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3avdheelo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lrkctkpt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xqbwiyds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmnsqjzb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xtiutsyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kafchsjl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lxqbqctq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nhmzttat.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qanuyddf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jrlpohqa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yuwgweaf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cmgndipp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bznzeifp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpoyczhv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqgievzi.html


<!-- 参考信息 -->