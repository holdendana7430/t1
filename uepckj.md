代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://hz.jqgfzy.top/gtgzkdlaqw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.snrcjt.cn/gtfjibllcx.html

Go:   // 单行；/* 多行 */
来源：http://hz.yonumen.top/gtnkxpjmhe.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.kuanghao11.cn/gtkjsoiqzw.html

C#:   // 单行；/* 多行 */
来源：http://hz.meibo888.top/gtacfrnpzf.html

[A15] 空值判断与默认值
来源：http://hz.vqdsnc.cn/gtbxcbodiu.html

Py:   value = data or "默认值"
来源：http://hz.xylfe.cn/gtkdmhogxi.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.birdmap.top/gtjuswxzcs.html

JS:   const value = data ?? "默认值";
来源：http://hz.tianlin.xyz/gthcsetpux.html

TS:   const value = data ?? "默认值";
来源：http://hz.xylfe.cn/gtgqfquazl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hammf.cn/gtuygxevaz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.shanyushiyangkeji.top/gttnrlpqxa.html

Ruby: value = data || "默认值"
来源：http://hz.sweek.top/gtbhqeyxmc.html

C#:   var value = data ?? "默认值";
来源：http://hz.bjfxy.top/gtyasiidbq.html

[A16] 真假值判断规则
来源：http://hz.jinyuanbaomall.cn/gtakqkjfuv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.feifeiyinyue.top/gtajsyoadq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.shangyingyoupin.top/gtdhyvezxg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.daxiang520.top/gtymobhnlz.html

TS:   if (!x) {}
来源：http://hz.tianlin.xyz/gtenartoix.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.chenjidiqi.icu/gtztynxbxl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.gzhubu.top/gttxhrxdxh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.shanyushiyangkeji.top/gtouabefhn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.wangshuangyany.cn/gtqzdszhhr.html

[A17] 位运算
来源：http://hz.jianghu66.top/gtausfqbqh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtyfaezbnw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhijiandao.cn/gtzdzfjxyf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtvmzccbak.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtdtwoagtz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ybcxt.top/gtheuadvec.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hnxiangtu.top/gtuozfgdrt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigufen.top/gtxgmismwr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhongyouzk.top/gtnimnwcoi.html

[A18] 字符与 ASCII 码互转
来源：http://hz.wangshuangyany.cn/gteesiclgl.html

Py:   ord("A"); chr(65)
来源：http://hz.sysykeji.top/gthufqnrna.html

PHP:  ord("A"); chr(65)
来源：http://hz.birdmap.top/gtoudqslqv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daria6918.cn/gtbeuwgqrl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxuanxn.top/gtntgqoifx.html

Java: (int) 'A'; (char) 65
来源：http://hz.shuidangran.top/gtyngetihj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zhaomingkeji.xyz/gtorhsqzml.html

Ruby: "A".ord; 65.chr
来源：http://hz.nanxinkj.top/gtdijpsbfv.html

C#:   (int)'A'; (char)65
来源：http://hz.yvedp.cn/gticbukdpm.html

[A19] 交换两个变量
来源：http://hz.shzxlz.cn/gtmzbvprri.html

Py:   a, b = b, a
来源：http://hz.hnxiangtu.top/gtsimfulrc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.nanxuanxn.top/gtkbjdcqeu.html

JS:   [a, b] = [b, a];
来源：http://hz.cdnleiting.top/gtlsnzynoe.html

TS:   [a, b] = [b, a];
来源：http://hz.meibo888.top/gtdibpbokl.html

Java: int t = a; a = b; b = t;
来源：http://hz.cqqwz.cn/gtqzssbgwr.html

Go:   a, b = b, a
来源：http://hz.feifeiyinyue.top/gtpqwifndu.html

Ruby: a, b = b, a
来源：http://hz.yonumen.top/gtcenysala.html

C#:   (a, b) = (b, a);
来源：http://hz.sysykeji.top/gtavjhrlkn.html

[A20] 读取标准输入
来源：http://hz.chenlongwang.top/gtilahfoym.html

Py:   name = input("请输入：")
来源：http://hz.ppjwa.cn/gtyqbnmvfc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ivvv.top/gtfjfqhbwa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.kuanghao11.cn/gtyhvafoyt.html

TS:   // Node.js：readline 模块
来源：http://hz.yj20258888.top/gtminmmjsq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.cucudq.cn/gtsdxatxvw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.fengsongda.top/gtoxdzdczd.html

Ruby: gets.chomp
来源：http://hz.wangshuangyany.cn/gtqqfszvmb.html

C#:   Console.ReadLine();
来源：http://hz.zycfv.cn/gtrsrkynhx.html

[A21] 保留指定小数位输出
来源：http://hz.yanxiufei.cn/gtqzmzffws.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cashguo.top/gtkjxsnbzi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtalxvtpgk.html

JS:   (3.14159).toFixed(2)
来源：http://hz.fengsongda.top/gthycbmrqc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jinqigfzy.top/gtqgfcdfek.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shuidangran.top/gtprjamzbp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtculerncq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jinqigufen.top/gttnoczrpf.html

C#:   3.14159.ToString("F2")
来源：http://hz.sxryk.cn/gtetnpauir.html

[A22] 获取字符串长度
来源：http://hz.hysaishi.cn/gtdsbnzcnx.html

Py:   len(s)
来源：http://hz.yj20258888.top/gtrifcgmjq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jianghu66.top/gtycjdgfjl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jiagoushi.top/gtauxzaqrs.html

TS:   s.length
来源：http://hz.zhixingplan.top/gtpnvyynps.html

Java: s.length()
来源：http://hz.jqgufenzy.top/gtiozqtptb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.gzhubu.top/gtqcbjnvsp.html

Ruby: s.length
来源：http://hz.hnqzz.top/gtlzwrxbha.html

C#:   s.Length
来源：http://hz.xingfuxueyuan.xyz/gtcbkfzxmh.html

[A23] 大小写转换
来源：http://hz.ydjk.org.cn/gtlwjxrbfb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gzhubu.top/gtqmyagsng.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.tanke756.top/gtydemibhq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sysykeji.top/gtfypwrykt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnqzz.top/gtfkizzjkz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.redwolf501.top/gttdqtxglb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cheryme.top/gtwnlhduzb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.dianchejie.cn/gtcdmxwdie.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yj20258.top/gtzdbltrey.html

[A24] 去除首尾空白
来源：http://hz.shanyushiyangtech.top/gtumgbwhqm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.tanke756.top/gtywojropc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.nanxuanxn.top/gtatmslzkg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cheryme.top/gtneitgnty.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhixingplan.top/gtcykuzswd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yanxiufei.cn/gtbmknacwt.html

Go:   strings.TrimSpace(s)
来源：http://hz.ydzc1.top/gtfehpyhcw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cdnleiting.top/gtxggqshvp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jinqigufen.top/gtcsypjlsh.html

[A25] 字符串比较
来源：http://hz.yonumen.top/gtggqcgewf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.wangshuangyany.cn/gtalrlnios.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.hnxiangtu.top/gtvzehwmlq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yanxiufei.cn/gtuxuytmyz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tian-w.cn/gtjzkksijp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jianghu66.top/gtnvrqtvki.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jqgfzy.top/gtcifeixqp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gzhubu.top/gttfmbptil.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shanyushiyangkeji.top/gtfyahatcu.html

[A26] 类型转换总览
来源：http://hz.kuanghao11.cn/gtallxetwz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinghuilouyu.cn/gtitwgegkq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yuanzhike.top/gtuvupfzzn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.wangshuangyany.cn/gthlzlkhxo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cqqwz.cn/gtfzljebxd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.dianchejie.cn/gtbssdcvfe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenlongwang.top/gtpuckhdza.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.fengsongda.top/gtzpfsmsil.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.guannengcc.top/gtgoyaretr.html

================================================================================
来源：http://hz.zhengqikj.top/gtbvzxemag.html

B. 流程控制
来源：http://hz.zhaomingkeji.xyz/gtllpkpjrj.html

================================================================================
来源：http://hz.tianlin.xyz/gtusheuxnw.html

[B01] 条件判断 if / else
来源：http://hz.xuanzx.com/gtskphhylh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gzhubu.top/gtbecxfaiw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.aibaodan.cn/gtkkknlibp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sysykeji.top/gtxvnlgeqg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cashguo.top/gtqzjkictl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.nanxinkj.top/gtxqoaqywf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jlsjyb.cn/gtynwhjazt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.ywan-chungtsiang.top/gtdtvwqpdi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gttpxzmvhh.html

[B02] 多分支 else if / elif
来源：http://hz.yongpay.top/gtotpvjsgs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shangyingyoupin.top/gtrlxvfayq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.bjfxy.top/gtuyqbuves.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gtgfdkzvdw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtfgqhakvy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtwyaylmbj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.feifeiyinyue.top/gtzqgeuztb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhengqikj.top/gthijbixpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ybcxt.top/gtyawzxjxa.html

[B03] switch / match / case
来源：http://hz.xuanzx.com/gtoqarpkry.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.nanxinkj.top/gtgjtbkijf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.316326.xyz/gtfuwfctup.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtlevmnrev.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigufen.top/gtgkkipjim.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ppjwa.cn/gtzsyhpflj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.guowangkeji.top/gteshmqcwf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yj202588.top/gtmntfvktq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gaohongyu789.top/gtkwoampwy.html

[B04] for 计数循环
来源：http://hz.zhiwuduotai.top/gtxqxfuuzo.html

Py:   for i in range(10): print(i)
来源：http://hz.nanxuanxn.top/gthgikmmog.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shanyushiyangtech.top/gtcmgwvctq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gogol.net.cn/gtncwczepm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.snrcjt.cn/gtzgkktbmf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yongpay.top/gtaqjlcgiy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.haohaochexian.top/gtrrqeaqjq.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenjidiqi.icu/gttrmymxzn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ppjwa.cn/gtefjunhit.html

[B05] 遍历数组 / 列表
来源：http://hz.dashuyun.cn/gtnqegcouk.html

Py:   for item in arr: print(item)
来源：http://hz.svipenyu.cn/gtvmgaqycu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.daria6918.cn/gtabtuguuq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yangfankeji.com/gtfzqduetu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ppjwa.cn/gtqwxwwfex.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yvedp.cn/gtqphuivfh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ehwqpu.com/gtynojslvq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xuetiantiany.cn/gtvrjxigne.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yanxiufei.cn/gtfxzvfxjg.html

[B06] 遍历字典 / 对象
来源：http://hz.tanke756.top/gttjkvxmus.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hammf.cn/gtqtiulnff.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daria6918.cn/gtldpgoouu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zdqjudy.top/gtowwbbsvm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gogol.net.cn/gtdvhzqclb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xziqi.cn/gtehrxvvto.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hammf.cn/gtybpmcyzi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ppjwa.cn/gtfhhwwsmt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.0kj1m.cn/gtlofptxvg.html

[B07] while 循环
来源：http://hz.xuetiantiany.cn/gtarloywqo.html

Py:   while i < 10: i += 1
来源：http://hz.xuanzx.com/gtagijxqhv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ydjk.org.cn/gtxsixwroy.html

JS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtcjsfynzh.html

TS:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtprnqvvqf.html

Java: while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gthpudwieu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.fengsongda.top/gtxkmrnpos.html

Ruby: while i < 10; i += 1; end
来源：http://hz.gzhubu.top/gtjaickcof.html

C#:   while (i < 10) { i++; }
来源：http://hz.feifeiyinyue.top/gtujzesyyg.html

[B08] do-while（至少执行一次）
来源：http://hz.zhaomingkeji.xyz/gtordcnnyi.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sufxvd.cn/gtnsvjitir.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.nwbrower.top/gtiftuxvll.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jianghu66.top/gtgntudgry.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtjoffdtpp.html

Java: do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gtxhcrrvvo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.chenlongwang.top/gtiwbnnron.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yuxming.cn/gtnoirxsvh.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtitbctfvj.html

[B09] break 与 continue
来源：http://hz.hammf.cn/gtzmhtible.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yvedp.cn/gtfwejcaeo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.c1oappe.top/gtxaqjdivz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtzywrmuxd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtkrfupncf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtiknqlpgu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zycfv.cn/gtxeyonhne.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.birdmap.top/gtirnbwahi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtivgfyahl.html

[B10] 遍历同时拿索引
来源：http://hz.xingfuxueyuan.xyz/gtrdbjjbtv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yongpay.top/gtbhczdngs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cucudq.cn/gtgpkocabr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.pycfn.com/gtssmlrxoo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhengqikj.top/gtrojqfhqg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guowangkeji.top/gtstqbchtn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cheryme.top/gtmthdohse.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yueranfly.top/gtvhsuriqv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gotoacloud.top/gtagnylemi.html

[B11] 生成数字序列 / 区间
来源：http://hz.9152youxi.cn/gtddszcxgj.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtwybjsepg.html

PHP:  range(0, 10, 2);
来源：http://hz.316326.xyz/gtncyyfgdz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tianlin.xyz/gtsfqeeefp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gttisrhyjx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnqzz.top/gtdlfqelqp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtxbplkrzo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.meibo888.top/gtbnsyvyqx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tanke756.top/gtkmojlnxk.html

[B12] 跳出多层循环
来源：http://hz.zhaomingkeji.xyz/gtbtbhwooc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.kuanghao11.cn/gtnpejxwsj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhixingplan.top/gtrvwncafb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtzmjwrvls.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtildmizrj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtixezmrtk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yueranfly.top/gtmrprqjou.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnqzz.top/gtmbgafmrx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj202588.top/gtzlypflsb.html

[B13] 判断是否为数字
来源：http://hz.yueranfly.top/gtwyaopaij.html

Py:   isinstance(x, (int, float))
来源：http://hz.xziqi.cn/gtdqywozfv.html

PHP:  is_numeric($x)
来源：http://hz.shangyingyoupin.top/gtopikdaxc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtmoxjpjgq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jlsjyb.cn/gtpfuvuazi.html

Java: x instanceof Number
来源：http://hz.jiagoushi.top/gthmjjpkgp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.fengsongda.top/gtgfxhxgpg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangtech.top/gtncrqjzab.html

C#:   x is int or double or decimal
来源：http://hz.jiagoushi.top/gtymkuhdto.html

[B14] 判断值是否在集合内
来源：http://hz.316326.xyz/gtfvaewmox.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dashuyun.cn/gtxwatnako.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ppjwa.cn/gtnxvzkzem.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gttalppyfr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtnditaimh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tian-w.cn/gtdtvbtoho.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.aibaodan.cn/gttcklfaym.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgfzy.top/gtzaoldmxw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuxming.cn/gthdqibylm.html

[B15] 布尔运算与取反
来源：http://hz.fengsongda.top/gtsvdxnysr.html

Py:   a and b or not c
来源：http://hz.hammf.cn/gtkywrlkyn.html

PHP:  $a && $b || !$c
来源：http://hz.aizwys.cn/gtqsdkonfo.html

JS:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtisvvpnpg.html

TS:   a && b || !c
来源：http://hz.ybcxt.top/gtqarpxify.html

Java: a && b || !c
来源：http://hz.yongpay.top/gtriwxoabn.html

Go:   a && b || !c
来源：http://hz.wangdashe.top/gtexsyomuo.html

Ruby: a && b || !c
来源：http://hz.pengpengdd.cyou/gtnfwtjkom.html

C#:   a && b || !c
来源：http://hz.meibo888.top/gtqlvmmrbf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hywenlv.cn/gtgdhbnuuw.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtguuafzaw.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gttmivctet.html

JS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtgmtheeef.html

TS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtfximwbvb.html

Java: if (data == null) return;
来源：http://hz.sweek.top/gthwwkkkbf.html

Go:   if data == nil { return }
来源：http://hz.gotoacloud.top/gtvvrdomoe.html

Ruby: return if data.nil?
来源：http://hz.yvedp.cn/gtzdrbqadv.html

C#:   if (data == null) return;
来源：http://hz.hywenlv.cn/gtlbxqecrm.html

================================================================================
来源：http://hz.xinyue.icu/gtshfkqqur.html

C. 函数与作用域
来源：http://hz.zhaomingkeji.xyz/gtdtvvzpex.html

================================================================================
来源：http://hz.cheryme.top/gtdpftditw.html

[C01] 定义函数
来源：http://hz.chenzaomai.com/gtgblhyewe.html

Py:   def add(a, b): return a + b
来源：http://hz.dashuyun.cn/gtllykhnod.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtjdzkbngi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhixingplan.top/gtejcpdayo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sysykeji.top/gtkquqfbeb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtbzpvlovc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhijiandao.cn/gthjmdtohn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhongyouzk.top/gtldlnekuo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gttwfwduqq.html

[C02] 默认参数
来源：http://hz.jqgufenzy.top/gtapdhgrtn.html

Py:   def greet(name="World"): return name
来源：http://hz.redwolf501.top/gtbygdelvd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhijiandao.cn/gtgwyjrwfq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtxdihyoim.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtrmmfpmgk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.52xcode.cn/gtuyznetue.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cucudq.cn/gttkrdkokb.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtwaqfbopr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cucudq.cn/gtfthxsout.html

[C03] 可变参数
来源：http://hz.gaohongyu789.top/gtcqgqkhqy.html

Py:   def total(*args): return sum(args)
来源：http://hz.hywenlv.cn/gtzxoqslxc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnxiangtu.top/gtckjndook.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shangyingyoupin.top/gthyakmqlf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydzc1.top/gtirzwysgq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.meibo888.top/gtosgjhiak.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jiagoushi.top/gtthyrgdyj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aibaodan.cn/gtzgukolvk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtehjzqrtr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.bjfxy.top/gtlvzmhayp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhixingplan.top/gtjxcgigaz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigufen.top/gthkbczgyx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gtqvrbgzom.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jyoumei.cn/gthqiucjor.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.fengsongda.top/gtsaeqtxwu.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhongyouzk.top/gtnhtrulwp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtxikcimpj.html

C#:   f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtbhrvjrgh.html

[C05] 返回多个值
来源：http://hz.xuetiantiany.cn/gtfmdyzxcn.html


<!-- 参考信息 -->