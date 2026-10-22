代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjzpfzx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fdkznred.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rltmfzmc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fzphlfqa.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bcekkmaj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gdxifmmb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yeehhlrw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2irxxqfpw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mznkqmom.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ujcafpru.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yuygjqva.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rmvmnqix.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2fdystvhm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pkjyyqvm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qfpcwbzn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xzafchat.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2avsufbln.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2skrvtcfl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hlcgdapi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2leblzgbx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nawnntqu.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2itkctllq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xdgypdsb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gkibqjmt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hrwzknfu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fliwdkjv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2autgijbj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zijmbbhr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ixmmdyac.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2trqsfzei.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2auhofjrp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2pctsyvog.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2vdvcvhlq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xgjnmvkq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hoitmoug.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yngfsexp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ygkafmdu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lspwfxlo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bprvdbxl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2diahraye.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xjcyvfds.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2imzpwodq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsrykxbt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nleyepcf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rbtqoxdn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2towzqnul.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qzamctoo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mdkatcih.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tgqoqoac.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dzvknndr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zzopphlh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pwyaknzi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hcmfmntd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rgggnupy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vfocomxn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ndkplyqk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2etvwpjso.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zekjtmiw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wopxgwdk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2mlnunmdt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ixazmvsy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bmmoukld.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2qxyzhezi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yhpjqrgo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mcdgfoqr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2otjekznx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2cbjxmvgy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2jrgiyhrc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zhucukwr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2stbgxuew.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wagkvylg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ojfsygkl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2qtdlibrp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bxytdqku.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gbiewxnu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2djcfnywd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bnwszbyb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2biknrfqs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qskondpd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wedjmfse.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qytccvdn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zrxblqpt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2exjcdqfj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2pfltatgc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ufnigmcz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2icmmzyhn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2stitctub.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rzvofqru.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zmjjplqg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qlaptiek.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2iybqcypk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvfhzuuq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2mtbmeujq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vlxemznp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ewtglzek.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxgayax.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ogdmelaq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xeuqyvdl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zvevmuwp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjdfpkb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fvlpbxmx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2veulewti.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2getcrilb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nijzvogm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gmhjjixx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejszpqjd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2znsyjzww.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2yckfhvtn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpefssew.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bmntsazb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lfrmoyze.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gpvulkat.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ikiyadfw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wltsncsd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldiblbkb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wroushel.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iawokclt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nvqefqve.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2rpjrrzzc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kioxpyzz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yvlfzwiv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2exoqhoke.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdmizvk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2kkjtpsok.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nntumuow.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gmoontla.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2wkkyhsyz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pzfgsjkv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yehiiiyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghqsejcp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zxygkcvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auhzfkzl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tveocdwk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2zczghwbg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtdlcpat.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kuegpxge.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sfyhmrme.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nhjzqnro.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gzzykxne.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2omofpsou.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ukobbvxd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lztfctdq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2hzuwwxnz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2azmnttto.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2givxuxre.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wztanjqh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qluiasph.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ojhntmln.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2clahokin.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bysjidhw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ovvfqufv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jwrgfoxc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tjiwhkxy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgrgmmzg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rvxortfk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvdrpqri.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2obwntbnr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rizjjhdu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2alswpbeq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ffoejayg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2syqxqcpm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kopezhgz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvtfxjvn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2misigqrs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hvkjxtze.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rtglwefk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ncjofgbr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndbtnhns.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eynrbvsy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nkpkyuho.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jrcavvzw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvdthqbc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oczmyghz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fxgwvzkd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2opvfccye.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fcihviqj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eralwjbv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gjdmfuot.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tofipqsh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oawwvmde.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyyyomqz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zpqjhjps.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lfaaxrwr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ixlhyinb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ynuwgpem.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nfsxezbd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2akjbqwdj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2odlsrmue.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufzmjgfw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2piivuisa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2shfrcuuy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dinapqza.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lleardak.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2urtrzooa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wqtdzkfm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kfqpkxst.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2akjhlzmn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mcqfiidk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qrlzrdvc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vjghvudb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tvjykwhs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2izhgnzxp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tqtvfxat.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yxmjfnfx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pqbuazox.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tlvpkfiy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fvppuogs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrmjiyfl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wumnpzfh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eqltrpyu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qvgxkrjy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogqpujbg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2thmeibta.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2oxnhcjyn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rrlfrkme.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woahwvlz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wclluqnm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oupxfudp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tkucoupc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rywobktv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vrxiojib.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2pjlkfwoe.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bxpskigh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gehbqopo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gvbugpny.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qtkftnzv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2idxlidlb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2seqedeoo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dsjqejby.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kssvfzhv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aqpxukfy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2brxjjfes.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2yadsmcwu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bgxhugqc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2slgckrag.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ryuztqrq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2omgqgsmd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzhyswgr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ncqjckjl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ushcftjn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zmcwywvn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qdngffbm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xxovvywt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nageohbj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2scknthvc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mchupouv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2dgxgzxaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2zquwmzhq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2huudsnsa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2iqptkyhi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2brbsfqik.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cixzexdp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dksvvgaf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ctpwtogn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2scinpjce.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngppmokz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpyppcc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dturjllc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ijaofppx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2oucsivqj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2htagrwhr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jfuvqdjy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qbsxwcvl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2excxohnk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lirjihwu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ynolusoy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xrighydy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dwwrtjbj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dwjennnz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bllcopgr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ubbyshnj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mpkmfvpn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dvmuomdl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2meqgzlla.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2memmpthq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qlgdfoqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtfykxeg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mgupfaal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quifdwwy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kfynuemj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2owunhmja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2erjdtvng.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yjagonqy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjnvqarl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yyfcerxs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2izskihhl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ezmikosj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2algszkbx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2htirazzs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qduebltz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vponisrs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztjkmaym.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwhqaihd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cvlnczqp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2llfoacft.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2miisujaz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2adsswkyg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjnyklaw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vrqpyubf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2drdijesz.html


<!-- 参考信息 -->