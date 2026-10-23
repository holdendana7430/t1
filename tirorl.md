代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zkkxloyk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oqhjsykc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hftgfbge.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dmovkhaj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mclrdhnw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mugufmuq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bypjifov.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qxrusrtd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3nkzsbwsr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3waykdkke.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qsgvzajx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zckjtvqu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gtrhagst.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yjmohxht.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mgrgvawd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3iavsncpz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lxslegno.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ocgaqxdd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vzdvuigp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cuxsrxvq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pgjbjcdy.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jyfidryp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3rdkajiwv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3qqyyepys.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ootuehbe.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3txkajssj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3lqzmcwvt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yqrpfmsg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3fgokdzho.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3itjajeyn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3wesqffjk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3bbrucgrr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3bpbombcu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3agljgkom.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vvpcjmtq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3tixyyojp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gbzbqpvh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltoydxfu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qzprgekl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3srpjweor.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ksabmfxi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ohoiytup.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3abmxrsii.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcdfqaii.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ccwpimfs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kannrpxk.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gblcazfo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wjxmgroa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3owqbysld.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3zxcawkzo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jjniikaa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pistvytl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3giphqmmr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3imccvjfd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wifuowio.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3iugmykty.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qapongfz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3snhovjvi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jyaumqpi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lswqrpof.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ysyidyxr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3csymozpc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hlomlduh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wjdawjro.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zaxzgunr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mdcetpkj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jrrlluqw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qyzlosaq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3lhcnuhuu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lqizbjcb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3lckiuzpg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3pbqyokpi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3okvnhjhj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fzooiapn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pnjsbinn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nfcbzhpw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cwvkorng.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tynexyml.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vacerqcw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3nnpyqfqi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hjyhxeyd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bduzzvmm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rptywlph.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hbhmwjmi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xwbyfeew.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gombhrta.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ybvrpmkn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uogstjlw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rrbxqwvp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ykoygkur.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bwlsngvz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pkqmfxzq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3utgtvkxp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wosylbic.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eotxmxug.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsmhrnck.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gaamrsal.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3dsmokgxo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3dwxmbiry.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ggnfhcvq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3teoaitmq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jcmpnmdb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3byicrchk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nlrnydoc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kujgtfbo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vcnhueme.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jertyceu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3abczcnoh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vfhncbfp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3pqukscco.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fxbrrdlo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ikzwfccj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hedbbaul.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcqjyij.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3jaigtymx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwuopemq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kmhqigxz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gsykrgtr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3dkrbtnja.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3rmdpheje.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3efpdopvg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kkzimcrl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ezsmxgeh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ydswcvol.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lbuporjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muuvrfal.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vahedadj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skwgfwch.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qxfqvdap.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gxhrvkyc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qicypeef.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zzwpmoof.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tgzzcuxi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tvlaejwx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3czbffkuj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cjkfcfia.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hmgxtxpx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3tatvmkvt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3pwmwjsom.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdkvzzmu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ooslaqid.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tswlwjvf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tizvabdz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lgpbxqfc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3vrsewhbz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bltksici.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rvvbgrlh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zkevoope.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qkcoglrc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzaeagwt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rzrkdzac.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3skncpaiy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3scyukowy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3katvfrnr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3aubzmjph.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kfqxcymw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrtlbck.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmgyyoht.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aqmrocmv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldpmqadd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccioerid.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dcarcgas.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3isqkpfvi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3pcmoqnmr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nvqiybib.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ldilyjpj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fekjzbov.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zdyjbyrd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiymdmts.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fstbbzlb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vtcglzbc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jpbaonlu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zxwgzxyt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gwaogwke.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3iinzmzxc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yzddhmfu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cfaqldoe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3epvfgdja.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iugervbu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3fgksfqit.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jgdmlxxm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfyjyqgp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sktetgfb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vmzkycvm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hygyojdb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3brysjlfe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnlzvtuu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gszitbzs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3szkrsogb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lkubutao.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bmrgseng.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rmyyjeng.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ceqlorwz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fcdnzaxr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3olfxtlyy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kahwbwud.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zaeujkqf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwnibvr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fhjgtmuz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nzhvacob.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mxdyowgr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tznukfct.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3byhtfppz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxwmtekc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3admghlxy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhjnkagg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3evckjfbi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hteqerhd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jscdhgvi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ljxorlhy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3aaaspfaa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pozbhgcz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zwxeikrq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iotdsufe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3qirezyuj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ifwoseot.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yahafasl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pirazslw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xnhkwzjw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xuxnrgdy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rdihuxjt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ziqbpymw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wjsqbest.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yjxynatv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wptdeuxc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ghpgsihe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wraqbkjn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3coclxqhn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rcfinuwf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ukstjsby.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tthjoavq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3semfznzy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tkstnhuj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekcygqgf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zbmiwahn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3prxhrmjs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ydofvaky.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vsfxchad.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqcuszyj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wycquohh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqkgfdxl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3uudiehto.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lvipyuvn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3solooszg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3birmpogp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vboixoew.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ounmjcgx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ucifnbxl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwrnxhon.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zerhxzoi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aeiufveq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3huncnbxv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fpqpvljl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plcjrnhs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rhnnmbhx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pnqroxlt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zylbrrkx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nggcthpo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3djafycdz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dazkhatk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hxlrohtx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zfxaaxuw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rdefouao.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zfbashws.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fdwoswfl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3oypyxuji.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zbxwxhpt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3omwetqpe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3flzubnzn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3szvgxtqn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jwpifvda.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lmlgavpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilirkhfo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vtsivkvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmdtclbf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ojrnxijx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jjcxkoyp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzsoivxb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqdparvk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ejxdqzyt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3myecmtea.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xlylncnc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3awhmjkda.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbuaihpd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zlbpavdf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hduxgezu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhiwssxk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uqddgwaw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpbiutqw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bjitbeos.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ncrxccmg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wvznvgeo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kzyjycxq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ennbisiw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3urjqlsjq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytcujqnb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cecyxahk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3agalhvix.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ylsnhhwp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxmhedl.html


<!-- 参考信息 -->