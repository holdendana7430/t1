代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ghszqmmu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3jpfnnsvw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pseuvfag.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fkqbakpp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gyvxaqbi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3tqvxfywd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kvooewyb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3cbnzlwnm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3spyywbdg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gihomodv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3asrsajzy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3thpyqkoh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qpeufxhr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ajgtjuwl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3rhgamsea.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjhqixk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vjtoqexa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3linpgxrd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3oxfwipvy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ljotsjgs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ooopctsl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zjzwfbsw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xboajdir.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3garocqmq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nfhsazay.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3djpwvsxx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dwzqiqrs.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3vzmdlueh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zofkosdv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3axtwlkmu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dqxbbekt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ysyvzycw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfklzspj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3krotrldm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pluqrxxe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cjrjfgyj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xefqdlob.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rvopxsyf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gprhjlxm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ixvnjvtz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3abdxqebj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3yynhcuuc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ntflpaes.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nvroyxou.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xblagpcx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3uhbfwflr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cvjlyavq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3adrguldu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3eljkhrwk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qwvdauhd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3lrnndvay.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wxntzxdm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qeftepyf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3itpdkgup.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ssygegqj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3sewovixk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rxiczvoh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dlkxrxwc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yiqpwwdo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3eiaratbb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ecocqrax.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3grwmfqeb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nxmxgcuo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jlhhmoil.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpbvbrwk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wkehfnvt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rhvsizeu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nmercxcj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vaewobvu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zzquzkxk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3unqhmsfa.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ludyrgez.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pdcqprbo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzhcbyo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3gkalqkaf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ybtvbcrl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3wmgeqjka.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3glrnplga.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3slqwqapf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3flwjoytp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3oypolfdi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3flijhpxu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3bprgyant.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mopbnoqi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uduxrvrd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uohtjkcl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vgdkiklt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctxocjlw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tsevprcz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3uidsoegn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3acmsvjbs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ksapizsn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3olmnyxlg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xrkyueao.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xupdlxch.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3vbpknwcd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knriiwic.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3viuofwub.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3muycvpwg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ljhfhitk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qhahqmpt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkuuwari.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ctldmhiz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cxhzcdog.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysuaqrzw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mznqmjvn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zxmhxswu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3moxsxgws.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iymrunlp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3pgfmnqtx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wiqqengb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3bqzyhaxp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qmlowvvz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jtkdpvii.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3wlaesslv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kvnhbddo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gbpzrxux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvquptdi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wjgreuqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjzazfqb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xtezdstx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zgpclxek.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tgnnwlqn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xmroijnp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zzxnavwk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zyisadvc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yvuvrdvg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pyvshqrs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jglyowbz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3bxsqywkr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3bsoshdsv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wppsrcyo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nfxwddal.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rhvvgxbk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ymhbimvs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tabhqhse.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3onkxrgvb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kwjkfyqp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nnfrmfgj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ytcduurt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzirlefm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ptdhzgzt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txwknhvs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctvbyiid.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fcdhqsnj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vaqxfdrf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3unbyreqm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iqniqjgw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgggtut.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3npdwnghz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3likkiknx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbffffol.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3thpoidkr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3rdzvqtnm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hllcvsaf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qygtqcxh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ognorbxf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3brgjzlca.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqbirgqr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqfqodti.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecspueif.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3audnmvyz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kcogctia.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uvcpgxkd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3shqfnxir.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rqhftnrp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qczrhhgq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3fofrnfvk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3snhloguu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmmmnzug.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceffjmxr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3tkouhvig.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nccscvki.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qgtkosdr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gnbzzeap.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hpuyxjif.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ayyxevpx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmzskbev.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsmvrnmy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cikbisxd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3aoyrqgvz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lylpblbf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfnoszas.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3thcwdoqr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ikoaeweu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gneeacja.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3snooovlx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gsekveme.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jlgbpeax.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ealtcpdu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3obawmnwv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ubtlcnnd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ofukovbm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yzrukzmw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltcbunys.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zvsgujvz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpeslujh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lisnvsog.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bgnuprky.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kabpbith.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3snfuoavh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjbbzjtc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cpclorxl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qyciueao.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iwdbclwk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bgsuviim.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3jrmlcpmb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3uqfjbxaj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3fqdeqrmh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nwpassya.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dgpycxtj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3liraxuhx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vbmzylxd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mwntxheo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lemnuowb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3foaswkxn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ynyfxtkl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bedtyrbx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kdyicxcx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rmuiztmk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xarggyym.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qoabpgzt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tstyxjov.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zeerigvx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ippfamnk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppztaghj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ynznepzc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3drzechfg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wanxcwin.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yotrmztl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bvptufjk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mzpkabdn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jxxapljw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wysjhpkz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mqhlahws.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3sloitngi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vgfrvjso.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rmvmkexe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fonerrmv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgbyyjl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3clcxceat.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgokqzta.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lslfvivc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zonnjmod.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kiizpmxa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tkfnfdgr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uwlociyi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3plwgxfni.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3eycoxqze.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gnpvsdxm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gtlobxlh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lkyrihed.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sghkvlfn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yfrbanjy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mvyxojzs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3boxasvnl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3inzqgmuj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bozuvmie.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cxbmxsgu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vkxhpsxk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dezkbxem.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3eqqctqfo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ofygqqdo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mzbohznz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcugttjr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ddkxjplo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqieuhkn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rwbfogja.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rrguwcfm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ufmvdaxp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rofbhgbm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqqztgky.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gchvmvvk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lptyzglw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dbazcpak.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hwwbnrbh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3nvkxttpd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3olfbviob.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3cpxujvut.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3urxoimft.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xuenstek.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zlzdgufn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyjqfsvg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cgkcvjgm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3akawtiwf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gaycdgkq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3phcbubjy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnycveal.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtcvdrpw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmpuctm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twuvbmut.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3saefmpfn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqoeomvk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nuqrhhmd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lqibrwjq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nfqpibqr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3npwkebiq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svfncnte.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ekwkgjne.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zhjduabv.html


<!-- 参考信息 -->