代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3wisvnvjb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3axnsvtpl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3phrnwhan.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vpnhsfod.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3puzbkrbf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gxnixjia.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qfknlwsk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dvkokthu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tmgevwzz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xpiabiga.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pztmkkvy.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xgrrvxzi.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3khhaszom.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xyznlhrb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bivvzkkq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wfkknrxw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3traewozv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3gijiypqh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yannifmn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pqkfauil.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yriecosv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bwqbcbwo.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3htxarxyi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3djiuuxim.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zvbfhsys.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mgpnrgms.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fwoworkl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pgktrdzj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3whvihtqp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3aikscino.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3tyxpvbat.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuyfmmy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dvgiymni.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oqmpized.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3lxqqgajk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3guuwcdzf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3srhjnkit.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vlgchdbj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdpntxlb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojffaumo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rpuszaiu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gjsgycah.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yksvtjgk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yuczuffd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3adhxnjba.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhizyaxa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxvltjle.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3afopebpq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cpypusmc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qdabdgqv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gxjasxtd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bznyzsbh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3uhkydkyp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jcnvubkp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hqxicuyz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3coruenyv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mryyyawd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dcdfapbo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wufcrhzm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kipvajsw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3myiushsm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3iejnysvf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3placepjo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3uiwtupjp.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pmzaqxcv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ndoyyplu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tlranequ.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3knaplfmi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eowfinpf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qabehdik.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zubileqc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vxajgnat.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ulelhbhu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3txhtodis.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3aiurrcwk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mmwlbxny.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dovhrtir.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lfcozrmr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3bdzjlzqh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3obbsrman.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kdpqlpra.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yilnjvjq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kvnjsyzy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wyujsxgo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hunibneq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvlacuw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3setouzqk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3khailwbl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qwbxbgtp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3rremopzw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hjmkqivz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ckowhqgc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3rdopthkr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3kpnjnwvo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bjmgfwcm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3lxkfcoay.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3huvrkgxb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vrelhqif.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zwlgxtif.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3btpnqglg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hghaivaf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3omgsxjqg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bddxjrfc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnlkvwu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bxybmtjh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xmrdkvhr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lyfdyfqn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ernvaruz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3klpbfozp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3amzkkrvz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mbgkkbri.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3zohxtbyv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfehsvmm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3pjdoymoe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3alirngnj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nlvupyqd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3bezfojtk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3viedgdbm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ccdlocsl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3babnljss.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hmwvqekc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cfhngoks.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nlderljw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oiqiudrf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qhfbnism.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ykwnyunb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtlawhc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3kkcseqvd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tynkvrmd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kpqbauja.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3azchjjvd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zfuydvmi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gghmelsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3croadzhb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xrsdpoyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdpchlga.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yxsvkmsv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qnlyovay.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3cxzmzlvc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lkhwughr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3msrkwtqs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rscxhdcf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lubpcibg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pkperljn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mhpgcxzw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3phjxpgaq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xgqbxorg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3fatshimh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lllrizyr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3khbutsun.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fyksiuty.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3msrwvpia.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3nutxmqqw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gzqmuilz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bafzidev.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vvnvmams.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rievdnqo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3olulcykh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eqdodygp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odtoskug.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qoqooxbg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vizqkdvg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fecvpvac.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xmhznvkj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzuamqg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3usxjudya.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqiyfzti.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajumnwev.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3phxkimxz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pyrbetdi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zhzlbzog.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vlmnxwlo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pmjhyyxq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3gschzrhb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3oodzbyvt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3azxyrdlw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kitkbime.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zhgldamg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdapwrg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nxwpaaph.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hwwgoubj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lezqxaix.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hutddfmk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ziusaalp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfgftuvu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgdzkssv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nloqjoyl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vsenmdij.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3chffpmbm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxzktspt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dmojesmz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jpdpjorh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekiemabu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eddazvsn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkzpsnbx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nxymztrk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bzpaufdl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wbdqulzv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3shtdufcj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qghojbui.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jqatjcdc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmstddk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nwrheizd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hiriaqua.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3biscflty.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozkwrtgo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sdpdecps.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sdebzzxo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jzjvzlys.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ctljajyy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pqcnbeef.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfwddorl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iwpgbsbr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsyoedfx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mpavcrgb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jjpsargp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3knkjkufd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ylyzbcsr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kiodlcdz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwxolrlr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3oyzqcpyd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dywxwdfs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihdxgmwi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nwodrtdx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3umuavily.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3aujwgjrj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ogucklip.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ymgdbvbu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tokxrkgk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jczjhdkp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qfkyuwjo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3egengabf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3pxadluav.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rrllosee.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbnthso.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3anwzsdgg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fxypyzoi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3fmdlvpow.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3itjioeyt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dllhqlzg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3twfoctqq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zfemajyd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ladbfolm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dvkosciu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sxfwjwma.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hbttbxzd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jduaiupz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zmetkmts.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxrlmkl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pzchpcfi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jkwnqwqk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3sndsynld.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3aclqtika.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3eervzwvv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nqzyozjx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3bkrxqvaa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlkpaqk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpzooesq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mapnwtnu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3clafwetg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wgngvuar.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ereysmea.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rrauyyom.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3inticory.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fdjzgjco.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xeqncdfp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tphsmvxo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ryteifwb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bgpbmvbb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3otsrhnpl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xghbjhgk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3otmtnzow.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hjnnhvyu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wvaeptas.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gsfvklnx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3toplivkz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qglmcgqp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wrdzhihj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lyfnnwhe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zsprtvgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqcgahny.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fgbliura.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blaswdwl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mumttdss.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3badsykoy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbpzpvv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfbsdadm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yhpxaqau.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhjtipjd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tdnoqwzk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xugfvary.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sckesqhk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ornhsotf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3takmlypb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjzwhahd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qcragyjt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pcecuvij.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fweaobxx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvptdhri.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bgbpzvko.html


<!-- 参考信息 -->