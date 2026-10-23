代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rliiezkh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xizeckjw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fwhvtimu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dsyghnxt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hiinypvv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jhiirtwa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zfvinsxv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3swoedvir.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dpxbkyue.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3herimusz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vnfskuhg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kviprqud.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3wlgkokkh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3wsjkjcta.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eqegdgwq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qfwguudh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cfyddaub.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3nubqubep.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wswuzezz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3gjrjcqqu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3luitlgqy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sxjwfalr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nswlyfwi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ovgxxhxd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fxexqmlw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hrudnwev.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3xvjkxyqe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqovyycu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ovkhnzom.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ffxqqgye.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dmbvsgvz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xcqklyoe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ajonmude.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3jvokjfbl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xunanpwd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bomxlbbe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wokfeqsw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ikkpbuub.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cblbofjg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3klsvozyt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tortjzfu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nbulxkue.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3obcdwcqk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rafcckyk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hujemuuf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tahjtsho.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3duwfkqvl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ahakbcab.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3bgzehtjr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xqhlvgvt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xrqgyfar.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3psorhkel.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ccfuhmfw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3kgebgazf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ekvehhdq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3joenbywo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3wyofqklf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qeufrqry.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ugvhswpe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pubtuhjh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jqkwbzjo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bhterqoi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fklfyjlb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ogwlddli.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rfixbbff.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ihfnrzxk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wcjoaplp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3fjsnjuxf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mlnedpgj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3lkxwmlys.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3oudhtyjl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3rsuhxxig.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vdqqdude.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3caqsihym.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wcyiisxx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rxhfikmw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3muprwagb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wyrxinjq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3quvmttyh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yvpgzsap.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sqwktcwn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqjhxfs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbhzfpu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ncdnbudq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cdihtrug.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qnuaefxo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xgtttgue.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3utrgirci.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3plwyqzgl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gjigpnzr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctebpdyq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tiqlvbvq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ozyzpwqo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iyjwjnka.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3avnxqysx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqafwzw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nhiysjfx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dwtczwrm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3acoaekkn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kpkvuzzn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dzqlcoyw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ikcbbcog.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3njowfpbv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3oejmpnum.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jaqifjkv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zjnagqss.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ffiirvau.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3infnhery.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3gsoutxgk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jkvsqbhg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gkldoktk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3knstrimc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3nujidsrx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3habzsnkm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnensqgq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lvvfyvxb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujxufegy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nowgmmmw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nwcxgcjw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qwrwrflm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qisjwubr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3eroryfcp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qdbmhpfd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3fawabxez.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rkkypotr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3apyypobi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tzvdcdsk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3onobrwtf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bhdptakt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xitjnesq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3eqhedorz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjvrraci.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qmwdnpwb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uveowppc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxnmmidt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lkjpflex.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gtfffoou.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3znwxggon.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lzvwhsto.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ryisqppq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xggskjzl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pxubunyx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrztmnp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjofxnfs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gmnwsmkm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ktcyjcgc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mpwxfjfu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vslypamt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ammdrlqz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vbumwpsj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wuktyssb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3meuenqnp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ixlzkbmu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrykcuhd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tawusscp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tmszogke.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fjwaxzef.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fyxawdvw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3toqqwbza.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ezcgnufr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbxmhjx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fwvdjuzn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbkgljuy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zqmxrpjx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3bxrnfzry.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvbyynsq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3yvnsskfh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3khhvqzqd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xupxzxzx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qrlmikmo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ybkjlxop.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ykbbfpcr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsmduaul.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3bdosgqzd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bnruqyaw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3alwtugpk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eohwbsww.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3txiwgwhk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ojnvkbrr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdbxiedp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvvutvbf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohmgtwek.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3yafokpnl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jxvxoogz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3onsgpths.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxtupapz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3psfimxuj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hleqbijr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrntqdav.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3weuwupea.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tulseoln.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mmujdqgg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nuwxxjru.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lreuudbm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3shwigydy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vyrsfblx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dlryckdf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rxxxqkmx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eizzbudq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3woxwfrfk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3garbrnsq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jamjgvls.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fmnxzztj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vqzxmcnh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3igghglib.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bhoyiyef.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uleygawy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zgdbouyq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ruolrfrh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gngxeccu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ztopetpb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3obqvllcu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3etkflguz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yhvodjjv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3slcesskb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phwwohui.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qfebbwhn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wihxcmjv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mgtelozb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3udricamg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ctxtmeae.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpffurc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3yixzqmmb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3cyullgmd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3peksagvr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ozusudid.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zmmoxjmu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fhlrtdju.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jqpdpolj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mlbatspm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iimtkwys.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3amwdtznf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wvegcpdq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lepqmleu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3akococwb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lcrapduw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nkgfcblr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hewtvoqd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3akyhuwua.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jcoocqjm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3svsialsn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3isdbjnwt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hkttiabt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjujzvh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ewqsissb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lvhasbgw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gktaxxrp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nghhdrrs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hwhrlitu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3alkqqgiv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3orthesvp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hzoghxpl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3huawobph.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atkycdub.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqyidofz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zddeoskz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mhcbzrcl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kyggbejt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lhprjdjh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3aeadtpuq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jgbgpose.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vqpdpaop.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tydgvuwh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ujyhqhrz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pufmblps.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kgocnnhd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ielswrdy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gaagkvdg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mmngdatp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiuqqjiu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ifcrhzmh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qkkwywiu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3amfofbzz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hawmqenc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3azaujkqe.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mkceokug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvppfgox.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gsqctqzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmvdfgtg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3prthwppn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3sjovxbmb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3efuntsiz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trbqoibo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mifaojsv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3byjsueoa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3njipawta.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hcmbznfq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yekpfigk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qjcyfwvo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ngsusuek.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3snyrobjf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sjfibtkv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3itjmolyu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tfkssrxq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkkxmaii.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mfxzypak.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3cckqvjza.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rigdridp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kqwsgvdw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3odrdmahd.html


<!-- 参考信息 -->