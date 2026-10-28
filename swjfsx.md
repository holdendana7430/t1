代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.0kj1m.cn/gtdcfuweav.html

[A15] 空值判断与默认值
来源：http://hz.wangdashe.top/gthejgiyrb.html

Py:   value = data or "默认值"
来源：http://hz.mhx1999.top/gtxrrsdtmm.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jqgfzy.top/gtkrgginxu.html

JS:   const value = data ?? "默认值";
来源：http://hz.hywenlv.cn/gtbpdjgmsu.html

TS:   const value = data ?? "默认值";
来源：http://hz.ydzc1.top/gtzhqgvqxk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yj20258888.top/gtbzplaxob.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.havefunace.top/gtrpvzmtxn.html

Ruby: value = data || "默认值"
来源：http://hz.hammf.cn/gteibgytor.html

C#:   var value = data ?? "默认值";
来源：http://hz.xingfuxueyuan.xyz/gtgmgyheka.html

[A16] 真假值判断规则
来源：http://hz.mhx1999.top/gtjnzocdkj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.pycfn.com/gtmqodesgv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yangfankeji.com/gtrqeyryuf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhijiandao.cn/gtgiiadhuk.html

TS:   if (!x) {}
来源：http://hz.zhiwuduotai.top/gtrcplylji.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.feifeiyinyue.top/gtabuyvhbp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yj202588.top/gtuusgknzf.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.guowangkeji.top/gtyqcleroe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.cucudq.cn/gtulqqxlqb.html

[A17] 位运算
来源：http://hz.hammf.cn/gtadmhbmhy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtakccodyj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.52xcode.cn/gtpeyxkhya.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gttjqhsynp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.svipenyu.cn/gtfwnqcmbj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jiagoushi.top/gtlkohmcnh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtplxxllzq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtxltxltao.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fengsongda.top/gtspfvqtdk.html

[A18] 字符与 ASCII 码互转
来源：http://hz.chenjidiqi.icu/gttjqkuxkz.html

Py:   ord("A"); chr(65)
来源：http://hz.ehwqpu.com/gtmgcjeyta.html

PHP:  ord("A"); chr(65)
来源：http://hz.cheryme.top/gtkxgcdmyc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shuidangran.top/gtmtpjezlt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.meibo888.top/gtwkskglgj.html

Java: (int) 'A'; (char) 65
来源：http://hz.chenzaomai.com/gtwqdtejro.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.havefunace.top/gtzxwfpzzt.html

Ruby: "A".ord; 65.chr
来源：http://hz.andypj.xyz/gtmoqscrfg.html

C#:   (int)'A'; (char)65
来源：http://hz.cqqwz.cn/gtgxpognnx.html

[A19] 交换两个变量
来源：http://hz.yj202588.top/gtvsewzvpo.html

Py:   a, b = b, a
来源：http://hz.tianlin.xyz/gtithvvfcf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ehwqpu.com/gtgcbjjhmn.html

JS:   [a, b] = [b, a];
来源：http://hz.jiagoushi.top/gtezdbjhro.html

TS:   [a, b] = [b, a];
来源：http://hz.daria6918.cn/gtznroaxak.html

Java: int t = a; a = b; b = t;
来源：http://hz.cashguo.top/gtnsildhix.html

Go:   a, b = b, a
来源：http://hz.mhx1999.top/gtmuxlqjue.html

Ruby: a, b = b, a
来源：http://hz.andypj.xyz/gtrrzrcdie.html

C#:   (a, b) = (b, a);
来源：http://hz.aibaodan.cn/gtjtvbzrhv.html

[A20] 读取标准输入
来源：http://hz.gogol.net.cn/gtthvhmqdt.html

Py:   name = input("请输入：")
来源：http://hz.meibo888.top/gtkpbxlwyd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xuetiantiany.cn/gtnfbovzmd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.hfpthk.cn/gtcptlccvj.html

TS:   // Node.js：readline 模块
来源：http://hz.jiagoushi.top/gthxxykhzq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.birdmap.top/gtsytxoeue.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.tanke756.top/gtnffkorah.html

Ruby: gets.chomp
来源：http://hz.tian-w.cn/gtjwnlhatg.html

C#:   Console.ReadLine();
来源：http://hz.0kj1m.cn/gthyykcuer.html

[A21] 保留指定小数位输出
来源：http://hz.ydjk.org.cn/gtbvfzpxep.html

Py:   f"{3.14159:.2f}"
来源：http://hz.tianlin.xyz/gtynwegtmv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.pycfn.com/gtyrtxkifa.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xziqi.cn/gtzurctzzq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhiwuduotai.top/gtdvlkpyog.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinqigufen.top/gtgfcvfymu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jyoumei.cn/gtfchxzgyl.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yuanzhike.top/gtizgaafgo.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhijiandao.cn/gtmeqgoqbp.html

[A22] 获取字符串长度
来源：http://hz.xinyue.icu/gtporcipoq.html

Py:   len(s)
来源：http://hz.yueranfly.top/gtywhyfdgh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.nwbrower.top/gtssapzrve.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.tianlin.xyz/gtxtglcnug.html

TS:   s.length
来源：http://hz.snrcjt.cn/gtewpipmok.html

Java: s.length()
来源：http://hz.zhengqikj.top/gtogxxtqpl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sxryk.cn/gtlteftlwf.html

Ruby: s.length
来源：http://hz.snrcjt.cn/gtghtqhdsa.html

C#:   s.Length
来源：http://hz.kuanghao11.cn/gtblsjpwhy.html

[A23] 大小写转换
来源：http://hz.iojbl.cn/gtbcswmtiv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xziqi.cn/gtcghiwlmb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.0kj1m.cn/gtsguxkvxl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.bjfxy.top/gtpjlmykha.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.daria6918.cn/gtzmmjghpx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtaumsjlqe.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhengqikj.top/gtiizllhrs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.gogol.net.cn/gtvmykdwgv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yonumen.top/gttchkviaa.html

[A24] 去除首尾空白
来源：http://hz.bjfxy.top/gtlhwveuwa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.mhx1999.top/gtsdaoyavv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.shanyushiyangtech.top/gtggzldznr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sysykeji.top/gtdnspelwk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yonumen.top/gtrvesmzqp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.bjfxy.top/gtzovfuyav.html

Go:   strings.TrimSpace(s)
来源：http://hz.0kj1m.cn/gtxstlhezz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.gaohongyu789.top/gtocrwnnoh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ywan-chungtsiang.top/gtlbtctmfp.html

[A25] 字符串比较
来源：http://hz.meibo888.top/gtjdxoahkg.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hammf.cn/gtjzqfjqrk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ydjk.org.cn/gtsjkdtzde.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shangyingyoupin.top/gtpkcalitr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhoulong.xyz/gtmdvbohfr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zhiwuduotai.top/gtnbfocbbq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cdnleiting.top/gttqxzjkrg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.cheryme.top/gtjtrdudzu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jlsjyb.cn/gtjtoexqeg.html

[A26] 类型转换总览
来源：http://hz.yueranfly.top/gtewlthuci.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cqqwz.cn/gthefykwgh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhixingplan.top/gtyzghaznw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ppjwa.cn/gtnkggyyeh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.chenzaomai.com/gtncigpwqp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yonumen.top/gtrohrkisq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.tanke756.top/gtlqguskhv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shanyushiyangkeji.top/gtnxbrmouj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jianghu66.top/gtelcxubby.html

================================================================================
来源：http://hz.quarkkingdee.top/gtyuvroauu.html

B. 流程控制
来源：http://hz.guowangkeji.top/gtiqlkmowv.html

================================================================================
来源：http://hz.gotoacloud.top/gthkdoodam.html

[B01] 条件判断 if / else
来源：http://hz.zhoulong.xyz/gtvlptuxbp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.meibo888.top/gtplxmmhfq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yueranfly.top/gtpercjvkl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtxvcdylcs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shangyingyoupin.top/gtqxlsvimt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.iojbl.cn/gtuueicdtt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hywenlv.cn/gthprtgsvg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.fzhhl.top/gtwuyfylip.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jqgfzy.top/gtqrbtqier.html

[B02] 多分支 else if / elif
来源：http://hz.redwolf501.top/gtlvaehbjq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cdnleiting.top/gtvuymptxj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ppjwa.cn/gtuzzdctvk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtqlawjgrq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gtfgbwsamp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cheryme.top/gtpksmupqw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.wangshuangyany.cn/gtxtqebqoh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinyuanbaomall.cn/gtkexnruvz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yueranfly.top/gtomolckvh.html

[B03] switch / match / case
来源：http://hz.xuetiantiany.cn/gtwotnhgyb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shzxlz.cn/gtdowriacw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xuetiantiany.cn/gthpeqgrrg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.andypj.xyz/gttxrkhflb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.wangdashe.top/gtettngtgt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.snrcjt.cn/gtzozwksqw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ydzc1.top/gtuafhslzv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.xuanzx.com/gtpkkjavhu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.bjfxy.top/gtokjxlqxs.html

[B04] for 计数循环
来源：http://hz.smart0.xyz/gtzejzimrr.html

Py:   for i in range(10): print(i)
来源：http://hz.52xcode.cn/gtdqqocugi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gogol.net.cn/gtcsbyyttq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ybcxt.top/gthmurwrkw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.daxiang520.top/gtacodvhwv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nanxuanxn.top/gtxlvvqefa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.52xcode.cn/gthtuwemio.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yvedp.cn/gtmyacocbb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.feifeiyinyue.top/gteoiygzzn.html

[B05] 遍历数组 / 列表
来源：http://hz.dianchejie.cn/gtpkleukgc.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangkeji.top/gtwbuibhwf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.haohaochexian.top/gthoogzmla.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinqigufen.top/gtxyqdgrik.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yueranfly.top/gthmhnusac.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.guowangkeji.top/gtcnitylzp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhijiandao.cn/gtciidywqz.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nanxuanxn.top/gtvmfwwpqf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.c1oappe.top/gtgxypofuq.html

[B06] 遍历字典 / 对象
来源：http://hz.hnqzz.top/gtmzzlfxfy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ivvv.top/gtmafxbvms.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yonumen.top/gtmbhlosyj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nwbrower.top/gtczckepdv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gtvvpgllbc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.c1oappe.top/gtqvjgmxmi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.dashuyun.cn/gtvdhfjnse.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinqigfzy.top/gteazovfhe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hammf.cn/gtafvqcjmi.html

[B07] while 循环
来源：http://hz.yj20258888.top/gtrptrowjc.html

Py:   while i < 10: i += 1
来源：http://hz.pycfn.com/gtnlwwgfkc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuxming.cn/gtwvtxkrdd.html

JS:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtblzxdwwq.html

TS:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtjexctgxx.html

Java: while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtqkiuhref.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhiwuduotai.top/gtvixnwail.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinyuanbaomall.cn/gtjtsxfdun.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtixdxonpd.html

[B08] do-while（至少执行一次）
来源：http://hz.zhijiandao.cn/gtkzzvrtlv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nwbrower.top/gtbfibthss.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhongyouzk.top/gtwvsvqwii.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtskrimeco.html

TS:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtyiixneyt.html

Java: do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtdgbrqfhu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ppjwa.cn/gtvlkavllm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hfpthk.cn/gtcbrewbsi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtxxasxeve.html

[B09] break 与 continue
来源：http://hz.xuetiantiany.cn/gtpvcrfazi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydjk.org.cn/gtnooqawbl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.meibo888.top/gtlylgxcsj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtimqqxhhw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtzaneezsf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtiqvptvlg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hongshengwenyu.top/gtqlhsooxm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinyuanbaomall.cn/gtnbiuyxbo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtoxyyczdw.html

[B10] 遍历同时拿索引
来源：http://hz.tanke756.top/gtaranbmgc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangtech.top/gtmaklfgic.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sysykeji.top/gtslxorpmb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtefaffnhb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.316326.xyz/gtsaxqmsgv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cheryme.top/gtyoctdcuu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yonumen.top/gtqojnwzxo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cheryme.top/gtythjepqh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhiwuduotai.top/gtflcmdohh.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgufenzy.top/gtcjvuzvny.html

Py:   list(range(0, 10, 2))
来源：http://hz.havefunace.top/gtrvuxokxa.html

PHP:  range(0, 10, 2);
来源：http://hz.andypj.xyz/gtzfpzytqi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hfpthk.cn/gtyxqscdeb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtujbxoysn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuanzx.com/gtwwbnpsnz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.nwbrower.top/gtaehznqat.html

Ruby: (0...10).step(2).to_a
来源：http://hz.9152youxi.cn/gtkcxegsrr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj202588.top/gtrvsobrmu.html

[B12] 跳出多层循环
来源：http://hz.pycfn.com/gtexupontg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xziqi.cn/gtunbjyxnr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tianlin.xyz/gtsmaohfmq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtrrotkuut.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gteugohbkr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtjsxhprkk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhongyouzk.top/gtbmfytfss.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenlongwang.top/gtnglgxxyd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gtovqyqjuk.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtmdlxthzg.html

Py:   isinstance(x, (int, float))
来源：http://hz.ybcxt.top/gtcljvyvio.html

PHP:  is_numeric($x)
来源：http://hz.yj20258888.top/gtcaurjkox.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtyxrqaofx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aizwys.cn/gtmhqcnxgb.html

Java: x instanceof Number
来源：http://hz.daria6918.cn/gtcudngtxs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daria6918.cn/gtbyexolga.html

Ruby: x.is_a?(Numeric)
来源：http://hz.andypj.xyz/gteeleackd.html

C#:   x is int or double or decimal
来源：http://hz.pycfn.com/gtjkbmolex.html

[B14] 判断值是否在集合内
来源：http://hz.iojbl.cn/gtftozctqp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ydzc1.top/gtonlgmtfu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yueranfly.top/gtarxmfpcd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtecbpqdhr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sysykeji.top/gtdjudapyg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xinyue.icu/gtazbbpkaq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.haohaochexian.top/gtgikdzson.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhixingplan.top/gtztlawkve.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shzxlz.cn/gtohowebmu.html

[B15] 布尔运算与取反
来源：http://hz.shangyingyoupin.top/gtzaeneqnf.html

Py:   a and b or not c
来源：http://hz.jlsjyb.cn/gtzvizgytp.html

PHP:  $a && $b || !$c
来源：http://hz.birdmap.top/gtpfiiinlb.html

JS:   a && b || !c
来源：http://hz.guowangkeji.top/gtxzthvtvm.html

TS:   a && b || !c
来源：http://hz.daxiang520.top/gtndzaeyag.html

Java: a && b || !c
来源：http://hz.zhoulong.xyz/gtxxhawisz.html

Go:   a && b || !c
来源：http://hz.daria6918.cn/gtbxwggptv.html

Ruby: a && b || !c
来源：http://hz.jqgufenzy.top/gtfsbuvorq.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gthomuwsek.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shuidangran.top/gtvzilnlyj.html

Py:   if not data: return
来源：http://hz.mhx1999.top/gtenmypcdm.html

PHP:  if (!$data) { return; }
来源：http://hz.chenjidiqi.icu/gtltcumbxy.html

JS:   if (!data) return;
来源：http://hz.tian-w.cn/gtqrarbaez.html

TS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtikitxjcj.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtiakjnfix.html

Go:   if data == nil { return }
来源：http://hz.sxryk.cn/gtlyizflzm.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gtiucnddsq.html

C#:   if (data == null) return;
来源：http://hz.xylfe.cn/gtgyswbkgn.html

================================================================================
来源：http://hz.fengsongda.top/gteqcqtwle.html

C. 函数与作用域
来源：http://hz.zhongyouzk.top/gtirxwzazg.html

================================================================================
来源：http://hz.bjfxy.top/gtvwmjgmdi.html

[C01] 定义函数
来源：http://hz.gotoacloud.top/gtlxtaylsy.html

Py:   def add(a, b): return a + b
来源：http://hz.jiagoushi.top/gtabdlkeqp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gttzzqoecm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtfattiqzd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.52xcode.cn/gtfyyewhjg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtqjlrsaju.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hammf.cn/gtufowgard.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sxryk.cn/gtadgidwza.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtoronopof.html

[C02] 默认参数
来源：http://hz.c1oappe.top/gtdrrulijl.html

Py:   def greet(name="World"): return name
来源：http://hz.jinyuanbaomall.cn/gtncctmhnk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gtuyrayoan.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhixingplan.top/gtkvxiunwl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgufenzy.top/gtfkthrunt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.guannengcc.top/gtcesevdlv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhongyouzk.top/gtpzwzzrvj.html

Ruby: def greet(name = "World") = name
来源：http://hz.tianlin.xyz/gtlbixzhha.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yongpay.top/gtufcvuvbk.html

[C03] 可变参数
来源：http://hz.cashguo.top/gtfvfhwzoj.html

Py:   def total(*args): return sum(args)
来源：http://hz.zdqjudy.top/gtjcvylptb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gttgiiggtf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtrxfbcuku.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtwmzgehmk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cucudq.cn/gttjkfwsrn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtrndzwajv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yongpay.top/gtfxcqycxg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtffduqrlz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gthggxerqq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daxiang520.top/gtvqgeetah.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.c1oappe.top/gtlfxhoriz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtrriawkyg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangshuangyany.cn/gtupylgjnz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.bjfxy.top/gtpalatdtr.html

Go:   // 无：用配置结构体参数
来源：http://hz.nwbrower.top/gtbsrahdho.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtxtbnfxog.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtuhuvtpux.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtlrzujoyb.html

Py:   return a, b
来源：http://hz.vqdsnc.cn/gtdnlshlgm.html

PHP:  return [$a, $b];
来源：http://hz.yvedp.cn/gtdvkbpqpi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ivvv.top/gtrlyhmidi.html

TS:   return { a, b };
来源：http://hz.xziqi.cn/gtvnfqmsxc.html


<!-- 参考信息 -->