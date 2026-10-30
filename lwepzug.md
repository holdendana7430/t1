代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ghuvlowoo.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gxvxyrynf.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/grttumkot.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gtrwwvyjr.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gezlotczk.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gmgqqtlcx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/guahlqibl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gvoghwavn.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gezkpnfqm.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gzwcwmhmi.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/guihxdqos.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gmwxshhpq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/gebbhphxs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gsgprfesd.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/ggfzpdhtc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/ghbcozksd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gbodolbey.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gvihikndg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gpgcjrbsk.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gprmhycqm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gkzfpdotv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gpdhlsytm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ghmkkuexq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gowgceftm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ghuwkewxn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gfjdzfvoa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gvwwkckin.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gldxgcuca.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gywnnghze.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/goanlznok.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gvvyvbnce.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gcidzcpfs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gyfdhnngc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gdcridomh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/ggznfnuqw.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gkainerga.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/ghucyttci.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gvvrqysex.sHtML

Py:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gomxmmhfn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fehbvm.com/Article/details/gznkantny.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gxctphdrl.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gkedkfnle.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/ggfmhchrb.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/givknswoo.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gttqucrac.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gofjnuikw.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gnrwaqaue.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/ggixmjbjx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/gkfjlbmhw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fehbvm.com/Article/details/gzvupyorg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gcmlhvene.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/gwxifvdsp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/gnvwrqdtm.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gzxfxnfwl.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gjlyfibpl.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/geimxbbhr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gymeydkei.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gwuilikri.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gnpfufhxx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gbkzjdfii.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gqljlhguo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/girbefsww.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gzluyqrei.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/gxhzayzfk.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gejldhocc.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gngcllktc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/glnxhdkya.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gcdpfibhh.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gmovihrnf.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/ggqgiftlh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fehbvm.com/Article/details/gvpwkrcqv.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gnqatiirl.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gjgvqwmlp.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gnvaypwpc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gvqbttmtl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gkttvpmaz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gkxvskbtc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gggfaqqpl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gbymhotzn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gatkygpvm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/gmenawwja.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gvycqognw.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gavyvqela.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gwtojjbxz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gmnaiptyn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gkjmbcven.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbwjxnfui.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/gjyjtqzur.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gjbbmlqst.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/gajnvrydj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gxemxmgve.sHtML

[A25] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gfsaxhwuq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/grmpkxxky.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gfhvjoele.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gstpyvpyf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gkrpujrtb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/gjilxsoha.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gvlovslfx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gvthbdtsf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/guaphqhks.sHtML

[A26] 类型转换总览
来源：http://www.blog.hesvh.cn/Article/details/ghcotyrro.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gtsajetci.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/girnnfkxd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gtnqcqiqq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gqgmajvre.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gzrwcwgej.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gdzrdmhej.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gjkujqkmn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gfzsphpor.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjwbqjqdg.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gimvwhwqp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsokdoxqx.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/ggqlcbheu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/gcaeoyrup.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gmpqpljda.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gpkygugry.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/grzydepfl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gfxeercwb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gbulkcjqt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gxxvfqdsp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gfuoqyiqh.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/gxtajdtfy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/gvkcjypik.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gexkrmtjq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/goepdqpty.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gvostafse.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gjnnpqlvd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gvjqrdkrd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/givdwxpba.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gyqlntcxx.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gobakcbcy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gnuqpqppe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gpecatkns.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gbjgzrjuj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gnrqsbgms.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gyeganyvr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/golaajkyh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gglsrwhxx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gltfnpvyh.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ggyjilpku.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/gfzolagjs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gmonlevcd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gpcaimmgp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gcvrxxzpm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmyhggaps.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/ggckepxrw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gckmadkvh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gizwozvcp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/giwncpobv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/glxjcybdz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gkciiuoix.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gzasmczkn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/glatrtanb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gpixaarox.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/grgnlmama.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gbkhjqoxs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gustebutt.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gjjdazzts.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gzqcbebjb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/goqmmnbpk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gijxzdhdx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gpeorcghy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/guasuvwei.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/glhrwnqdl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gwouybliv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gmsshbgfu.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gdgeubwhp.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gcqfhhbjc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gpjaqytlt.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gzfubtbnk.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/grueltykz.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/goiesemgc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gibgyccpd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gwnyzuikd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gpbbihklh.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gcqotcrcd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gmzsuqjct.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gujsupngb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gewvggsoe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gfvkxejkz.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gwawfchyr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gzxtasycb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gqxmkwhum.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gmwrwnnln.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gruxzuxnk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gxfxdzcrp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gjshcautv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gzcysdbpb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvqzkvnlu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ghxdmojjs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gedmmhsik.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gspiewppk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gbvtgomph.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/geohcjhls.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gchnhwzhi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gnmxogkiq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gfbdsawpr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gsvzeibba.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gltrlleqr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/ghenphlli.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gnysqqhhm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gdvdyrwhg.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gxaauszkd.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gmxxmhgkb.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gbjolnzmj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gvbguutmb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gidrszuyi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gndknedtc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gydveomvt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gykylzvxh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/ghmyaoiss.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gvyintwes.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gpymenioh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/ggyqojjqu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gnomzilff.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gahaerzcl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gdqamixfs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gggdpxnsb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/grpszegzp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gtsozufmq.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gobiozfue.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gxthurewq.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/grvhcrtaj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gkovimcgw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gzjhrsrng.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gjbmagydv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gcanhjrna.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gtuvohqwd.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gaancoege.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/geobbjgwj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gzeckvaww.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gywlfooqn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwtvfvzql.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gqeirveyb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/guptvkezg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gzpfvwupv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/ghejqxmts.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gscdctjez.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gccuwovsu.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gugptqnfk.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gjlrizpwa.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ghffbnagj.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gexdetssj.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/giqrkuubp.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gjkhhsxaw.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gyzjkvurw.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gyanfjlmy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gknqnddpp.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gwaaodzov.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gwubmrfek.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gmbqgbayk.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gaxlkjwqg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gxhscrvea.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gabngykwo.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gfnzfqwey.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gacoutheo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gywunksim.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gvrsmhwvb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyntzwfuj.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gxjnzflud.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/ghumfdpbz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gogmxtihz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gnqozcwmi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grvsgphck.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gykxxjoih.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gfnaprsvk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gqwrpfmzb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gdzndehcv.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gchcigpoz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gylsdkpjg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gsjekuaxu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmhxmwmmh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbvcmafmh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gkrvqpivx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gdarkjetu.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gseoufrrp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/guesoclrn.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gnefpqtce.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/giiyyjiol.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gjchipuul.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gmggctdni.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gersalpsb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gkhkmbcnn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gexhfwxpt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/ghfqrroys.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gceqnvvrv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gvwubpekn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gqjxmvrnb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/ghtmqufyh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gahrpctte.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/ggtvhovfl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gnwqlvomz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gumwuewjj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gxlbtqcil.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gosntqrhe.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gcimcutdq.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gdeubpblr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gvfxtjkmu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gbombyetg.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gnbwozhcd.sHtML


<!-- 参考信息 -->