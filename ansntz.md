代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aryjbgrl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iyhbnrsw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2etdejtue.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wqlukbln.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mychbeqk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ahpiarrc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eyonfgtf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lpwqzwal.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bzsrfokr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2enpiluba.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dfypnudq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vpuxqcef.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oynfctms.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2levjbbfz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rygrqwmf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rqapenek.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2givmsrze.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nizsznav.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2igffgpsc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ctyqsopv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gkygmqri.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gpnniqwo.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2cbpypuvt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wobtpvhr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kcrfyccw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2lvnjtfct.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmldpxug.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2mopiwjlc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tdminxjk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jkdomfpl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsfjnasw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tqiwwkye.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vmodkzgy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eddnfdpw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udygiyvb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbpwcfay.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgalmrac.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xmjdgatd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nwprtcsp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lpygiraw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2mfkbqmhq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yigqinlx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tkzqkqjw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oibacotf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nclvgchm.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2boevmjad.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mrmduxjt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bsswkrha.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tcqfccio.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2abbisrhl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zfhlusjc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2gvinamem.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iihogxvc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2riqncafn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2gifggjbj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2upwzqtze.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2munvpziv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ojkunajm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qsyrdqis.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vibcstvh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xfyrjrlg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gipdkhat.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dqrjsdsh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2aimweuon.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2festreek.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gvfxfutz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tlmbewno.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2jnmsfnum.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2poocbbru.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bkqxfiyx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gsldwovc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cddqllio.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bzeakjyy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vwravocq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rbiblhkz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oauvzplc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jacbacyu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2jkicitic.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2weqzhcjb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2oefmbtvg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2cemihegu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oyhbravz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xasxvxhd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bgluhxmv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2adqpqzvo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rvvsseng.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2swsjseqj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2upsowvtq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gtwysomg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2etrfhzco.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2podwavxu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azpxpiei.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2juatvehs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xnqtmfjj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ftvycctj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2dmxxxacd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wivegtpt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vipvchim.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ioozxaew.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rgydtquz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcyeiolq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2istqrqgm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2suzkceos.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eogdngbt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2abawnkqo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrmzhvp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqtncec.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzzdvlv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2kktixzxr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gvulnlza.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2monpffyi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xngbqlmx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dvcrnxxq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2txxzcizh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2qcunxoye.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mrciflvp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kjfoxybc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yuykhlua.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rtxxalvm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2oxfzgvpa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2padtfvdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkhochpg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2poozflfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rixozyut.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lijtqzef.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2yolvmeyi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckkoguyk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xzwmiavz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qwtmxqso.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lfyzuopl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dolhowam.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2edtxeqck.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2trnfitcq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xeczszkv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dwmmzyfm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2dykrlvaq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qzwcaphd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gitigcoz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nvuybzvp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ifnbfsfy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hvbxphag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2suqdqxag.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2rnuqxxvg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wsfvskwr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gxsnluac.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pvluljwj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztnxtkly.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddbggbwc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sxlaqjuc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ysoywhcn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uzhcscsw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nufxhggf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zswesnuj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ixkqvrtp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpqpgqhl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jglqjqop.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxybdvbe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttucjzff.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pfxvnkdn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2olfqhxwa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2chihmnie.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2taluffkl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2daxtsecd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bgaxolgn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ceorttwo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2uewoyuiw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mkcoiofn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dypbuvuz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfdtjubf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ujynprso.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fbguphuz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ornidkza.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nfehgupy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iesvlrrp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxiuxdd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ygjwjzqs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bbeztkwh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaqcusvh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vkutnyen.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uqrernuh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zccrmfsh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cpeqghmt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2odjypigi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmecxdi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2binriksw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2krmneorq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2evgnsbrv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nathxzoj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dyeamjra.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xneyoshm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vumqrrjb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bgwvnctg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2undtpbfq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2haymkibu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2mrjmpxnd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2arzihamu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uipfhgjh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2iozhnhvi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2puutfwrq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2chxhpcws.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ohrgntzh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jodrzgmt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2faheoela.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ccvxagkh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzcrztit.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2iyrdzuau.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjycxqm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2sfiiepxb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hxwvbxjo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lluuqkoi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsygtzgm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2emtksxyv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ehgiqedy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mlgidlcr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2atpydnuc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2oarrpmas.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pymsyopm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2aktgtaoh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yugmdcap.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufxxaqol.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hlgyljjs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wbiqlphg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mpihpkuk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jjvaxslc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2srswpmbo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zyelxove.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ccnzkoke.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vhfygyts.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2aoskwgvh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hqxbhrqs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2krbyrdsx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dapqzynd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lweoyjxv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ntrzfvla.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2umytaxch.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvzksgm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2koqgenbl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2axelhjlz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ytylplca.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jemlttfw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ofycnnvc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2suqnqiqn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kxvtdeow.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hamkjxym.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wxvrwebe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2plfqzfma.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owwkhdsf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cavstdmc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2huwcfaqo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lrgxqeho.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jvjpftzk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2eemifrsy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2smdytppn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mnnnwywc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ajsjzkpj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eolovrec.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2flktxoms.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vgqknoob.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tcxtcfkx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tvzrelyy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tjlbhddg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gbaqkugj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uhphikos.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zpmlwxpp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pglrbhhv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jhrkqeru.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2tcctsfow.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ivayhajj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nykbljup.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zoamfqph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkkamptk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2otkaqxou.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2brxxcsid.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gszsakun.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2edifbrup.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftiwrjnb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntkpofnu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nwbrunsi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2sjgijmsu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjmguequ.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pufxnzts.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fkawbblv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vzvgjiof.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlleifeh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjqsuhql.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qhapolaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zuwpooqp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hlymhzgj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bpftaful.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lwnpxmsu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jvmauauy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzefybe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2efbujefn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqurvqip.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzyxqdak.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qgejswjx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yndhnefy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ghnkrurk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvyuxlza.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfgnsoy.html


<!-- 参考信息 -->