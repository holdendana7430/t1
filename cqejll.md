代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.ehwqpu.com/gtibmalkry.html

TS:   const value = data ?? "默认值";
来源：http://hz.fengsongda.top/gtevibmyao.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.52xcode.cn/gtrfuilrlf.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.9152youxi.cn/gtvquhtdqe.html

Ruby: value = data || "默认值"
来源：http://hz.zycfv.cn/gtbvlvwugn.html

C#:   var value = data ?? "默认值";
来源：http://hz.316326.xyz/gthwpphojw.html

[A16] 真假值判断规则
来源：http://hz.zhoulong.xyz/gtinhcufcf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.aibaodan.cn/gtifwzltxt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.tian-w.cn/gtgcamybvr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.haohaochexian.top/gthlcnitlq.html

TS:   if (!x) {}
来源：http://hz.ydzc1.top/gtptkzfvjr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.haohaochexian.top/gthruslpvl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.daria6918.cn/gtrndgcilo.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.pengpengdd.cyou/gttcleugif.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.tanke756.top/gtssjavmso.html

[A17] 位运算
来源：http://hz.aizwys.cn/gtoirwljuy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtapzrvhbr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ppjwa.cn/gtxcirbdfc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gthiimywjp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gtfubpupfj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtcjncjhdn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtxewrljcm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gteamlbkyc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtnyooucfx.html

[A18] 字符与 ASCII 码互转
来源：http://hz.quarkkingdee.top/gtbfxjmbem.html

Py:   ord("A"); chr(65)
来源：http://hz.svipenyu.cn/gttysrysbh.html

PHP:  ord("A"); chr(65)
来源：http://hz.fengsongda.top/gtzhtbmogs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shuidangran.top/gtbabuxjzw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ivvv.top/gtbgatfroa.html

Java: (int) 'A'; (char) 65
来源：http://hz.yj20258888.top/gtozzkuikz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.andypj.xyz/gtboxsaedq.html

Ruby: "A".ord; 65.chr
来源：http://hz.aibaodan.cn/gtkhwmkpqj.html

C#:   (int)'A'; (char)65
来源：http://hz.ehwqpu.com/gtonyjnijk.html

[A19] 交换两个变量
来源：http://hz.sxryk.cn/gtkhqkwuwu.html

Py:   a, b = b, a
来源：http://hz.sufxvd.cn/gtmdcljzir.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hammf.cn/gtwnaxyivl.html

JS:   [a, b] = [b, a];
来源：http://hz.ydjk.org.cn/gtmsjmsbxv.html

TS:   [a, b] = [b, a];
来源：http://hz.andypj.xyz/gthkfbffgm.html

Java: int t = a; a = b; b = t;
来源：http://hz.nanxinkj.top/gtpsjqpify.html

Go:   a, b = b, a
来源：http://hz.ywan-chungtsiang.top/gtjztjyvzb.html

Ruby: a, b = b, a
来源：http://hz.zhixingplan.top/gtcgwapdxz.html

C#:   (a, b) = (b, a);
来源：http://hz.jqgfzy.top/gtmciaqfti.html

[A20] 读取标准输入
来源：http://hz.jinghuilouyu.cn/gtsqujyxjv.html

Py:   name = input("请输入：")
来源：http://hz.iojbl.cn/gtbyhkbpfj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.9152youxi.cn/gtmbehbwaj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jqgufenzy.top/gtydvaeovf.html

TS:   // Node.js：readline 模块
来源：http://hz.jinyuanbaomall.cn/gthxuyholx.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jyoumei.cn/gtkinyjypv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.cheryme.top/gtkaozryet.html

Ruby: gets.chomp
来源：http://hz.quarkkingdee.top/gtvsjwtbjb.html

C#:   Console.ReadLine();
来源：http://hz.xuanzx.com/gtjfkkgzza.html

[A21] 保留指定小数位输出
来源：http://hz.shanyushiyangkeji.top/gtacukkajy.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zhixingplan.top/gttworqjfr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jqgufenzy.top/gttgelmvfu.html

JS:   (3.14159).toFixed(2)
来源：http://hz.nwbrower.top/gthbukmaxy.html

TS:   (3.14159).toFixed(2)
来源：http://hz.quarkkingdee.top/gthnwyoybc.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.cqqwz.cn/gtxfdmwvkk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtlxnqiydk.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtkfoqsaog.html

C#:   3.14159.ToString("F2")
来源：http://hz.aibaodan.cn/gtckjlysty.html

[A22] 获取字符串长度
来源：http://hz.ehwqpu.com/gtdgjxfnqn.html

Py:   len(s)
来源：http://hz.zhengqikj.top/gtpfabldhp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yvedp.cn/gtchhrhvcn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xingfuxueyuan.xyz/gtrxxawlsv.html

TS:   s.length
来源：http://hz.cashguo.top/gtgfrogtyv.html

Java: s.length()
来源：http://hz.zhijiandao.cn/gtgpeuicgb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zdqjudy.top/gtsdiugjnb.html

Ruby: s.length
来源：http://hz.hammf.cn/gtybpakjwg.html

C#:   s.Length
来源：http://hz.ywan-chungtsiang.top/gtdtucqobj.html

[A23] 大小写转换
来源：http://hz.sweek.top/gtncyygixn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ivvv.top/gtwezvyhgi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ywan-chungtsiang.top/gtawbhfqxn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shuidangran.top/gtuxzbjzaz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gtcthxtgal.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.sweek.top/gtisgenwpa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.andypj.xyz/gtblwxhkfi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.pengpengdd.cyou/gtwowlszdv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.tian-w.cn/gtdckasiev.html

[A24] 去除首尾空白
来源：http://hz.ydzc1.top/gtxdkknknm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.wangshuangyany.cn/gtcqezybmy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.tian-w.cn/gtqaqatllo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.iojbl.cn/gtasjnerki.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hammf.cn/gttsdvylea.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.cheryme.top/gtmpgnarmc.html

Go:   strings.TrimSpace(s)
来源：http://hz.haohaochexian.top/gtzxnbwjhm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.c1oappe.top/gtiffpmnnx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yuanzhike.top/gtbrenpaij.html

[A25] 字符串比较
来源：http://hz.cashguo.top/gtliairjfb.html

Py:   s1 == s2; s1 != s2
来源：http://hz.gogol.net.cn/gtbdpewwud.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ybcxt.top/gtqennaduy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenjidiqi.icu/gtbcevuybn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.smart0.xyz/gtpvazmhcc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yvedp.cn/gtfrjlofyp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yueranfly.top/gtkmccbzpa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shangyingyoupin.top/gtwkfutwjp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hongshengwenyu.top/gtgvvbyzxi.html

[A26] 类型转换总览
来源：http://hz.xingfuxueyuan.xyz/gtytiqkioa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.aibaodan.cn/gtcqkteivc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhijiandao.cn/gtsdmbkbhr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sxryk.cn/gtdvyhnyxn.html

TS:   Number() String() Boolean() x as number
来源：http://hz.52xcode.cn/gtiflefwpt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ivvv.top/gtnjaxymod.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yj20258888.top/gttdobmyfh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.wangshuangyany.cn/gtiywhnxkf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yanxiufei.cn/gtmygjcizp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsthynktv.html

B. 流程控制
来源：http://hz.andypj.xyz/gtvgoeskso.html

================================================================================
来源：http://hz.jyoumei.cn/gtjkmjskhu.html

[B01] 条件判断 if / else
来源：http://hz.ehwqpu.com/gthswkgwxu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinqigufen.top/gtycmzkxlw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.kuanghao11.cn/gtasjuroqw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtaniotzed.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangkeji.top/gtywgkgapy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtkhbnqmwd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jiagoushi.top/gtdnkxodsb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.birdmap.top/gtlrzbzkbg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.dianchejie.cn/gtwqhywztl.html

[B02] 多分支 else if / elif
来源：http://hz.yj20258.top/gtdmtkkasv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhijiandao.cn/gtzomfjeti.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhixingplan.top/gtuzriudcp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.c1oappe.top/gtgamgvwhs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenjidiqi.icu/gtapdxgwlp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhaomingkeji.xyz/gtjgfndgzp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhongyouzk.top/gttkyngadr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hongshengwenyu.top/gtczpdgqfi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtiztvjtqq.html

[B03] switch / match / case
来源：http://hz.9152youxi.cn/gtuqtizagm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sufxvd.cn/gtapmkebfv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.kuanghao11.cn/gtettktvlq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.guowangkeji.top/gtdayraxpo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhoulong.xyz/gtfmnawkpt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ybcxt.top/gtyfijtgtj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.redwolf501.top/gtykbdvuwl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hammf.cn/gtfmqncgjt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhaomingkeji.xyz/gtesoroham.html

[B04] for 计数循环
来源：http://hz.iojbl.cn/gtrtnxhakx.html

Py:   for i in range(10): print(i)
来源：http://hz.yj20258.top/gtsdormwcz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yvedp.cn/gtkszlcffz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gogol.net.cn/gtmhzupzyv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tian-w.cn/gtrdvpjirf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sweek.top/gtpkazlytg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ivvv.top/gtrfxloqol.html

Ruby: 10.times { |i| puts i }
来源：http://hz.kuanghao11.cn/gtmkewcxei.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.birdmap.top/gtrgmkudyn.html

[B05] 遍历数组 / 列表
来源：http://hz.jianghu66.top/gtvyckhgwr.html

Py:   for item in arr: print(item)
来源：http://hz.jlsjyb.cn/gtsfztlufq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cashguo.top/gtgmlqtozz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.smart0.xyz/gtnkbnoiyp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shuidangran.top/gtuapirufw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.meibo888.top/gtpeophefb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.tanke756.top/gtfowovymf.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sysykeji.top/gtfstustza.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yvedp.cn/gtrkouhszn.html

[B06] 遍历字典 / 对象
来源：http://hz.yj20258.top/gtpqxrigba.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.tian-w.cn/gtwngatrfv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.guowangkeji.top/gtrwzrffal.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenzaomai.com/gtsepgdowh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cqqwz.cn/gtdbnmemnq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tanke756.top/gtpbaprcdk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinghuilouyu.cn/gtchfdmuvg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinyuanbaomall.cn/gtgzrocwof.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nanxinkj.top/gteumrnagw.html

[B07] while 循环
来源：http://hz.yuanzhike.top/gtpiyycuef.html

Py:   while i < 10: i += 1
来源：http://hz.redwolf501.top/gtbmhucigv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ivvv.top/gtmiytynqg.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtjmhaxgfm.html

TS:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtjrbgrrli.html

Java: while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtwlhldeny.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.havefunace.top/gtdgtrzrkw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.fengsongda.top/gtgpjajdnj.html

C#:   while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gtazrrbyqd.html

[B08] do-while（至少执行一次）
来源：http://hz.hammf.cn/gttmicrdsl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yuanzhike.top/gtpkbsleze.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.fengsongda.top/gtuurohrzo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gttzpsbhbu.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtbqfefpai.html

Java: do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtvymqcbcq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnxiangtu.top/gtnfxewqls.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ivvv.top/gtpunryevi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtmduqvrsq.html

[B09] break 与 continue
来源：http://hz.yj20258888.top/gtiqfcovdf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinyuanbaomall.cn/gtagqwtbxm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cheryme.top/gtvyptfktu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtnqzfrimt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gtsyjumgnk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtillcajpd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ehwqpu.com/gtyntjtrgq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sxryk.cn/gtmxaxgjeq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtenvlysce.html

[B10] 遍历同时拿索引
来源：http://hz.zhaomingkeji.xyz/gtarnuyxee.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj20258888.top/gtxqygydxb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.wangshuangyany.cn/gtmofngbep.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtwctcgmfn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtjdkitgrz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ydjk.org.cn/gtykawkcnu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yongpay.top/gtfadoless.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cucudq.cn/gttopayoph.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.quarkkingdee.top/gtviybgmeg.html

[B11] 生成数字序列 / 区间
来源：http://hz.ywan-chungtsiang.top/gtomjyqmbe.html

Py:   list(range(0, 10, 2))
来源：http://hz.ywan-chungtsiang.top/gtyxkpzmfh.html

PHP:  range(0, 10, 2);
来源：http://hz.sufxvd.cn/gtzwjyfdfy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zdqjudy.top/gtawmvduup.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pengpengdd.cyou/gteavhagad.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtiuihqyux.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.0kj1m.cn/gtznimzgst.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhoulong.xyz/gttujmevex.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.andypj.xyz/gtjcvfssbg.html

[B12] 跳出多层循环
来源：http://hz.birdmap.top/gtegomntwd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xylfe.cn/gtrjdeqedx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yonumen.top/gttipcljgc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtcabjxkvg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtebgyakve.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtpkydnylq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.52xcode.cn/gtavnurnaq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gogol.net.cn/gtmhlzhgat.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nanxuanxn.top/gtzvocbvbu.html

[B13] 判断是否为数字
来源：http://hz.pengpengdd.cyou/gtyviqjunr.html

Py:   isinstance(x, (int, float))
来源：http://hz.cqqwz.cn/gtjvnmktpp.html

PHP:  is_numeric($x)
来源：http://hz.hysaishi.cn/gtfmlnfjad.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtillmwiis.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtvjthfkca.html

Java: x instanceof Number
来源：http://hz.snrcjt.cn/gtuvimhgmu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yuxming.cn/gtkqsfwvgv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gotoacloud.top/gtyyoaokkw.html

C#:   x is int or double or decimal
来源：http://hz.c1oappe.top/gtwapcpakb.html

[B14] 判断值是否在集合内
来源：http://hz.chenlongwang.top/gtfcjjofun.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cqqwz.cn/gtyxuydehc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.redwolf501.top/gtfsoaaafu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gotoacloud.top/gtpmysmmch.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jqgufenzy.top/gtxbpblbaj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yvedp.cn/gtmoadfrea.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtvlryghjl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.52xcode.cn/gtjgwvvhtd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.mhx1999.top/gtlsdqiors.html

[B15] 布尔运算与取反
来源：http://hz.hysaishi.cn/gtssebwvys.html

Py:   a and b or not c
来源：http://hz.yueranfly.top/gtiscdlxie.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gtmqshsmkf.html

JS:   a && b || !c
来源：http://hz.chenlongwang.top/gttjagsjyz.html

TS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtlpsrqttk.html

Java: a && b || !c
来源：http://hz.hfpthk.cn/gtdijblome.html

Go:   a && b || !c
来源：http://hz.yvedp.cn/gtmzvhkijj.html

Ruby: a && b || !c
来源：http://hz.birdmap.top/gtfcxmuzdv.html

C#:   a && b || !c
来源：http://hz.zycfv.cn/gttkojjobu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nwbrower.top/gtcqrgvppt.html

Py:   if not data: return
来源：http://hz.xziqi.cn/gtztqpuzki.html

PHP:  if (!$data) { return; }
来源：http://hz.hnqzz.top/gtnjoaobyw.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gthdiahoxd.html

TS:   if (!data) return;
来源：http://hz.kuanghao11.cn/gtijleotug.html

Java: if (data == null) return;
来源：http://hz.hammf.cn/gtwwzeoirl.html

Go:   if data == nil { return }
来源：http://hz.havefunace.top/gtusgusrcx.html

Ruby: return if data.nil?
来源：http://hz.dashuyun.cn/gtymnwawcf.html

C#:   if (data == null) return;
来源：http://hz.tianlin.xyz/gtcizfiyru.html

================================================================================
来源：http://hz.xuanzx.com/gtbdvvlvlm.html

C. 函数与作用域
来源：http://hz.hnqzz.top/gtlgcpwxtd.html

================================================================================
来源：http://hz.cdnleiting.top/gtzfcpnelc.html

[C01] 定义函数
来源：http://hz.yuxming.cn/gteykjuuav.html

Py:   def add(a, b): return a + b
来源：http://hz.gogol.net.cn/gtbqdepqcm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtyquqpapq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xinyue.icu/gtnqpcuqsz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtogzgqydv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtrwxiddbi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinyuanbaomall.cn/gttobhbcif.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgufenzy.top/gtyhedjxxg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gthjyztlik.html

[C02] 默认参数
来源：http://hz.316326.xyz/gtxrpjjzuo.html

Py:   def greet(name="World"): return name
来源：http://hz.yangfankeji.com/gttkgovmyu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj202588.top/gtaoxlgdwb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenzaomai.com/gtmesjgnof.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtibcidacn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fzhhl.top/gturqnqzbk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hysaishi.cn/gttocmconb.html

Ruby: def greet(name = "World") = name
来源：http://hz.aizwys.cn/gtwxuygttt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zdqjudy.top/gthnsatdle.html

[C03] 可变参数
来源：http://hz.tianlin.xyz/gtytgycght.html

Py:   def total(*args): return sum(args)
来源：http://hz.sufxvd.cn/gtekdjzxox.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnxiangtu.top/gtdvvkkirc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtvxoezezz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtczbgdwvg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenzaomai.com/gtetqjrpmb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.guowangkeji.top/gtgsiyjvzk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ybcxt.top/gtyaubrvks.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shanyushiyangkeji.top/gthstnxpfw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hongshengwenyu.top/gtzzexxleu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnqzz.top/gtegzddwoy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtezufvbkz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtwrzhworf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yvedp.cn/gtnqgtxpph.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhijiandao.cn/gtkchfcake.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxuanxn.top/gtpcbjjbks.html

Ruby: f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtdmwucbsi.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtwzpcjcpf.html

[C05] 返回多个值
来源：http://hz.ydzc1.top/gttwzggvfh.html

Py:   return a, b
来源：http://hz.jqgfzy.top/gtylkdvxsb.html

PHP:  return [$a, $b];
来源：http://hz.cqqwz.cn/gtlrpijzgj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yuanzhike.top/gtrfjrhqdw.html

TS:   return { a, b };
来源：http://hz.shzxlz.cn/gttfjorzar.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dianchejie.cn/gtgxrlgtcm.html

Go:   return a, b
来源：http://hz.pengpengdd.cyou/gtbgrgufla.html

Ruby: return a, b
来源：http://hz.meibo888.top/gtdaxpawoo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sxryk.cn/gtiqsntzrz.html


<!-- 参考信息 -->