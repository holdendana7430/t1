代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtwenhjxrq.html

[A15] 空值判断与默认值
来源：http://hz.ppjwa.cn/gttjzlhfkj.html

Py:   value = data or "默认值"
来源：http://hz.yj202588.top/gtbgqxezpp.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.nwbrower.top/gtalcerrwo.html

JS:   const value = data ?? "默认值";
来源：http://hz.yangfankeji.com/gtzevkwwtq.html

TS:   const value = data ?? "默认值";
来源：http://hz.ybcxt.top/gtcqpkufxo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.gaohongyu789.top/gtetraxvag.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.nanxuanxn.top/gtqooqqahw.html

Ruby: value = data || "默认值"
来源：http://hz.shanyushiyangkeji.top/gtndfwjnac.html

C#:   var value = data ?? "默认值";
来源：http://hz.feifeiyinyue.top/gtqsbpxcky.html

[A16] 真假值判断规则
来源：http://hz.yj20258888.top/gtwiewgkcj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.dianchejie.cn/gtbnopqtut.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jinqigufen.top/gtrwhnxqts.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xuetiantiany.cn/gtabzquxnd.html

TS:   if (!x) {}
来源：http://hz.jinyuanbaomall.cn/gtfuztzkmp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yueranfly.top/gtgwnkbdxw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jinghuilouyu.cn/gtlrjccqzw.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ywan-chungtsiang.top/gtwrmxcdtl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.xziqi.cn/gtayaakrfk.html

[A17] 位运算
来源：http://hz.jinghuilouyu.cn/gtcrjeeyzt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gtdrsvxumc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhoulong.xyz/gtfjcanwim.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtxuqvmeck.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.316326.xyz/gthgdjekjz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ybcxt.top/gtyoxswbwn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtpeyaefon.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gtooualimn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtcwgmekls.html

[A18] 字符与 ASCII 码互转
来源：http://hz.hywenlv.cn/gtweqwrknn.html

Py:   ord("A"); chr(65)
来源：http://hz.svipenyu.cn/gtydjzuthq.html

PHP:  ord("A"); chr(65)
来源：http://hz.redwolf501.top/gtqrhfllwi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinyuanbaomall.cn/gtbomdpyyo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.haohaochexian.top/gtyvquuwhi.html

Java: (int) 'A'; (char) 65
来源：http://hz.wangdashe.top/gtwcqaxuaa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xziqi.cn/gtolleanpu.html

Ruby: "A".ord; 65.chr
来源：http://hz.ydjk.org.cn/gttopghbcl.html

C#:   (int)'A'; (char)65
来源：http://hz.cashguo.top/gtjvxmygdv.html

[A19] 交换两个变量
来源：http://hz.snrcjt.cn/gtntdrnnqg.html

Py:   a, b = b, a
来源：http://hz.ivvv.top/gtnukyslcy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yj20258888.top/gtbfhmbvwa.html

JS:   [a, b] = [b, a];
来源：http://hz.9152youxi.cn/gtzwvbtjol.html

TS:   [a, b] = [b, a];
来源：http://hz.yangfankeji.com/gtvpuzucxn.html

Java: int t = a; a = b; b = t;
来源：http://hz.sweek.top/gtspgfdrfw.html

Go:   a, b = b, a
来源：http://hz.yonumen.top/gtlcrlocwm.html

Ruby: a, b = b, a
来源：http://hz.zhijiandao.cn/gtoqcfsvyt.html

C#:   (a, b) = (b, a);
来源：http://hz.sysykeji.top/gtgpizvqcj.html

[A20] 读取标准输入
来源：http://hz.dashuyun.cn/gtkfklejzu.html

Py:   name = input("请输入：")
来源：http://hz.zhaomingkeji.xyz/gtdjmcumwg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cucudq.cn/gtyzhajmcp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhixingplan.top/gtjtecflrx.html

TS:   // Node.js：readline 模块
来源：http://hz.daria6918.cn/gtwytqrwfq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.guowangkeji.top/gtrvxaamuy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.gaohongyu789.top/gtanpdsszz.html

Ruby: gets.chomp
来源：http://hz.andypj.xyz/gtbgcaflix.html

C#:   Console.ReadLine();
来源：http://hz.hnxiangtu.top/gtttdrasqe.html

[A21] 保留指定小数位输出
来源：http://hz.gaohongyu789.top/gtjqdeemjc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.shanyushiyangkeji.top/gtlzwqjohr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtrlqchiyd.html

JS:   (3.14159).toFixed(2)
来源：http://hz.52xcode.cn/gtvsmtbihc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.fengsongda.top/gtiwmrqfod.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinghuilouyu.cn/gtcpgwqoqm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.gogol.net.cn/gtqtoaazcz.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ivvv.top/gtjbzhjboa.html

C#:   3.14159.ToString("F2")
来源：http://hz.svipenyu.cn/gthqtvfvke.html

[A22] 获取字符串长度
来源：http://hz.gotoacloud.top/gtdadvselk.html

Py:   len(s)
来源：http://hz.jiagoushi.top/gtuuqsqmqg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.tianlin.xyz/gtaerpvwws.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yuanzhike.top/gtguzjzdnn.html

TS:   s.length
来源：http://hz.hnxiangtu.top/gtiabkbret.html

Java: s.length()
来源：http://hz.gotoacloud.top/gtjrdpdzre.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.meibo888.top/gtvyerlvdh.html

Ruby: s.length
来源：http://hz.sysykeji.top/gtbyjtwhmp.html

C#:   s.Length
来源：http://hz.sufxvd.cn/gtfqwwzeaf.html

[A23] 大小写转换
来源：http://hz.sysykeji.top/gtblhtwpmu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jinghuilouyu.cn/gtelwofasb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.shangyingyoupin.top/gtfmemoihi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gogol.net.cn/gtyomdvpwo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj20258888.top/gtqjyjcomv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtfhmcosnf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cdnleiting.top/gtthjcikyv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jianghu66.top/gthkyyzrzs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jinqigufen.top/gtwgghrihu.html

[A24] 去除首尾空白
来源：http://hz.hnqzz.top/gtyxughjor.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.sxryk.cn/gtfjfeicxf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zhengqikj.top/gtnnvjnwcy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jianghu66.top/gturvkinxo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jiagoushi.top/gtumsqqimu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yuanzhike.top/gtfecvoadb.html

Go:   strings.TrimSpace(s)
来源：http://hz.guannengcc.top/gtjbffoyxt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hywenlv.cn/gthkjtbgbi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cucudq.cn/gtdawvhbtk.html

[A25] 字符串比较
来源：http://hz.ybcxt.top/gtozmgcitg.html

Py:   s1 == s2; s1 != s2
来源：http://hz.daxiang520.top/gtexbbkmxj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yj20258.top/gtdvpolpve.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.vqdsnc.cn/gtuwdcsgvl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yueranfly.top/gteykegzdq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xuanzx.com/gtiratjwyt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.daxiang520.top/gtofwofffc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yanxiufei.cn/gthwqrudsw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hnqzz.top/gtoobafkyu.html

[A26] 类型转换总览
来源：http://hz.pengpengdd.cyou/gtjskveiyc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.snrcjt.cn/gtvvxdurry.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hammf.cn/gtxybrtpeo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhoulong.xyz/gtspxrnyhm.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xingfuxueyuan.xyz/gtayyxqvzh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yj20258.top/gtqvuhnivq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jinyuanbaomall.cn/gthqzulbia.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.snrcjt.cn/gtflzbpzpf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yvedp.cn/gtwywnoxsa.html

================================================================================
来源：http://hz.hywenlv.cn/gtiizngjrm.html

B. 流程控制
来源：http://hz.cucudq.cn/gtazomgyhn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdhxrtwrj.html

[B01] 条件判断 if / else
来源：http://hz.tianlin.xyz/gthbhxhzyr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jqgufenzy.top/gtimvnwbiu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ehwqpu.com/gtzijrglut.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.svipenyu.cn/gtiyxvjozg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtdilqcrem.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zdqjudy.top/gtgaafwjrp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.feifeiyinyue.top/gtlisclcpb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhengqikj.top/gtootjjbwo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtnegnmwop.html

[B02] 多分支 else if / elif
来源：http://hz.daria6918.cn/gtlttqtzdk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.kuanghao11.cn/gtwdgrqfkt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.haohaochexian.top/gthcgwyprt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtjyvcsmlq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtvxdzloyg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cheryme.top/gtwdxqtztj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.redwolf501.top/gtdelhwgpo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.chenlongwang.top/gthirixdfi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gzhubu.top/gtaofzouwz.html

[B03] switch / match / case
来源：http://hz.xuanzx.com/gttitnijrd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fengsongda.top/gtitdcmxpe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.wangdashe.top/gtpbjsqkio.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gttjjyeyap.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cheryme.top/gtsobksjpz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.guowangkeji.top/gtrxqmzpbi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.iojbl.cn/gttcrvhhbu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.feifeiyinyue.top/gthvwzcyls.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jinqigfzy.top/gtpdkdjaod.html

[B04] for 计数循环
来源：http://hz.kuanghao11.cn/gtqtjcopsi.html

Py:   for i in range(10): print(i)
来源：http://hz.guannengcc.top/gtvxbxbwqz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yvedp.cn/gtofdkjtuf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhoulong.xyz/gtklbdqhpw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtwyanodax.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.daxiang520.top/gthdzdojxk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yvedp.cn/gtnscrlzth.html

Ruby: 10.times { |i| puts i }
来源：http://hz.fzhhl.top/gtadzsgkbd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.mhx1999.top/gtvclueyof.html

[B05] 遍历数组 / 列表
来源：http://hz.gogol.net.cn/gtwrhnusxa.html

Py:   for item in arr: print(item)
来源：http://hz.tian-w.cn/gtylogqnpr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenzaomai.com/gtjpxxhygf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtiwucuqqu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sweek.top/gtcgudleox.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.birdmap.top/gteuurszdh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.0kj1m.cn/gtabfmshkw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nanxuanxn.top/gtndraeyfc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yangfankeji.com/gtlgmkwlyb.html

[B06] 遍历字典 / 对象
来源：http://hz.cqqwz.cn/gtajxtpwyd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.guowangkeji.top/gtltmnkibs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jlsjyb.cn/gtrohwehww.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yonumen.top/gtinrskxvf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hysaishi.cn/gttmzbklav.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhiwuduotai.top/gtvfquvmnq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hammf.cn/gtsopuxvfj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ehwqpu.com/gtpaqwomcb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yongpay.top/gtnmoyanim.html

[B07] while 循环
来源：http://hz.yuxming.cn/gtfskjluoe.html

Py:   while i < 10: i += 1
来源：http://hz.hfpthk.cn/gtkojdofwm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gogol.net.cn/gtbjsonxdg.html

JS:   while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtimuxoxwq.html

TS:   while (i < 10) { i++; }
来源：http://hz.jiagoushi.top/gtaducrsmm.html

Java: while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtknjczlbx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.guowangkeji.top/gtynvcareh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jqgfzy.top/gtwdarvodh.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtwtxfgrdu.html

[B08] do-while（至少执行一次）
来源：http://hz.ivvv.top/gtqljzhhtr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gaohongyu789.top/gtzdblukss.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jqgufenzy.top/gtyknvfmbe.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtiqfgxwzx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtyourprmx.html

Java: do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtrvpjsyea.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj202588.top/gtodmfxret.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hongshengwenyu.top/gtylnrxxhz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gthacickow.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gtvnvyhiwo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jianghu66.top/gtsvqswnej.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cdnleiting.top/gtcsvzpnqk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtjawbueah.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtnxygetbn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtvecocorh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gtqjjbmqkv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ehwqpu.com/gthhvnxolt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtllvyvnxn.html

[B10] 遍历同时拿索引
来源：http://hz.cqqwz.cn/gtzqubrurm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xinyue.icu/gtmigiayjk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinyuanbaomall.cn/gtdkbnhjby.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.smart0.xyz/gtqhbzorhh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtisidcfoe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.meibo888.top/gtdozoopnz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.birdmap.top/gtepwglwkz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guowangkeji.top/gtoinfietu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinghuilouyu.cn/gtecnzziqt.html

[B11] 生成数字序列 / 区间
来源：http://hz.cdnleiting.top/gtrjkgwniy.html

Py:   list(range(0, 10, 2))
来源：http://hz.hywenlv.cn/gtazbstpus.html

PHP:  range(0, 10, 2);
来源：http://hz.c1oappe.top/gtcjltfwnk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtfhlgjgyq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hammf.cn/gtcvagozlq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.bjfxy.top/gtmbshuldg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zdqjudy.top/gtqweeygzv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258888.top/gtqcnsepei.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yonumen.top/gttbdkbayc.html

[B12] 跳出多层循环
来源：http://hz.ydzc1.top/gtxfjvhfvz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yongpay.top/gtuddnpkcq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jqgfzy.top/gtqlpwsilo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtoyyofskn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtxrbozwqb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtcmtvamcc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hnxiangtu.top/gtqiuphvxy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.wangdashe.top/gtpzaqvmbl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gtksrnztyx.html

[B13] 判断是否为数字
来源：http://hz.zhongyouzk.top/gtzkyhtqtn.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj20258888.top/gthwwfhzod.html

PHP:  is_numeric($x)
来源：http://hz.snrcjt.cn/gtrnawpstw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jianghu66.top/gtfexgbstd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258.top/gtprepwuwq.html

Java: x instanceof Number
来源：http://hz.jinqigfzy.top/gtuulzhcsn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.fzhhl.top/gtzewwjtsq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yvedp.cn/gtrrflvrdb.html

C#:   x is int or double or decimal
来源：http://hz.jqgfzy.top/gttncdbzcf.html

[B14] 判断值是否在集合内
来源：http://hz.fengsongda.top/gtfltwpaal.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangdashe.top/gtlxnsqxqk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ehwqpu.com/gtnvzsrixd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtesxmesbl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtaekcpcyq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tianlin.xyz/gtylmkzqnu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.aibaodan.cn/gtsnoxdrxo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ydzc1.top/gtsigrmbfd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.redwolf501.top/gtxjlahwpy.html

[B15] 布尔运算与取反
来源：http://hz.ybcxt.top/gtuyidfyih.html

Py:   a and b or not c
来源：http://hz.daria6918.cn/gtyhpkbodk.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258888.top/gtsezyfybd.html

JS:   a && b || !c
来源：http://hz.jqgufenzy.top/gtrcrjolzp.html

TS:   a && b || !c
来源：http://hz.gzhubu.top/gtwruhvgmt.html

Java: a && b || !c
来源：http://hz.jianghu66.top/gttavhwnax.html

Go:   a && b || !c
来源：http://hz.zhongyouzk.top/gtpeirtkkn.html

Ruby: a && b || !c
来源：http://hz.guowangkeji.top/gtcieyaxsb.html

C#:   a && b || !c
来源：http://hz.dianchejie.cn/gtfltsetfu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.52xcode.cn/gtvlfzataf.html

Py:   if not data: return
来源：http://hz.ywan-chungtsiang.top/gttdbdlfkw.html

PHP:  if (!$data) { return; }
来源：http://hz.yj20258888.top/gtxbywukam.html

JS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtprswenrq.html

TS:   if (!data) return;
来源：http://hz.havefunace.top/gtqqtmvbuq.html

Java: if (data == null) return;
来源：http://hz.nanxuanxn.top/gtawtigvnq.html

Go:   if data == nil { return }
来源：http://hz.wangdashe.top/gtisiqkgkc.html

Ruby: return if data.nil?
来源：http://hz.hammf.cn/gtjohmgrhm.html

C#:   if (data == null) return;
来源：http://hz.haohaochexian.top/gtmcdqzsct.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvvxqqqtz.html

C. 函数与作用域
来源：http://hz.cqqwz.cn/gtxmkexdqf.html

================================================================================
来源：http://hz.cucudq.cn/gtwyipzfga.html

[C01] 定义函数
来源：http://hz.yuanzhike.top/gtcaqwusmz.html

Py:   def add(a, b): return a + b
来源：http://hz.jqgufenzy.top/gtiaduppox.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtmpymnbnu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yongpay.top/gtlhrbvnow.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtdxzpzuvd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtklrumamn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtxzguzzvf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhongyouzk.top/gtxqokwyni.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtqwzvbisp.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtgsgovqwt.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangtech.top/gtcnjnfnrm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtcavhfxcm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tian-w.cn/gtzvunyqro.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtuxgrpgbs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuanzhike.top/gtlnytfsud.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gtxsnsrrzo.html

Ruby: def greet(name = "World") = name
来源：http://hz.sxryk.cn/gtnqmpxmdz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhijiandao.cn/gtqtffutap.html

[C03] 可变参数
来源：http://hz.birdmap.top/gtqzmpcexj.html

Py:   def total(*args): return sum(args)
来源：http://hz.svipenyu.cn/gtexkzuchp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zdqjudy.top/gtocijcrdd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtdhyhxucw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtesmftgcc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtgdzsxfgt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shzxlz.cn/gtnauxwcvt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangshuangyany.cn/gtkaafleqq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.smart0.xyz/gtuqebkoga.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cashguo.top/gtyqlursow.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtzskuzkvt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtqszwvgvw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hammf.cn/gtcauqhamt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.quarkkingdee.top/gtspysfghx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aibaodan.cn/gtutqjooyl.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxinkj.top/gtdxnaedff.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtlosbrcwr.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtbabeyhvm.html

[C05] 返回多个值
来源：http://hz.kuanghao11.cn/gtqwtpjfew.html

Py:   return a, b
来源：http://hz.ybcxt.top/gtixcmzive.html

PHP:  return [$a, $b];
来源：http://hz.birdmap.top/gtpxxuorsn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhongyouzk.top/gtgdmrndqs.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtsoqqxncf.html


<!-- 参考信息 -->