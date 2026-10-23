代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3toaxcyig.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rjnfnezj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nwmhgkjz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ybrazegk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yovroidv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xklbigqo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yxlqrjxl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdnqhyqw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jenyczff.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tbchcaeq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ieuyofyw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3oilsnszu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xidqisnx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hvwviaor.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wespkevh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hzssmztg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3lcwfbpdu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3gwvmkdds.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mzdkftls.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hxjsbszb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yvwepkqq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fiuultku.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rhvqxexp.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zdmkkefm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ckywicee.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ugthwiuw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vatiqlcs.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rfgomwcp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3bqaopsyl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vkfillod.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3unqqsdwr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3qzaucmvh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vzndibwk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3owkriglx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ihzdpvpn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3sdwcehcb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3sucwnpao.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yuoaawel.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qaooybyf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptblsqbd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hkagunrd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jovfhhka.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nnbxkwgn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3teyrxgye.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hxxtqmws.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzgobka.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3nwvvwpjk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3murzbvdw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hymeonjj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3beifdccy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3pqwjupnb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3amegawew.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qbqtvriu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3byvviijx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3yahfodau.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3eoykalsp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dwjdjfvs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gttkyooe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zzzkdecg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbnrzxqh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nlwfmcsk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wzxxuncb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3oyhkkchc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ttylhcyq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tuqkkunx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ioyxhpfk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aomokcih.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qxakrmrx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3apvipjko.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mkdjiabo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lffugjwg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qoipgevx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yozdcvrn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3flaqrayl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzydkny.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3klkkkedg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gwzrjjfp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ddivjgxj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fxxflhmr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oftpjltu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3njieuoyg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sezcsqts.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3snabxchj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yoamrywg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3smhvycxt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxjsknp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kfwnxhra.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bzloqdua.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3evdazmbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfmpnrti.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zvhoslsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wprbrjvm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xhustjux.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bkedsquo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ewminlqd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dfusxgvb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xoovletg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uoclodep.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kgdgzhsl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jkzhhtuh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3igomcqfe.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3edczojaa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hgwnyltd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wlyjnzfz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vahspnnh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bwkznocm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3varkxgto.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gmwepwks.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ivojtkux.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dlodcqbv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3lfdvqlkx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xvwnjtpj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cwkvguie.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3auhjkbzt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ffakrmff.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrynoxbu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3iwqtgybg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rvkmyyxh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xwbrvklh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpwotlss.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3apcfcqsb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jftnnakz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fcogduik.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ddseapbe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nntggxhd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3cogxxntk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jdddulbf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mnwtytfp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wqzptsjg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfssixd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdwcemlr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aagnqgbj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzerswzl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wzplpjor.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3aaiojttq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ccrxtudi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilststnx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bhhjiczu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3guizcfql.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mhrmtlul.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ysmbyixb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcsdzowf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cxwpjuya.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bclrttay.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3sjrwayqi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3isdduqqv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sfgcsorz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3glsruzbr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbtgqtzp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pdqjyuch.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fmmouhxh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xftcialh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vidrkfzm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3sdfpiptp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbplycxk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bfowjtbk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mxpjrelv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wfojospj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3noteheig.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tzmmuuhg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3imikapzg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3koqabyzz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mushbbjx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vjojxsap.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3smtwcnlb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rjwkltly.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fuaxqssz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hkloqkzb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qomjlwib.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhcmzeaj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bvqkfcem.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pvsvvqwi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kmqpenod.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xtrxffaq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tfmsdduv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mubgsgno.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3llsuefzc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xzespewh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wpkqdvfz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jyxzoppd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ehnbyxci.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqsohdly.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xvagorbh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zzziifmc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmwgxcje.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gizooxzh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pcbfwazb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzuwgjpy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wbmxjhbs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mxgkqpkr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eaucwkfh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vyhswljn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mfommsmx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jbqmlrfl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dyuizuuv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3asscdeqm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zilrftjd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3adbwbbcc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vzfrheww.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jfxwzzzz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lgbjcgtt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pizncxqv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcmfqili.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udkkrzgb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ahlszpib.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bhdvvokt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vvqzivxt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vbnjcqlg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xbcvflqq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nixwqhuy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3nyoxkege.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3swsxfgii.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdcngbd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3obmsxrsy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lhbzioma.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhlpcpww.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtybvcpd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxrvkiy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3pzrjzowo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fconkfvi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xcszrcnr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bombmtzv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sbvvlyew.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3arauxcpj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lzdswkgv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vszxlyda.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zfyvbbhk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ihmggqcg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fwrawflx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwlhmgsd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jljdtgml.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wrzyxvpn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fhyiadrb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hunznwhm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fsiydbns.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cccxlmmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcbmqsic.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3stfepiax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhosgkmk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zwdfvbyp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tqyiplsm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bncozyrv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ugvnoxey.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhewynfx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmykeypc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gaarlhoo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3iqhzjyfl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ospryluh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3svgbskjl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jfhazjbg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vjpmvqgw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqerzsyt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3htwdfxom.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yqyvhsik.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfylexib.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cxrebdzi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uwzglsef.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldphazdr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xddijayn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qqkhjmgm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3erwuqsht.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qyygtuje.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhnxhsg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tecyjjze.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fbgdubut.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jvigiqeo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3istizvua.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3joggzmws.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ccgsbjae.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3djvzexjt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ecfkwjnl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3syzwlpan.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bcnswysi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqoembi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvasvdg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ytafzlvg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3watcnrfj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3atwpogdw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gpdkatgp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3afjyqlcl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nplbffrk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3aryedcuq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hklhrsey.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sqdezsgv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lohgfgyp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3sreyadzz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3pgljgtlg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zcrohfpq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3crtmzjtm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3onmfbfcb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zccdihzg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xkslcpgo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rguirlxt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ijwdyoou.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3yqvmhhaq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qqsxkmsn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uqormydj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xavswzpv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3spzpxtwf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kucnhdtq.html


<!-- 参考信息 -->