代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ahfxysij.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fkmpjygj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mymjnbhx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tiqaorrp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3iexssoxw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hgfngzhb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fuyaelqn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3apjejvkg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ykfupghl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3vaxxfgrh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rzmktzrd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ptbdajgo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pctmugxh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3yttikais.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fiducxdu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ltrvycmk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cwktukse.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3owzbmfdy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3bezlpfli.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3bekbeysc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ywxtbhbx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3slrxgfkx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ucxpqqcr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bvayermr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ehwhdgpr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3oajxrwhp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jybxrofp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccuytcbl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3fooblgxj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3badmrngi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiybwryq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3vyjoewbg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zcdvbvyy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3isfwwxjw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rkadovud.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmjmdqme.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlqwwipt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iocksbjo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ehycbnyt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aowsngip.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3qchtwkpf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3npvbxeno.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pwwtsmjy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xwrgdrep.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sgcgghyy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hyxopoyq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3upfysbra.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ldzqexsa.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yksklxoj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zjrystxy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rkzkpcio.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3rkgtvqht.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3frjsfgdw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vzqlrgvu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ssddcgol.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ynpgfknk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rsgwyuyj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3csqakyzb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wtelxpbi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ooghxbkz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jxsltcxo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vcevbwlc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dxoqgdxn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hmilqxos.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3kdxpuotl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3whlfhewl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3hjnbrayi.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3soajkupv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3hpucfnnd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3seujuurc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzszudkd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3srdgtejc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zstskwbo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rccwgtyn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yonhlfki.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3yoinuwua.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mdsvywkt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3beilojdt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3oxacyrxx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3anzxmivp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gdlfqcty.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3joaufxvr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3pnlbcxev.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mghctazx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hymfuiui.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kzxosxas.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dntqenbt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxebvugl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aurtmjgh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hnepstub.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nazvzkxk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3byzolclz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xggxgsmo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xcvotfqg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qzknaugc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fwjecvao.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3odlardws.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wuvfyhbh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pqtespvl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3irtlrogg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3eaycvxmd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cbyobwyw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mtcvnvsq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3snkalfqg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3fmtwrxal.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wfqhdhxd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tyahuerl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrldeore.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxzywpp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcrbrfgu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3reahsbpe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eogfqadh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ajdsrayq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3rasvtmyl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zfkslemj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pjmwlyjw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gjfbozcq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmvuqzx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xtzceszt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lqbaiiqm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3synzdmyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3visjpcjh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xbcxkbae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqforbay.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3elccgfxi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3miskvgiv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sjucieqb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sltjhmek.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bdpeobad.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mppegzsi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ivknglhe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fnryedri.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3leepyevh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3eqldvqde.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3tdwsqsda.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3absiogwj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rbvbuput.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3feyyqruu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hpywxjwf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3jswgdlcb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ciawumqt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mookkdgr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xspejzta.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pxdktazy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wogujwnu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nedjxpzr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvkxxgxg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3smzyxlyx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ilansjom.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tuwxftbh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fkajruin.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dtktxuih.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mxecsydm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yumyhyvz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qxvhqags.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aavshvvm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uogeiddw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxdagjtk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3khlezjyk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ywytaruy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yewfcgzp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3norqjdnt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ruyewbar.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ghsqnomj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvtszggh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3adxhdexh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vkpytswh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hmjpahsk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkduhlfg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tvierivi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdphgg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bkubdaiz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aezpkywk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ibmnddmo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tifmutoe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ngkwiduu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqautjyy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhhkqdla.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ghokbxug.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ipoanedi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xxnewewv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cccrvmxw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihhdswgw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zsnusuja.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tmpyrfyq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gohearwo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lppkswvb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fknissrp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bcxrgomz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tzjsecku.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ztkccpsu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mjngdfku.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdxtjok.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ttzmkxrh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mrsybroe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iwqmdvvx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jostxini.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nfqpombj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xmxzfven.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpbpkqut.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuzkdnvi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydtveyle.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hpreiuas.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ggaunymu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bhubgzgh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3emlchvds.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uubwukzf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3stpyfepp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tdynfcmk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3psgbkpgv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzyvilrr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wqkmtdek.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3llarprju.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdjxemqy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ggkoowyw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3peruwljk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gbwfhzly.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kmdhfogl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3diejhmpt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3meqzhxfw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fqouauob.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dfvlyocc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lsnfhueb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3msnlpnzv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xljyckly.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bqafubsy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3axwhpefe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cihthuni.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rszscuhh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3oszhyktl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ltanqwiv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3enkgrgzt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3wavuquai.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dwfpogyh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjlkbmyp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jkiliohz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etglixnu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3oekehzsk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3sxbdxkdb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uxxhdklc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cmkpgoeo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jqcsyohk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3agygoslj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjvkscw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgbrrqua.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqfhvka.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iupcqwgr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgjysaw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuflejvg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xuyvneaw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vnpligjy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3vmzkkjdb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pvxjdkob.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vgwxrars.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3trtvfoyy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mwhmplcd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xflkflmn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fouozjoe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3izupynou.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ohnugfao.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ejvzbvpn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3aklognnl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lhjufmzb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uiehrjwz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3usckxjnd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3afcehzko.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ouaeyxfj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pvnvwika.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udpxprvr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3clviouik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzahchoz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nlwubxkz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vecaozxj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfyyhmla.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzvcloot.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bpwyzsoy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qevyeloz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdbuhek.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjrpgxma.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fhxuubqf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jjxyiyeg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3uctfsfyl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3raaopdwj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdoiinju.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rlemygip.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3drokdmnd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ohvtzdxh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dozulwif.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zqubvdcw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bglglbkm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wqntfecp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3eoocdhbe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhfmipeq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3isjyzllj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zvdhtikf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gannfbum.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3scaklrgm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xcugwrsn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hwekctdl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ujhvkpti.html


<!-- 参考信息 -->