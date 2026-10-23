代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jqkrammg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ncmofmoz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cjxprgze.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ihqohwbw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3msgokkzx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sixxnsal.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ahqhhymb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zebmbxek.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3cbtwundd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3drqsskys.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fgotaxfh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bgybmdyr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ckpwhcfk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ufbddmem.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fqyujpul.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vjrvdeea.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dsmrprae.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tnpwrjvh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vqqnzthr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uajosocd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uvcfqsji.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bsyixnll.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kxeqsbmx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eilvbkbx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jnuysslz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3oykcmgph.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mvxvmfey.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qwxipwti.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hywobwqq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3najemmax.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tqorogoj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lhnaanrq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bhwmqdbk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3jxudonod.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ikctioie.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uyhbnrve.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3krgiphsi.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mxgoxbxg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3szczlpad.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vtcbhgkp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3sgjpnbew.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dworiebp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ueybnrpy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qhxnttqy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3lrnpteem.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3smyrovmf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyitwunw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwdrprop.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gxclwvhk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3dwaxdmxg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oeqummfz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3evhrzelg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3flqzikgj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzsxqcig.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghhyvmol.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tdzlmyhk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uekruxrj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bpzdmpts.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jupcppdf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cqkereah.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3zfgzoanx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uqwaxiyf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xgjkcybj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3uqobxdzb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oidvhhli.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gvnbstnd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3lkxhgpds.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3zrfkpyba.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fslgkyvn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3mrbwnubl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jpxttgaw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3crrrzcwh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3sajwjzaj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lzceiauf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qdqmoqnc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qsgbbdwy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uicvnpnd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3kdccbddx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ufatjwze.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3prdbqylz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xnbbrhop.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ctjhilpp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bhiatmtv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3knlhvzsz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yxqakbde.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3jabitcne.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3sokdheqh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3jtaqmszh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3opxstreq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmexdks.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cokklixe.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjftdxnp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3faqhxybm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gnndixth.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xdwscwuh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3oyuhdmju.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kmefweok.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofiocuns.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fdecfcbp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3cicxfsqy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aeusicct.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3xuwwhefj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ardnyejx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lhsxthxj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3mczvmtlp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qdqeceii.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fckncral.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xepbmign.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qbdesluo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wxjibtpf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jvbrzbho.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kuvlpyhf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ikrwyiip.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3cidrccmp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rlywtjmp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qqzgrnbz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ywwaacgs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lzdhuqtm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3alqeunsy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fuktxzei.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gykvxdea.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3dlpgfvie.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tiqrypws.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xuiqlqts.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yungjivh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tmfftkky.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3llsfimmj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3exfanwuc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mtdhuuin.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rtxtikil.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3luyzqhht.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3okyqisya.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qymiekar.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3chtorhmw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lakykzvh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3lqwcelcw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rotkcpyc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pjbgipqy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dagcfgfg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3eiifgosp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dswftywh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juktwwlp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3orenrjjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auzqfsha.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qryubjuf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3npspyxev.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tjnxdriy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rmnxlzsd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eivfqlti.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bhydtzuw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uuybyzbp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bnjeonat.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fmywhnbm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fagmhiqg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3wkwkcopj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yywphfsz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kqqewiby.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qwhihtnr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bfeivgja.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxipnzg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kdwawblq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yymocybd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dpndcdoq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pvgfzpmd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qshazocv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3idntwili.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lnhfpxxp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtllslxq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jenlkbgw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fmhbmtbh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3necorjos.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wemscxym.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ofgoidvr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqfdyeyz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ehamsfpo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qalwsyeg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3sxsqlgwx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3iwixjane.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cvgyintq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fflwekdo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iiwspwxm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fbvfogsc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uceyvkjw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwwxolid.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqlwvajg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qnyqydyx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yalhtdnn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tfxxmrcx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gegleesq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fgjjckab.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sijfpkpg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vqbrtkog.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkynhymw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kgjijzus.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3yjmabick.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ilznbdhs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3flxqqszp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3knljvgji.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fdmqzfqa.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bqtyyopa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3owbhqmaz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwrzgelx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjdxbyoy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wyjzznep.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cfsbzhmy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3upwbwvwl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iajlrvvp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fmvjeyge.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gbfzbeao.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3trynsvio.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vcutxrsn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3faqcwkrp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ebwxaomw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3geqhiymo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vvxvrecg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yywdpydy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qqzmihhc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3oqnevfmo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmicncqz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vzrhnxvb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mfmceimp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ktcilfhx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3shfqealz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3oajyqdkr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ihgknkvo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zzimydjz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ywkhgmtz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fgryxkkw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nuxeevyr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mlsrjitk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3sujjhnjs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wrancbdn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ydgozgjd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lyojkiif.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zhrivzsn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3reybtkey.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ntkkgcqe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nxzbgixh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tihdrkve.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bggffyyx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3scldlxod.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3klodxibk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3neitgmfj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wjlpausf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dorqocgj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zasmxfkb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zqaosjma.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shmjonfw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mmouosdq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtbqfhwq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rkdajvgq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jgpshoiu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cuvndwkh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tatzkpkk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wulsdzvr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zynztpdi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vlxzrpjc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mfmbnmcu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lmxavira.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qqaebyuc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gwpzhkrx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3njtqseoz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wpbtrtgw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ixlidgkq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3audnjmmz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iuegbcme.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oqinuiln.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ebsymgit.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojkixpqc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttzpnnlv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3zorzlydt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3levkomvp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yninlamr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lzycaotx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vagqsvgo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vrfnifai.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3djbrveao.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jmiaumav.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3evrartew.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yjejhpsk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3uwgddygm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wxsosaax.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hvawukow.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kdljcdrk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3impuglys.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gkenrjci.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zdyiwhfn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wnxjyuqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmfhbwvd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ucqaaakf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrqfyqoq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nckvkydl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xeqfmevd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3meckxlzo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ffqvkxjp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzhtcrsw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3irmhmdgb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tbimsdca.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lgdeysdm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jvslhlkn.html


<!-- 参考信息 -->