代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mxsfjmuq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lzmvkbxo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gvynkpxa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ndervtxm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3muhkwshc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3rvncjyqm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wzkjpxyn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3foyoywfj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xdbkemrb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sluiwolq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ydrjxgac.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zkuhkwol.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kvoewlrk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3drlurgoq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vwszgygt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ffubefcf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3uxjgxzpe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3wvanlikz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ybxraztx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ozdtzdwg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ypcuwhjq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3wgfmghrh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xirlbhwc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vthalczh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nilppzut.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ixcuhbxr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wjmzyxff.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dlwnwfer.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nxaoksyi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3blagcllp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hhegpfyv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jzklrpto.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mmedyojy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rlxxsbow.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3nzrauswd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zvnbgull.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3mdfzfxrp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ienorvdp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iapwzrik.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbgzjcbp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3mpsejbnq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ijmsfyqa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mcxvfenl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bkyvthlj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oqykxkek.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3asuwkijn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lnbbpluz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3grqtbwss.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnodmpfe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3brjxshba.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzedyqmn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uzdztfba.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3mjkmfhvf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dzxflkbu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3iuxiprle.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zzixrdmf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3pergwfks.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3boeffrfa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3tmbycfgo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3zokkehyk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cjrvahda.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3klicoiaw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ixkgmawo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3fzzsgvhq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ichjhomy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uhbiekyz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hpacdnzs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3obacvchr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mjigwlje.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3thcjtvsh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3aqkfxagi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zsojzyma.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zucogjgs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tmlylxbt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3aderpvvc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3dsluwffx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zqljzisw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3krpzhmrd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fuahpxan.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3zradaime.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3evglmnek.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eyvyuyps.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvybgiqf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlqrwtge.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kfzrwrsi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hxontqnv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ilgngbnz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3vmsthujf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qlfgluwe.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqgauqa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3coqreghh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3qdktjtub.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sapzycwq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zfpdtgtk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ghkcozna.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vqzoyafx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vyhjjpur.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nolwsoac.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dentxdzg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdcmzcyo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bpsirxfl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wgsudyxm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mlbtnkoy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogjgovrq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kflahrsz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ivdlzehi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3bfxlmssp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3frzwqvgo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ewrhonys.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eaoqqyvq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oerlrvqn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ufcnsjta.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhcucpde.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vcdflase.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hayrullf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3htayolgs.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3cwlybahb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zmhbpjjc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yndkhbwy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3njfvlqzy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcmyctbo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nqqjyzuw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3aeuaaryv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tibfoybw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3evbguzdc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yfejolkh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3sdtkaqrb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wlftaupp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3aaergbzf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vxowaoca.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rfbhsira.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yqyqjzkh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zpcdrftg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cugojmho.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vzixmnwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owddnzmb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rpsmmwfo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3njfmphwp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yevkbtar.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zdtzygpf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3txdzgthb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pdffclto.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3gbqlcpwl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vpmuuywz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3epztjwnt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xwryxrti.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xuictvqt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgkfurfh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fckvkurl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jsljsukx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tmpayfeg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ajtqvrtd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3spmxjjwj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrszsrsd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vaoqzosj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jqznabyw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifymjdhx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yyhckykd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eotqtuml.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mhjeikcg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pyvlxwwc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zdrsrzlb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3spjfpshr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dbibunvx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3njvdzeix.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvkwzkze.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aqhzekwc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wkhvdjtm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3omwqzshl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nmhkygus.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qjfnyefj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mtcukzvo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ehcormrb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xlarwtne.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yxljtydb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwucders.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3solqhexf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3npnvysot.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3edkuaiyc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lezdphfg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmriokuu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ykcxxiub.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vterqhim.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3opcvdota.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqrdtcs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrfemanm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjabjbym.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3efsolyfb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dkmtjrol.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kkaumuku.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kziyiiqw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ffflsbxx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dngazpkp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjliuucb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nknlhnzb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bnsbrxnz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ippbogdy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ngsosppp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lkpandan.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ytxolctk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bepowpfn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3trzarlhi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rtbrqthy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gvlkhctd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ngosuqid.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gyvhezct.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mryojmqc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xiiaosrr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gbpqcglv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3rseqdcou.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qqtgxgcc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nkbxiefp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bsbavwlk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fydkqbzh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mgaexgyc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cuhnqdjo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3patlbuyd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3oiztpzkg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpgkblv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oqyzkstf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3upzwfmgp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mddyambx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3eicamoeq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mvnwncom.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hcauerdt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxzglgwt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dhtfxjja.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ctzcmshe.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3riutkywz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3twldlerw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xrztwxcj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3tmhbnvbp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vhchrfcs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fbgfybtu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yanrnywx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rgcsgzdk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3sxwqpnxp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ijwgdjaq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jrvjdcyc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fravymjs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3taowvdiq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yvnwwhcr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rnarogyt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3shruytbh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lbkmhzfm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ukawkonj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3sonyjxnu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdlqwis.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmvoptz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xyzlnhbq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qhisnsqg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ybmxbxdi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kipicibl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3outngxcv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3snnjxdny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gnsyhjzc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rvupyhzs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxglodiq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dsqkatni.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ptxwaaif.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rtycdpeq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xnzxufbc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wehntnvp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3womdejdz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bzkqqpxm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pebwnvhy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sfkpwmpg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fcneirvc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mhmdpejo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wplyhluh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcgutuxc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oskxeyit.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zsuvfwcp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uuzdfhol.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3arpukdba.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjnpjcso.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xypkrxsn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ucnaldpe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zkdifefw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xjsyroxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grcmtukg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pjkpbglr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlsitsqi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdlpzeel.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vdgfvjrm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vyogqdki.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoyqdmdm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ninvsurp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tijyvbqp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3drdwvkjq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzovgxsq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dijvxbfu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqblzead.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zjmoqpmc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oudssxxf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyklnjv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3llzuyiye.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qwihkszp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3sekfkest.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3skztrrjw.html


<!-- 参考信息 -->