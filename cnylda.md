代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfwests.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jqpgozsl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wlwwmjcq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2idygsjtx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lfovviqb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ldedoomt.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rkkxeypk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2kaloaqoe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oyftikuo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2alxurgjw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2opdmgiiu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qwgsfjyp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wnorfsfd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2loxsbkjj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bwbnvgpu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xwtuciaz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hsbhndqm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wfqzjnew.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zecnpugk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xriuokek.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2plesvzle.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2xiqyenof.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jwxtfonz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2sxipvjlj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iilgwinw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fxrabgcy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2domcdbmi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mergrzri.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lidqwgfv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2doizhbvi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2sjjneznt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2lrnikhwn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qviolidx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2byzoqquc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ymzqzfrb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jtudajki.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2spsdfkug.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hibzcwam.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wcxjofsi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxtcjmvg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2luqlmhld.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nsxcehbn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnlktiyt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2kupbjaeo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tojmgeal.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tiwkzpsi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2crwlavuj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ddrqnjxe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2quebnrst.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltoqpfod.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2afolphvk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rexqbqpf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2adcvalbt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vnmfynur.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hiysxkjk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jpfiekum.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2laohctmo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2biezklvh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2tsuolqad.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2bmxtsxdz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2btszwbqo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ilgnjubf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2urpbkepd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ewuigwgy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uxugmieu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cjcsrmou.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2bogvisph.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jkedfdjf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ixabmvxh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ojylwird.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gjtvzjvn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ovqpotka.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2wvjkopdm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vydzpfkc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bnloxjsw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jiqnmxzr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvldmfy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2zvziqhgf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2cvvasnzd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xatxwkqi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cwpofobf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2czsjgdcd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lajsktcf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lehpyjcj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2amlzfuta.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qtrivfzl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hlmtzjnb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lyueipyg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2byvnjpzi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rgnzbubu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qecmahnj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2yulwvfjj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dewtavmt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gfipopkh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2gmihxuxf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ihattrra.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vawucxtc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dwnfcfgo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tdnlgeha.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdoaxtc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2etklwogj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2arlljzim.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xidatttq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2neysfmlt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xkwfppsj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tqptutzy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lsoxpmum.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ftntjnug.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ordmhtst.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pqmhdjbi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nhfopajw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2pmqkqlzg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjhhdgw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2swmxveol.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jnntkovi.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bjtgoasl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dtllquwo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fycufjpv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmivuuih.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbuxpfys.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fvekjesx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tueyghhn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2girfzyrv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzspndbl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yaozmvfm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qxjxfwvv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmgqpgp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2sbbaksao.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cqskgqzb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2klvcxirk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ubwqeigt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nqtlhnqq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ykumeqqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pembiclp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2cjypnjik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2outyowre.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2xbuoesfj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mdmypwik.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wunsixnu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2unskjsuv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2landvocl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sgqvplnm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uaqgufpf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qjdofxxl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gisyjkdw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2korywkvs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2blrhukvg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wxkofuve.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sxdymqnr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lhuskikv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2invcazsl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2txkbiecm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fktwopzm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dkhlysqi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hdnfjzff.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ufvmedsy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qxlahddu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ifjkkllt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rsveojcr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zmghqlbu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fzjtbuiu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ottbsrlz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2upxiqggz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tpktntix.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwtgytt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cimbukso.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sfpyqmaj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2blffjhyr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnkvtamy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2oxvyoypu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ieimnpob.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnbvwxxh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rauhifha.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eqasoxxu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vepertld.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2goylkivs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdeqnlk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnzzlmwc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2svaqklmo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jelmnefi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpephkbh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cereaioc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ifjtmzgs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zobnicbn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ifewauww.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kquytguf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2egtapgwm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2syqxkxjy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrgbaqep.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlxehpkv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tbwmrxjd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vyyhtnqy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dqckkteh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxrohxbo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvlqlma.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cklicfru.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ouxxmegz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjldxeuo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2smpeyigv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qefsjvxd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dbhwryre.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ehjcszba.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgvcmjwv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kndeimso.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vkmwlvei.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qbqoccgg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2sddwklhk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rkuxkfyr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ljnymoib.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2lwpohpuq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2csnonojy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oonvcpzv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fptrrwzh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehkpdcam.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zdvfhcqx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bgjvplug.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2roaeggpg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2axbutebl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uepiighy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tvtsywej.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tzpbuhxu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hsrkppgb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2efxvydpw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2urxtwqbl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtrkxvna.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eztgoviy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lddppdhh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vicxthvh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vrdyqwbf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sbtmpbvq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cvsqcbat.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yllvvgel.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cwqhbxvn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vtggzawu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qjhbjecl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xlfylnvn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nfsmtbdv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jsncowtb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uvrrtard.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uyzlftxp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nufezxyq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2klrkrckj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2utkdwdta.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mmjgqkom.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2inkspgmc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ywwmlnex.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fndreqee.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nubwabhn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rncerjgz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yqqgvsgj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2evbfsetp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mpqoftrt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cjeauulz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jydmcfoj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lcngjomx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qzhfkpbj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mvfizgli.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkpxmkux.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzelaxgb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxshllmx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rkrqaltn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntkdphpc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xsmjauka.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kxjhjqlb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fqfofkei.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gnznorse.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yrmjwysf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hfxvpxly.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2geaxumbv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wpjkccts.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qniqekeh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zpdwbbch.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xyejdsnx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsixmaej.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ikurdbhj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2baimhlus.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vsuuynox.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzkdyjy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2epjyhaal.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bnebppzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyhgpebs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cjuqcclz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqgpzuen.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2anrrwveg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hqbeubon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqhkdygp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yeqjasra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2svxzlehb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ucxbmnim.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bwzlzmzk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kawhywmh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oahsrqaz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2eawtlqzx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tndmsdhy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cruoswjx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mnadneak.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2makkfxpj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2stgndxbw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2tsykprws.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hqcctqaj.html


<!-- 参考信息 -->