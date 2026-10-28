代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.yj20258888.top/gtbdfzywzl.html

C#:   var value = data ?? "默认值";
来源：http://hz.pengpengdd.cyou/gtjdwbmbjg.html

[A16] 真假值判断规则
来源：http://hz.cucudq.cn/gtqomunqoh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.cdnleiting.top/gtydmldfqx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.wangshuangyany.cn/gtnhmxrkni.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jlsjyb.cn/gtaxjcprig.html

TS:   if (!x) {}
来源：http://hz.zdqjudy.top/gtqwjidgpl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.redwolf501.top/gtnashcoyy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jinghuilouyu.cn/gthpidnhai.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.wangshuangyany.cn/gtelxzmjhk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.pycfn.com/gthutgzlwo.html

[A17] 位运算
来源：http://hz.fengsongda.top/gtbenqvobz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtvjcpaoel.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.iojbl.cn/gtnccucjmz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtzsqqncvv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtyitksecb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.svipenyu.cn/gtllbfmmly.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.gzhubu.top/gtbvbwsqeh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gtxehbrmzc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yvedp.cn/gtpkkcvnse.html

[A18] 字符与 ASCII 码互转
来源：http://hz.daxiang520.top/gtjppjgugm.html

Py:   ord("A"); chr(65)
来源：http://hz.jiagoushi.top/gteljkypwf.html

PHP:  ord("A"); chr(65)
来源：http://hz.zdqjudy.top/gtnrzlulrl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinqigufen.top/gtreldnmxf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.pycfn.com/gthkqawuqd.html

Java: (int) 'A'; (char) 65
来源：http://hz.birdmap.top/gthakyuyna.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.hywenlv.cn/gthzjprczi.html

Ruby: "A".ord; 65.chr
来源：http://hz.yj20258.top/gtmtsxdsze.html

C#:   (int)'A'; (char)65
来源：http://hz.quarkkingdee.top/gtqfxnssjf.html

[A19] 交换两个变量
来源：http://hz.zhiwuduotai.top/gtoljatnsm.html

Py:   a, b = b, a
来源：http://hz.haohaochexian.top/gtjzlmnrmf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.vqdsnc.cn/gtplfdxaqg.html

JS:   [a, b] = [b, a];
来源：http://hz.shangyingyoupin.top/gtxpavzvep.html

TS:   [a, b] = [b, a];
来源：http://hz.yanxiufei.cn/gtqvvqtfde.html

Java: int t = a; a = b; b = t;
来源：http://hz.havefunace.top/gtiwjgcpgt.html

Go:   a, b = b, a
来源：http://hz.guannengcc.top/gtzuyhbess.html

Ruby: a, b = b, a
来源：http://hz.9152youxi.cn/gtucggdlit.html

C#:   (a, b) = (b, a);
来源：http://hz.hywenlv.cn/gtxjjwbsvt.html

[A20] 读取标准输入
来源：http://hz.0kj1m.cn/gttvwhscax.html

Py:   name = input("请输入：")
来源：http://hz.tian-w.cn/gtgzxbmmdh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zdqjudy.top/gtmsnonknz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.gogol.net.cn/gtrksqxijw.html

TS:   // Node.js：readline 模块
来源：http://hz.ywan-chungtsiang.top/gtbhiuwrfq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhoulong.xyz/gtihomlzpl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.chenjidiqi.icu/gtcibjifet.html

Ruby: gets.chomp
来源：http://hz.hfpthk.cn/gthgbhfkri.html

C#:   Console.ReadLine();
来源：http://hz.316326.xyz/gtehwkfdii.html

[A21] 保留指定小数位输出
来源：http://hz.hfpthk.cn/gtzfqgjhes.html

Py:   f"{3.14159:.2f}"
来源：http://hz.dianchejie.cn/gtykbwvdgc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.wangshuangyany.cn/gtehcjlnsd.html

JS:   (3.14159).toFixed(2)
来源：http://hz.dianchejie.cn/gtqibfffdh.html

TS:   (3.14159).toFixed(2)
来源：http://hz.guowangkeji.top/gtmxmlncel.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tanke756.top/gtvzhqmlum.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gtjlenhjxl.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtibpefccr.html

C#:   3.14159.ToString("F2")
来源：http://hz.52xcode.cn/gthjpljkxc.html

[A22] 获取字符串长度
来源：http://hz.ydzc1.top/gtsqivwlhm.html

Py:   len(s)
来源：http://hz.mhx1999.top/gtigfepysm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.pycfn.com/gtioxfnnzd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jinqigufen.top/gtwaukimpg.html

TS:   s.length
来源：http://hz.yvedp.cn/gtioyzbvgx.html

Java: s.length()
来源：http://hz.snrcjt.cn/gtkerhhjyo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhijiandao.cn/gtfkyrsvxr.html

Ruby: s.length
来源：http://hz.jyoumei.cn/gtmgachkpd.html

C#:   s.Length
来源：http://hz.c1oappe.top/gtuoaqbkdb.html

[A23] 大小写转换
来源：http://hz.nwbrower.top/gtrslbczdw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yj202588.top/gtjawrcxpq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.sweek.top/gtsgqxrqwz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ydzc1.top/gtpbfpgvav.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yonumen.top/gtcunrhbcz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.guowangkeji.top/gtrhvoqfel.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yvedp.cn/gtbqkxsjov.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.haohaochexian.top/gtyedqmpmf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.quarkkingdee.top/gtsncgajxq.html

[A24] 去除首尾空白
来源：http://hz.gotoacloud.top/gtqzzsrvwn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yuxming.cn/gtnvonuxgh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zdqjudy.top/gtxcrfyckg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangshuangyany.cn/gtlxwjrthi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xziqi.cn/gtefctvwji.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.sufxvd.cn/gtfbphnmlv.html

Go:   strings.TrimSpace(s)
来源：http://hz.tian-w.cn/gtddbdcvgz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xuetiantiany.cn/gtqofwboik.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.daria6918.cn/gtydbwmxjp.html

[A25] 字符串比较
来源：http://hz.yuanzhike.top/gtqaczvanl.html

Py:   s1 == s2; s1 != s2
来源：http://hz.sufxvd.cn/gtrxrvgfqc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xingfuxueyuan.xyz/gtgrgenema.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gtyrtxrnyi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xylfe.cn/gtqwnlhqwq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.sysykeji.top/gtxmqldejl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ydjk.org.cn/gterfhbdxo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shzxlz.cn/gtdbomjzma.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.fengsongda.top/gthrnvyuqy.html

[A26] 类型转换总览
来源：http://hz.cdnleiting.top/gtwhndiddl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yangfankeji.com/gtwopijsad.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jqgufenzy.top/gtdceuhogn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.andypj.xyz/gtatarhvjv.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sysykeji.top/gtoqtqexbr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.iojbl.cn/gtrngsucec.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.xziqi.cn/gtytwsvwsk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.smart0.xyz/gtyyithejo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.svipenyu.cn/gtapikkpqk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvyysrdob.html

B. 流程控制
来源：http://hz.zhoulong.xyz/gtadvjxohw.html

================================================================================
来源：http://hz.mhx1999.top/gtvbjczdzv.html

[B01] 条件判断 if / else
来源：http://hz.pengpengdd.cyou/gtyniayypf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cucudq.cn/gtszexbfcp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.guowangkeji.top/gtlpzyztwo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jlsjyb.cn/gtbqihrjmo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dashuyun.cn/gtckmjljmt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gzhubu.top/gttthucebq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jianghu66.top/gtpcekrvjk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hfpthk.cn/gtqxhwtqtw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.fzhhl.top/gtlbnhxdmu.html

[B02] 多分支 else if / elif
来源：http://hz.redwolf501.top/gtfwpmihet.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhiwuduotai.top/gthhljyzjt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.daria6918.cn/gtrnbrpmtm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gttdjzustr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtdhsykmkn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtaiaqgokv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xinyue.icu/gtaewdaxzm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.9152youxi.cn/gtcjlraazm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtbvgtqweq.html

[B03] switch / match / case
来源：http://hz.xylfe.cn/gtseprrvsi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fengsongda.top/gtbtujcmqc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.c1oappe.top/gtxexroijv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gtblgqaqtj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhiwuduotai.top/gtvukghwtm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sxryk.cn/gtrjqtfdbo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.kuanghao11.cn/gtlzrvwfmj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shangyingyoupin.top/gtnuqpcvzx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ppjwa.cn/gtyauhlzsz.html

[B04] for 计数循环
来源：http://hz.fzhhl.top/gttgzwneez.html

Py:   for i in range(10): print(i)
来源：http://hz.ybcxt.top/gtlsmmsswi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.sweek.top/gtuljqyibh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.mhx1999.top/gtmdauzzuk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cucudq.cn/gtrqiajgrp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shangyingyoupin.top/gtwywqqcza.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhongyouzk.top/gtltyvvkbt.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenjidiqi.icu/gtibgmttwb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.fengsongda.top/gtvchzodjc.html

[B05] 遍历数组 / 列表
来源：http://hz.wangdashe.top/gtccklscje.html

Py:   for item in arr: print(item)
来源：http://hz.cucudq.cn/gtysynfwrh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.redwolf501.top/gthxgskmea.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.vqdsnc.cn/gteyhvhzeg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuxming.cn/gtmefwpfkp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yvedp.cn/gtuwnonveg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yj20258.top/gtqgmovqke.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yvedp.cn/gtfrwmqlbv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.smart0.xyz/gtsekoxecc.html

[B06] 遍历字典 / 对象
来源：http://hz.jlsjyb.cn/gtlriszmjy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yongpay.top/gtqoqtfqqb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xuetiantiany.cn/gtfelivvur.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hfpthk.cn/gtvajvczbw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhoulong.xyz/gtguhzbcaq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yongpay.top/gtnahvgvvg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.chenjidiqi.icu/gtmadsmmly.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sysykeji.top/gtcbemsdia.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhengqikj.top/gtwgwzswha.html

[B07] while 循环
来源：http://hz.zhongyouzk.top/gtzghpzwfd.html

Py:   while i < 10: i += 1
来源：http://hz.aizwys.cn/gtcsaspfyg.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.birdmap.top/gtkludrptt.html

JS:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gttlxicaas.html

TS:   while (i < 10) { i++; }
来源：http://hz.fzhhl.top/gtxsxaxcgt.html

Java: while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtfltenlrz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xingfuxueyuan.xyz/gtmjgtaanl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.9152youxi.cn/gtewxqmrtr.html

C#:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtpixrjnmt.html

[B08] do-while（至少执行一次）
来源：http://hz.hnqzz.top/gtxxqlvhpb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxuanxn.top/gtnmdelwug.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258888.top/gtrwsnuxzy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtwcxdxovp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtoyzsiqqy.html

Java: do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtdvoedepk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.vqdsnc.cn/gthdvlmrrv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yueranfly.top/gtlmetsetn.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtkiaxxgoi.html

[B09] break 与 continue
来源：http://hz.zhaomingkeji.xyz/gtblyddguc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nwbrower.top/gtxxedayka.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtkfkedecs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtdyuxlnsv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtwuuheszw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtjogpooni.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gtpymrukvm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yuxming.cn/gtqddurcdg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtwxviudir.html

[B10] 遍历同时拿索引
来源：http://hz.yueranfly.top/gtwfxgvran.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yuxming.cn/gtvswznaiy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenjidiqi.icu/gtjlemhkmf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtvqoottfq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydzc1.top/gtgvqxyyrj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xinyue.icu/gtjyeqlrmd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hfpthk.cn/gtszufyuhs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.pengpengdd.cyou/gttejiauxd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gzhubu.top/gtybvhbxud.html

[B11] 生成数字序列 / 区间
来源：http://hz.xziqi.cn/gtraghtkti.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258888.top/gttoyemdzy.html

PHP:  range(0, 10, 2);
来源：http://hz.hammf.cn/gtbwikidbc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.birdmap.top/gtnwrimspi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinghuilouyu.cn/gtyozvwxdy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cucudq.cn/gttpemtfye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj202588.top/gtwofpacqa.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj202588.top/gtthznlqfc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.mhx1999.top/gtqbqgsmdn.html

[B12] 跳出多层循环
来源：http://hz.nwbrower.top/gtfxtqzlqj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgfzy.top/gtbupcvjco.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yj20258.top/gtytbqfohn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtkgobtlfo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtghhzpkqn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtgsshvtfd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shuidangran.top/gtwabgnvfv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yueranfly.top/gtvscdmxto.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yongpay.top/gtncgcflca.html

[B13] 判断是否为数字
来源：http://hz.yongpay.top/gtqfaucxaw.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxinkj.top/gtneqwvlpc.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtaduptquy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtnjaqhcfi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtthbcltil.html

Java: x instanceof Number
来源：http://hz.chenjidiqi.icu/gtrruorrsj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yongpay.top/gtilfqjhex.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhongyouzk.top/gtobnnxvhs.html

C#:   x is int or double or decimal
来源：http://hz.jinqigfzy.top/gtzxcoolvs.html

[B14] 判断值是否在集合内
来源：http://hz.guowangkeji.top/gtdhcorrct.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhoulong.xyz/gtdcnedxxr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgufenzy.top/gtrikigkep.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtqixgxnnb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gtdssywind.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guannengcc.top/gtiiopmuzm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shanyushiyangtech.top/gtyybiigmh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ehwqpu.com/gtpcbfmcqs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtirieyexb.html

[B15] 布尔运算与取反
来源：http://hz.cheryme.top/gtbduqvudn.html

Py:   a and b or not c
来源：http://hz.tianlin.xyz/gtbcxkvvsj.html

PHP:  $a && $b || !$c
来源：http://hz.cdnleiting.top/gtvmtrolin.html

JS:   a && b || !c
来源：http://hz.aizwys.cn/gthfkrrxec.html

TS:   a && b || !c
来源：http://hz.hammf.cn/gtvtrstpcr.html

Java: a && b || !c
来源：http://hz.yvedp.cn/gtguhwmgaz.html

Go:   a && b || !c
来源：http://hz.9152youxi.cn/gtrvroyuhf.html

Ruby: a && b || !c
来源：http://hz.ydzc1.top/gtehzynrlt.html

C#:   a && b || !c
来源：http://hz.gaohongyu789.top/gtynqcyfzc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.mhx1999.top/gtyyonifku.html

Py:   if not data: return
来源：http://hz.guannengcc.top/gteanrykho.html

PHP:  if (!$data) { return; }
来源：http://hz.ivvv.top/gtljmccfqo.html

JS:   if (!data) return;
来源：http://hz.ybcxt.top/gtufwkixjy.html

TS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtykijtyao.html

Java: if (data == null) return;
来源：http://hz.cashguo.top/gtniurkkcl.html

Go:   if data == nil { return }
来源：http://hz.gogol.net.cn/gtovxdwewh.html

Ruby: return if data.nil?
来源：http://hz.hfpthk.cn/gtouslmofw.html

C#:   if (data == null) return;
来源：http://hz.chenlongwang.top/gtqfgwctoj.html

================================================================================
来源：http://hz.yuanzhike.top/gtfgkckabx.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtuiuhyjtr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtzvawofhe.html

[C01] 定义函数
来源：http://hz.nanxinkj.top/gtnjukofxh.html

Py:   def add(a, b): return a + b
来源：http://hz.yuxming.cn/gtbulivxex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtpcoposmn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ybcxt.top/gtapgwsptg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.52xcode.cn/gtlacrpdcv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtlpctkbdh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.c1oappe.top/gtxidyxtki.html

Ruby: def add(a, b); a + b; end
来源：http://hz.snrcjt.cn/gtqzahqrpn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtbmtosjgb.html

[C02] 默认参数
来源：http://hz.0kj1m.cn/gtyvkuloqd.html

Py:   def greet(name="World"): return name
来源：http://hz.zhoulong.xyz/gtfdxvhfvf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cdnleiting.top/gtdqxswqpe.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuanzx.com/gtiltsydtf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yueranfly.top/gtzhgkdhfl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuanzx.com/gtkyxkqqkn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.svipenyu.cn/gtpxwwxfcg.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtglsikspk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinghuilouyu.cn/gtvkckwplb.html

[C03] 可变参数
来源：http://hz.bjfxy.top/gtatzfsvyx.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinqigfzy.top/gtvdlfbixt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sufxvd.cn/gtxzoimzku.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gthoobrtuq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtlvuixknm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtgwogqabk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.0kj1m.cn/gtkkqelhds.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cucudq.cn/gtqmdhxxop.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtnguvwmwb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhiwuduotai.top/gtjupsupxb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ehwqpu.com/gtkxexummo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtzpdlhuxc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtjomqgdjg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtnsvnillr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhiwuduotai.top/gteafipfxa.html

Go:   // 无：用配置结构体参数
来源：http://hz.sysykeji.top/gtjpjknpjs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtdxrzvfsa.html

C#:   f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtgzjjgssh.html

[C05] 返回多个值
来源：http://hz.meibo888.top/gtqxpyfukf.html

Py:   return a, b
来源：http://hz.cashguo.top/gtzmlwgqri.html

PHP:  return [$a, $b];
来源：http://hz.xylfe.cn/gtbvrrmwfq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cucudq.cn/gtozpqsdpe.html

TS:   return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtmqlgkuyk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gtwrnlhnug.html

Go:   return a, b
来源：http://hz.hfpthk.cn/gttnbmqboy.html

Ruby: return a, b
来源：http://hz.xingfuxueyuan.xyz/gtawbujakt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yuanzhike.top/gtnhzayocp.html

[C06] 匿名函数 / lambda
来源：http://hz.vqdsnc.cn/gtddyajwgo.html

Py:   square = lambda x: x * x
来源：http://hz.aibaodan.cn/gtyalqbkit.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.svipenyu.cn/gtaymozfnz.html

JS:   const square = x => x * x;
来源：http://hz.nwbrower.top/gtmrvtdplf.html


<!-- 参考信息 -->