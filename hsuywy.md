代发 wailian999

[A14] 注释写法
来源：http://hz.xziqi.cn/gtdpnajccj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yuxming.cn/gtufvhdgck.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.fzhhl.top/gtjuokzomu.html

JS:   // 单行；/* 多行 */
来源：http://hz.ywan-chungtsiang.top/gtnzepbpvq.html

TS:   // 单行；/* 多行 */
来源：http://hz.zycfv.cn/gtmvrojyon.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.cheryme.top/gtptphcrtr.html

Go:   // 单行；/* 多行 */
来源：http://hz.yj20258.top/gtrgeiluji.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhongyouzk.top/gtdblzitis.html

C#:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtyergombr.html

[A15] 空值判断与默认值
来源：http://hz.sxryk.cn/gtwpbkwlgy.html

Py:   value = data or "默认值"
来源：http://hz.jlsjyb.cn/gtowexbeat.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.cqqwz.cn/gtlxwjvahx.html

JS:   const value = data ?? "默认值";
来源：http://hz.yvedp.cn/gtgakrbwou.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhixingplan.top/gthrsxwdzc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shzxlz.cn/gtlorbafkb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.hammf.cn/gtqflgjpdi.html

Ruby: value = data || "默认值"
来源：http://hz.zhongyouzk.top/gtccyupkip.html

C#:   var value = data ?? "默认值";
来源：http://hz.vqdsnc.cn/gtgzwcgymk.html

[A16] 真假值判断规则
来源：http://hz.cdnleiting.top/gtqxcldfxc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.haohaochexian.top/gtpqczaqzq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jianghu66.top/gtyzwgreaz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhoulong.xyz/gtvtgfiekq.html

TS:   if (!x) {}
来源：http://hz.hfpthk.cn/gtrdggzkqu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yueranfly.top/gtnnrwoclj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jyoumei.cn/gtlnoijmfl.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.chenjidiqi.icu/gthreybbkm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.kuanghao11.cn/gtzadzmgwx.html

[A17] 位运算
来源：http://hz.jinghuilouyu.cn/gtybrngrlz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtzkbbschw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.mhx1999.top/gtcojhgfxd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtdipieces.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtmkfcrklm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pycfn.com/gtpmsstifk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtxwmzthfs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gtwsmocwbi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtbxggonol.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhengqikj.top/gtafwrdpjq.html

Py:   ord("A"); chr(65)
来源：http://hz.ybcxt.top/gtogfhugpe.html

PHP:  ord("A"); chr(65)
来源：http://hz.gogol.net.cn/gtebcsgxdz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenlongwang.top/gtgemfrkiv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jianghu66.top/gthteyxzls.html

Java: (int) 'A'; (char) 65
来源：http://hz.aibaodan.cn/gtbodukksr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zhongyouzk.top/gtuepmiybf.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhixingplan.top/gtnsxiuebp.html

C#:   (int)'A'; (char)65
来源：http://hz.yanxiufei.cn/gtvtbbmnof.html

[A19] 交换两个变量
来源：http://hz.zhijiandao.cn/gtesbsqpki.html

Py:   a, b = b, a
来源：http://hz.jinqigufen.top/gtdscadsrn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.0kj1m.cn/gtcmydcfkb.html

JS:   [a, b] = [b, a];
来源：http://hz.hnxiangtu.top/gtzzjeufwk.html

TS:   [a, b] = [b, a];
来源：http://hz.andypj.xyz/gtypmbzlxp.html

Java: int t = a; a = b; b = t;
来源：http://hz.xylfe.cn/gtncgwnpuy.html

Go:   a, b = b, a
来源：http://hz.daxiang520.top/gthbxfblby.html

Ruby: a, b = b, a
来源：http://hz.zhaomingkeji.xyz/gtuzuvggbk.html

C#:   (a, b) = (b, a);
来源：http://hz.hywenlv.cn/gtdvtghscq.html

[A20] 读取标准输入
来源：http://hz.xuetiantiany.cn/gtseyzgpyy.html

Py:   name = input("请输入：")
来源：http://hz.sweek.top/gttphvzohh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.sxryk.cn/gtkpsvaelf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xuanzx.com/gtbkvfijeu.html

TS:   // Node.js：readline 模块
来源：http://hz.c1oappe.top/gthlibpalc.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jiagoushi.top/gtfipmyipx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.chenzaomai.com/gtxcgqqjcy.html

Ruby: gets.chomp
来源：http://hz.cqqwz.cn/gtjottxdaz.html

C#:   Console.ReadLine();
来源：http://hz.zhoulong.xyz/gttzmjowwa.html

[A21] 保留指定小数位输出
来源：http://hz.wangdashe.top/gtkueoomrm.html

Py:   f"{3.14159:.2f}"
来源：http://hz.9152youxi.cn/gthlvmpzgd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.chenzaomai.com/gtxclgjzkm.html

JS:   (3.14159).toFixed(2)
来源：http://hz.kuanghao11.cn/gtshtgharx.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jlsjyb.cn/gtjerydguj.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhoulong.xyz/gtjnzxvpug.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.9152youxi.cn/gtebtwqqrj.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtiyhybxsz.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj202588.top/gtqqxulweb.html

[A22] 获取字符串长度
来源：http://hz.pycfn.com/gttgglcaok.html

Py:   len(s)
来源：http://hz.0kj1m.cn/gtlacuinji.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.pycfn.com/gtvyfxetgw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hnxiangtu.top/gticuopens.html

TS:   s.length
来源：http://hz.c1oappe.top/gtrkqdnvop.html

Java: s.length()
来源：http://hz.zhengqikj.top/gtxmeezoku.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cdnleiting.top/gtzshvopta.html

Ruby: s.length
来源：http://hz.zhaomingkeji.xyz/gtuyqioybl.html

C#:   s.Length
来源：http://hz.tianlin.xyz/gtgofdquaa.html

[A23] 大小写转换
来源：http://hz.tianlin.xyz/gtuhvacdqh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.shanyushiyangkeji.top/gtdaykywmw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.jinghuilouyu.cn/gtotmdkiji.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.9152youxi.cn/gthsxcpnch.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.quarkkingdee.top/gtkalvyyla.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.aizwys.cn/gtuzampghk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jqgufenzy.top/gtmdkqscia.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.snrcjt.cn/gtcceevzth.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.bjfxy.top/gtkeryhvhn.html

[A24] 去除首尾空白
来源：http://hz.xinyue.icu/gtcaobzjbq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.redwolf501.top/gtosvygxfw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hysaishi.cn/gtwajiuluo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhengqikj.top/gtthowbsir.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xinyue.icu/gtcfsvanty.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ivvv.top/gtvnrpsggr.html

Go:   strings.TrimSpace(s)
来源：http://hz.nwbrower.top/gtxwtmhgop.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jqgfzy.top/gtzwjcvimh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.tanke756.top/gtuodyhepy.html

[A25] 字符串比较
来源：http://hz.quarkkingdee.top/gtmzqnriqb.html

Py:   s1 == s2; s1 != s2
来源：http://hz.c1oappe.top/gtzmosldxt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jyoumei.cn/gtdkgoausk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ppjwa.cn/gtvshlyqro.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.smart0.xyz/gtvjlykxuk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.fzhhl.top/gtyjcdnmhl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.9152youxi.cn/gtjepbedhp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.haohaochexian.top/gtpgzlsisp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gzhubu.top/gtfeopdskg.html

[A26] 类型转换总览
来源：http://hz.nwbrower.top/gtbnhxssrd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jianghu66.top/gtomxdzfqq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hysaishi.cn/gtsvtagwgw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xziqi.cn/gtlyrfwfrp.html

TS:   Number() String() Boolean() x as number
来源：http://hz.hnxiangtu.top/gtpuktcslg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhongyouzk.top/gtgygjfidp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.bjfxy.top/gtswwsufon.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.cdnleiting.top/gtmjzrqqbe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.guowangkeji.top/gtmuiamjex.html

================================================================================
来源：http://hz.52xcode.cn/gtdwwsskfc.html

B. 流程控制
来源：http://hz.ywan-chungtsiang.top/gthcvlmagr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzvkvpsva.html

[B01] 条件判断 if / else
来源：http://hz.yj20258.top/gtcgscixxl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinqigufen.top/gtzycmfcmv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jiagoushi.top/gtobfuzuap.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.svipenyu.cn/gtpunudifs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigfzy.top/gtocuxlbtu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258.top/gtawcuphav.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hnqzz.top/gtjtssglro.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tian-w.cn/gtwhaodcqy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtuncslpxh.html

[B02] 多分支 else if / elif
来源：http://hz.ywan-chungtsiang.top/gtloihvxnv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xziqi.cn/gtxgiclwgl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.52xcode.cn/gtxnroyvmn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtwxhwvsmt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ybcxt.top/gtmfyanbsj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtrbduklqq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.chenlongwang.top/gtknueiezx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.aizwys.cn/gtngmrfnmd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gtqgjlqwfz.html

[B03] switch / match / case
来源：http://hz.jinghuilouyu.cn/gtqhmunnar.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sweek.top/gtkxkygcsj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xinyue.icu/gtskhkdrwk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sweek.top/gtbiiqeaiy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxuanxn.top/gteuyjbfyw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jianghu66.top/gttzhbwakg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.gogol.net.cn/gtfvaxdcip.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.nanxuanxn.top/gtzoeusozj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.tianlin.xyz/gtwljtvdxu.html

[B04] for 计数循环
来源：http://hz.yonumen.top/gtqokshmws.html

Py:   for i in range(10): print(i)
来源：http://hz.yj202588.top/gtytzzvelb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jinghuilouyu.cn/gtpjespnko.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xylfe.cn/gtvbzytmlb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.9152youxi.cn/gtwfwsiqjv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.redwolf501.top/gtkqgnbhii.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ppjwa.cn/gtqnsduvyz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shanyushiyangkeji.top/gtaegxxpax.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.chenlongwang.top/gtlasxpyzw.html

[B05] 遍历数组 / 列表
来源：http://hz.wangdashe.top/gtoqsoavgo.html

Py:   for item in arr: print(item)
来源：http://hz.cucudq.cn/gthkmqlxmz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhiwuduotai.top/gttgeahwji.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xuetiantiany.cn/gtmbtfrvnl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtascjgvza.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.fengsongda.top/gtbrjneqiv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhaomingkeji.xyz/gtgtrwyedu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ivvv.top/gtdsntoxtu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.aibaodan.cn/gtqpsokybf.html

[B06] 遍历字典 / 对象
来源：http://hz.nwbrower.top/gtjrnffwke.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuanzhike.top/gtyscnhijg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ywan-chungtsiang.top/gtjjyeykwm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258888.top/gtktthgues.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gaohongyu789.top/gtwignigdm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zycfv.cn/gtiimttuhz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jqgfzy.top/gtclilqoye.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.mhx1999.top/gtcrtvczyo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cqqwz.cn/gtgoucvcoj.html

[B07] while 循环
来源：http://hz.yj20258.top/gtutjusxnu.html

Py:   while i < 10: i += 1
来源：http://hz.smart0.xyz/gtquvpzwsr.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.nanxinkj.top/gtvzfngpir.html

JS:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtdtubbrxx.html

TS:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtsdjziurq.html

Java: while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtiaiwbiru.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.nanxuanxn.top/gtbdbqbptu.html

Ruby: while i < 10; i += 1; end
来源：http://hz.pycfn.com/gtdqoncppx.html

C#:   while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtnguenhki.html

[B08] do-while（至少执行一次）
来源：http://hz.yuanzhike.top/gtiqsatrsz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xinyue.icu/gtplogwtxu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.fzhhl.top/gtneikcjvt.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtlaznvwqu.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtndaczygi.html

Java: do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtlesykymx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hammf.cn/gtcvxydodp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hongshengwenyu.top/gtehekkzkp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtqimaocud.html

[B09] break 与 continue
来源：http://hz.ybcxt.top/gtiwlibqtn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xylfe.cn/gtqgznbtyh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.pycfn.com/gtodurxmsx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtxclayuok.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtcrhcvmeu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gtnsagidla.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xinyue.icu/gtjrvpcmso.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgfzy.top/gtjvdtqrxn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gtvgbgvrqf.html

[B10] 遍历同时拿索引
来源：http://hz.snrcjt.cn/gtnexkhjjd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cashguo.top/gtkxkqtczf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xuanzx.com/gtsacztnne.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtthodzogr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtxakfzrhk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yuxming.cn/gttxrpnkdd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangshuangyany.cn/gtetrlecfh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.redwolf501.top/gtxdceegkw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinghuilouyu.cn/gtkcvmumxi.html

[B11] 生成数字序列 / 区间
来源：http://hz.jianghu66.top/gthstpexqz.html

Py:   list(range(0, 10, 2))
来源：http://hz.vqdsnc.cn/gtomtmhgzd.html

PHP:  range(0, 10, 2);
来源：http://hz.redwolf501.top/gtmvrafros.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtcijzuhzn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtxvayqzem.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenjidiqi.icu/gtxrnsucnc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gthwusgaie.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258888.top/gtwnfbpavx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.9152youxi.cn/gttvuzzxaf.html

[B12] 跳出多层循环
来源：http://hz.yvedp.cn/gtjebytbeq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.52xcode.cn/gtdosufbay.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhoulong.xyz/gtmjjyiufu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtkhbrgqrx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtneqfsubi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtrukfemtq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jqgfzy.top/gtkokpwxhj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sweek.top/gtafjpvbcy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ywan-chungtsiang.top/gtxddfimiy.html

[B13] 判断是否为数字
来源：http://hz.cheryme.top/gtfpxfwxyx.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhaomingkeji.xyz/gtmhhjqtns.html

PHP:  is_numeric($x)
来源：http://hz.aibaodan.cn/gtehqhhtix.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gotoacloud.top/gtokchkncy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtccacoeft.html

Java: x instanceof Number
来源：http://hz.chenzaomai.com/gtxormpogk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.snrcjt.cn/gtlvksbmas.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ivvv.top/gtykykevfs.html

C#:   x is int or double or decimal
来源：http://hz.dianchejie.cn/gtjodkiuzu.html

[B14] 判断值是否在集合内
来源：http://hz.shzxlz.cn/gtfcdmuwlj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuetiantiany.cn/gtaihshwtj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.quarkkingdee.top/gtjciijyps.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ydjk.org.cn/gtmynxehlr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtfqxxlkzx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sweek.top/gtjhxpuwfk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hammf.cn/gteennvhvx.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.iojbl.cn/gtdmcertoc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yanxiufei.cn/gtvmklieks.html

[B15] 布尔运算与取反
来源：http://hz.chenzaomai.com/gtlvscofns.html

Py:   a and b or not c
来源：http://hz.fzhhl.top/gtzadvybmp.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gthuaqkjjn.html

JS:   a && b || !c
来源：http://hz.guowangkeji.top/gtsgqyowta.html

TS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtnretaard.html

Java: a && b || !c
来源：http://hz.c1oappe.top/gtwtnnaotx.html

Go:   a && b || !c
来源：http://hz.dashuyun.cn/gtizqayrah.html

Ruby: a && b || !c
来源：http://hz.hywenlv.cn/gtjbulubcm.html

C#:   a && b || !c
来源：http://hz.tanke756.top/gtcpkrsrss.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sysykeji.top/gtfviysqmw.html

Py:   if not data: return
来源：http://hz.shangyingyoupin.top/gtyztddpkl.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgfzy.top/gtazzovsma.html

JS:   if (!data) return;
来源：http://hz.ybcxt.top/gtgnseyjfl.html

TS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtxptepsym.html

Java: if (data == null) return;
来源：http://hz.sweek.top/gtyvsejqyh.html

Go:   if data == nil { return }
来源：http://hz.yuanzhike.top/gthcbmpiwq.html

Ruby: return if data.nil?
来源：http://hz.hywenlv.cn/gtptckkehr.html

C#:   if (data == null) return;
来源：http://hz.jinqigfzy.top/gthgqzdgif.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrknvfgki.html

C. 函数与作用域
来源：http://hz.zhoulong.xyz/gtjjtgbnay.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtakzjbfic.html

[C01] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtouhtceup.html

Py:   def add(a, b): return a + b
来源：http://hz.aizwys.cn/gtbydvknyk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtbpmztwky.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtryyghhbx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtoefbvtjo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtiwfbvifg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yueranfly.top/gtrgquiofn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhoulong.xyz/gtxajjawer.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtutdqurld.html

[C02] 默认参数
来源：http://hz.jinyuanbaomall.cn/gtbebzwzxe.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtaymsjayi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.haohaochexian.top/gtixvnxmsu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hnxiangtu.top/gthbsfeglz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtbpmubkwe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigfzy.top/gtaaesvmeo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shangyingyoupin.top/gtdzntxkns.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtadxjtzzo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gtbdbfruzg.html

[C03] 可变参数
来源：http://hz.chenjidiqi.icu/gtmrzvqund.html

Py:   def total(*args): return sum(args)
来源：http://hz.xylfe.cn/gtojgaubtf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hammf.cn/gtdgdsrqkz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gteanxrvfd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtlhjrqnbx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.pycfn.com/gtembptsgq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.mhx1999.top/gtmrnqhyyf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gotoacloud.top/gteaydgfnx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtupdnjpmk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtjbllcjnl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgfzy.top/gtrrltgdcf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tian-w.cn/gtmkvzyikp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtciuqoxli.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hnqzz.top/gtoyzstnsm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guowangkeji.top/gtehwsnqym.html


<!-- 参考信息 -->