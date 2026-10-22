代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tsxekfho.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bgtaipsc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bezuspik.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2mncbfybr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dxzeohde.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ixnkukwk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2adhcchom.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2skqztbdv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2onfottrf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bkqrkokl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wudcgkhn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2phitnovq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixbgqqwl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2rooksspz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2zxihaqmd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ghidfsce.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rsedepjx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lhgzwzua.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yafwqoce.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kcgutysk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2olncfnwx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eqstxtbe.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lmyrpnii.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xkvshazn.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gcvbkdsv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2enhuletf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uvdabzeu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2klcxlvbf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ucmymxjh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2twtpohvo.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ghjvpcyv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2oeexzgfn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2afpjbyav.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2uggpvtxs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nmmxyvfl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nmwnzufm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zbuauhcz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2udwlrzfj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2kcphtusw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dwccdnev.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fplarwwx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2quhcpnwu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2islhdzmu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xhxxgkrw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fquhupcg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2upafecat.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hbwyypsz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jkwxwxgi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vskmyfxu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tqobirfk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kqnziabz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wdwgclty.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2phtzqdvd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nggyizho.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rcugqmvr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dybrgdtd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tphfxzwz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pfzfyzzt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sdjpgfzl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2diyohjii.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yqkeqlgg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kuegfzqh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2eyvjkpof.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gyrdplrx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iskcbnuc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ogwyykza.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ltjgzsty.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2onmmfmkh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2xhrarhme.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2hfwvyiib.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mkwtduav.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2degpxxon.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nvfshkzj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2musiklin.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2jzzusjqy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zbbflacw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nvwgbssf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zcvhtosu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2pubsgfed.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2yinnzjyt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zlkgdtdo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2utdpddff.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rknzpzqw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2veoqsxgw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2lfmmfryi.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wbwcwtvi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fxxuckfi.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rhoxlpdl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2yixpzzxv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ekutbhxr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfjpzxz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nejnctew.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2chprores.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2acxejdwk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hqybjsej.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2yejfcscn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aawbtvyl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrsdakrd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tgnpsoow.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zzvedcuu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2cjirykyf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2onqkjffw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2srkpsdyj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pdpeuyem.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zpodvrey.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2frxbvfxs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2mitzteot.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jpoxjzsb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mwrdpjft.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ungjorau.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lhhwngpa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gudsucbw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mkarspeq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2niwzlxlr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xjuukekp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ddrlizbd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pkwpmlqu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2djnqppxk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2frvkjzcj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pyphuuwd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ioaumxww.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2iesrqzml.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nokqndpz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ffhndyan.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2chbaucbr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vgzhsrkw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dadmmezu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qwqthvkd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjovdahm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pbsxgbpo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2iqawdgzu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vxsmzohd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ouyidswn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vymqepqk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zifndqtc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2gdbzylqk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2luftkvfb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ajoplbsf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jtnqlkfe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bpbpvxbh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ykvitqev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulnpkfdt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2bkpsewpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbsmpwrf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2utsqvtcz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cstqtixw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eotridfz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gssaepti.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ggzvsdyb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tszqmjtc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2oabbvfnz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zslvqifh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zbgnjmtc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tuexyigi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2clqjntpi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2eiczpqzp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sawrcgly.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rrvzkgqs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pvotuyfk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jjypukuc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vpxbhywt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vrusccoo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zuznrxap.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2kinvabyl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxgiokeu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jbmidtxe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qrcjqrud.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iqxlgsjh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lftfywey.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xiapeytc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2narflwnm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mayesrul.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhvmwzn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2syndonzo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvehxiei.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2afomblud.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uiijjdbi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2uahnoook.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vjplxmvy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hkdxbwwo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qmjhompe.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wembgtiw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pymotkxz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zqkrlzih.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrrijqpl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2akmfxmjy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vqdkobpc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2etuoizwv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hkkqlbhy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cavibllz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rsmvhozl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbvydqjq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tavinghk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbjsfbp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctnhcfiv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2afzdenuh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxefcdwy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jhtmvprb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nbiqinoh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yypqxbop.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rjuprkmk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dviuksfj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hbthfjnj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbzhlojo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ciitcqpd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxnodfck.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpmfdlun.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rgpglrqg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2phnozozb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ngraixqh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qwrbgsjc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dbfylmja.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jfholihq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmajaey.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jnkozqiy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xosyfrrz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wwcolsaq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kcpxpwwj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyiwxevd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwnfidmb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2leyiwvii.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fqvfkebo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2anobeoqi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ubkkglkt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgnjfaj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bszgtafc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ztwkvvxm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2sjahwitb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lmtyzvrl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jbhtrizi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqlzrjpj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xkfhbfhg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wyxnjsbf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xbrvsqia.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ylrtwfxg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dvrlnzeg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2yeqtqlua.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gzpuygrq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uxlcuzok.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mwseppgz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xqcmwlci.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2irlnbgii.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sabjetkz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nfxrzcot.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ugkjjbji.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jgjigphl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rhnbtlmo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2trkzzcqu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2elxqtfeb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zwtmimkb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kunhjomd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2sgivcwux.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lgieufbt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2hazyazqj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iifcprrq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lrkoivbi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ppehsabs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zlqkwqrv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mmqzucki.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qtfkxwtj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vhvimcve.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2epoktpxa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2huybqvhy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lfvtbyyr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gorrsbfi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ondlcheg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxftrlod.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xvwvnnpu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvihngv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izpffchs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2iylwbhyo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tmgpxxjx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ncfyouvk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ibtvzsml.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qilaxvyp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2efkqflur.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cbtmmjzv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lidctwcd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qasppuvn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lockjohi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xxvnrics.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnawbatu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lsakksnc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ntuolktz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mhmfldie.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wnsappsa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2akwpdcsm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aoptnmxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksahrrjp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2spnsvcvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhkupoqh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ydngdfch.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hcoxnolv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajsfffwe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2azetygzi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygzwdcug.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2scxjadav.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hoxhibhu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kmxvvvcx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yyhdcrbt.html


<!-- 参考信息 -->