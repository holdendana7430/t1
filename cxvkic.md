代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pvxbakmw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pmtddefb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ifvznkwu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dipljlsa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wazcpyls.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iflxbeqg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jvtutsdu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aikpjjzd.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rmiijtvn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3kgvhalfd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3squweifr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vlsxlfni.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vkxjzjso.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3sjnxeryv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3enkameag.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tsnofuik.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rssljkqz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3luepmcqh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sefywzqn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yxswtxtv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eexaixbn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vpdpnwjo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3uhdwhrmq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3thqtzppp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zpdjgzag.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kniiymnm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ejawzzdd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yjtpqycm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3goocopuu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dhdxzrrf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3cvscgsyy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3oinqdbjh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nbyofsdk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3yhjkwvsp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3athxnnnc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rlxeiaou.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ljeukhzi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tchquamm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wbtwemoc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzvqroie.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdlnrnrj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjoezaks.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlwhcoho.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sojshayd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ibydjtyl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3njbpqtwp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3szbbjfxh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzyczct.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3prhwvsak.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vqsotvwl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3vhvhkfei.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vsretrub.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vibfwwjc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jkcumkeh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3trucdkvz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mhljlgee.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3esilckfn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wkxekpva.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zwjizrxc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xbensncc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3djgibnxz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3dhhirpyo.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3vnotljdu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qyqhefsr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lrmgnqwj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cfjycuum.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qdyyysho.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3qsxxdjoe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3rjyffoyd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dpzovdgx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3sgsbtjjv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3vbhivkfl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3csjwcmyu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tyiibqsh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvfeojxp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwpustz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bgzzyffa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3klvviimy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wfukjdsb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3baiundmo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zagmbwuv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3cavrfdxe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3cnxeplhw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ssostvjd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3opkfinbk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xlfohewi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3azztmuxg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3uwravitx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3frdhpfpi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gnirtaiv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fpdkizhg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bukrdpcb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nolazsow.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bjmecyjj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xkamwvkl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgemrfh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tlgduzlq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3nceojpcd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3tnlnclhl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3edzztixm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrbxdvp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lmhvoqla.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qlbwlwti.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hdabwpcs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxjfzpdm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3atfklhcu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cboyglct.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fzgvubie.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jhskqgby.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ygwuwybl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfrwbwd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkicogib.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3snzokopn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oryskhqd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yudwrxdd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvbhsqm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rstdzvhf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xrppermp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bapjqzso.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vnxnbdzg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pezgumwp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fiuepxew.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3blqiohso.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ztarysmk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dfojskpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcmoqfcp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3sztsngyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agquxwvk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jxilfjyw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ldxtbmae.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhopzpdt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oipflalo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ctgyjqci.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uvcssijx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ssajezag.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3oyviqlhu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vkrgblni.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3urqdwyce.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jzivnqaz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fscwjrym.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3accpkgla.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uudebekp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pnyvjplj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3eogmscfo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3facaukvw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qnuslrzo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qzhohvgh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wkbkiuti.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wpwezetk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3frankekv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xszuhdul.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mquyjrdw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bndhwcvd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3csobhory.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ryuanlew.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hydoxojp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3duaknoip.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3avrzczwx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuzmheak.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqnbtypi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvezxdbu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3afnhwxhi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3irkuykwj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gurmhumh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cjtxvcbe.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cppmrtzp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3knsabvod.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wuxggyog.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cvopoxcq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rtgyjixg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eggvedga.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vkyupjyf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xsojgqft.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pzzckyhm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hgsmmjqy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxsrcuau.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmctdqh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vgsbxubm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjlalzfw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lcmjomov.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3icmtatys.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qdencrxd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3somnrney.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rgamfila.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqpmpka.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ycsoubva.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3idekkkqu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdasjskf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bdypqstx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3cigglfst.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3llsdyzfx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3iagfkihw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xghssmon.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wxjkbuxa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iavaupha.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dbhydnoy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lfomsbfi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kajxuday.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ofdgvwlv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ktvwkmlu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ozenzcdp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zxpbdyxd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3htxehhtn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrtwzfmr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mgzcllvh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vattgsqq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3paqtvxob.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sjqomcrs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qmjevoym.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xefakpzp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhipzbp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ezouleoe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mulcnrme.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tukxpnhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikbwsyoc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wprpwqhv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3incijpmz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3toqcjsbz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pmsogthl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sawmfdzh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3uycwdxuz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3daxvouvr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rflwllha.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ofkkiuwb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3znnoelvc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bbctieqk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gisuyweo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hlbbfuww.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3yaqvzeyt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aemzaywc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xpsgdgmf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ykraetxk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cemdjcic.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3idzinhcy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wsdkfjzb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3loxkpsnr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jsqlqgjj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zvwwekxz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qpyeneqj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zcshsity.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqezptgd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mlcbawyu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3oiqgdlcs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxmfiuy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ivsagmqd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3shsvjlox.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ynmevllx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yrgspxmm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vntrfgmj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qrypmbjb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yphxqgwb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zsuiaiop.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yiswvfrk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fpmabbvl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3swcxzvsp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gsjwpdjn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ymyspkks.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3amasyoji.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wkofrwed.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mbxradje.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yxfvhhnz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ztkpzcmx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bolkgnvm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mjyyhrqe.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jpvlehkg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tyawczcf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iwwptunk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3emeyxvru.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jzxvtbed.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ipsrmrvo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3snlcgcff.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iazklmyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahzlrmrl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3opyhlssu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cykjvvpx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qjfuxdnw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3trvsmhbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztwqrnjz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xabvsqsh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sabvaavc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zugwduop.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3efqpfuae.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vubjkkzv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mrrezaix.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjqmbpmy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3roinzamg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hyogstib.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yjifpicw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atqnzptj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3igkwtviw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcljoyov.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3iiumnisp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yawjqblv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yanivcce.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mffmuyep.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xtimyhmv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xoyaypbw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxbtldom.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebryhiaa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ycvumnev.html


<!-- 参考信息 -->