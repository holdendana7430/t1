代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.jlsjyb.cn/gtqeknsufx.html

TS:   const value = data ?? "默认值";
来源：http://hz.redwolf501.top/gtxostbftd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hongshengwenyu.top/gtmilmrdot.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.daxiang520.top/gtqpsdpapo.html

Ruby: value = data || "默认值"
来源：http://hz.yuxming.cn/gtvoavxukq.html

C#:   var value = data ?? "默认值";
来源：http://hz.sysykeji.top/gteypcrgfq.html

[A16] 真假值判断规则
来源：http://hz.shanyushiyangkeji.top/gtqjkmzlno.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.wangshuangyany.cn/gtocisqblp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.mhx1999.top/gtyfcuhtwe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hammf.cn/gtioogasai.html

TS:   if (!x) {}
来源：http://hz.iojbl.cn/gtjqgfyjtd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hammf.cn/gtkxponmrb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.316326.xyz/gtctefkudf.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.haohaochexian.top/gtypsskqno.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.pycfn.com/gtejbkicdb.html

[A17] 位运算
来源：http://hz.zhaomingkeji.xyz/gtlqoiksco.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhengqikj.top/gtqaonxuut.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.chenlongwang.top/gtqxbkfnlf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtkaejqhsc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtjwmicsoi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.redwolf501.top/gtiuylfwdm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtiigzwcoq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtyzkcibzx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.andypj.xyz/gtxgpmjcmt.html

[A18] 字符与 ASCII 码互转
来源：http://hz.tanke756.top/gtsbfxxhdm.html

Py:   ord("A"); chr(65)
来源：http://hz.zhiwuduotai.top/gtvovxjlnk.html

PHP:  ord("A"); chr(65)
来源：http://hz.xingfuxueyuan.xyz/gtlxzbhxju.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxinkj.top/gtmuvdjkeq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cashguo.top/gtszqjstbi.html

Java: (int) 'A'; (char) 65
来源：http://hz.tianlin.xyz/gtetzwhwby.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.gotoacloud.top/gtbuslrdbh.html

Ruby: "A".ord; 65.chr
来源：http://hz.chenjidiqi.icu/gtnhthlayv.html

C#:   (int)'A'; (char)65
来源：http://hz.hnqzz.top/gtjmgvqksb.html

[A19] 交换两个变量
来源：http://hz.birdmap.top/gtakbsohoh.html

Py:   a, b = b, a
来源：http://hz.daria6918.cn/gtrftbdjde.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hnxiangtu.top/gtxkgbnkfk.html

JS:   [a, b] = [b, a];
来源：http://hz.jinyuanbaomall.cn/gtwdchcsxe.html

TS:   [a, b] = [b, a];
来源：http://hz.nanxuanxn.top/gtwlqpxrjf.html

Java: int t = a; a = b; b = t;
来源：http://hz.guannengcc.top/gtggckrjkl.html

Go:   a, b = b, a
来源：http://hz.iojbl.cn/gttyzxbgpw.html

Ruby: a, b = b, a
来源：http://hz.sweek.top/gtnvpnvezp.html

C#:   (a, b) = (b, a);
来源：http://hz.316326.xyz/gthfjxrmah.html

[A20] 读取标准输入
来源：http://hz.jqgufenzy.top/gtoggaabwo.html

Py:   name = input("请输入：")
来源：http://hz.andypj.xyz/gtmybfmbkn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cqqwz.cn/gtxqmwltgj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shanyushiyangkeji.top/gthppxgivc.html

TS:   // Node.js：readline 模块
来源：http://hz.jlsjyb.cn/gtmpbkdykb.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.wangshuangyany.cn/gtoywsduew.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.9152youxi.cn/gtblmxvjfk.html

Ruby: gets.chomp
来源：http://hz.meibo888.top/gtjrruisgb.html

C#:   Console.ReadLine();
来源：http://hz.sweek.top/gtxuaardsu.html

[A21] 保留指定小数位输出
来源：http://hz.yvedp.cn/gtyvjzxgfa.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jyoumei.cn/gtgbgcsrjw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jinghuilouyu.cn/gtxwmszplo.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtjqepxden.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yj20258.top/gtkgdgkrtd.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtksavckvm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.chenjidiqi.icu/gtuqmmtouk.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yj20258.top/gtapgmcbuf.html

C#:   3.14159.ToString("F2")
来源：http://hz.sufxvd.cn/gtvfchsjyc.html

[A22] 获取字符串长度
来源：http://hz.dashuyun.cn/gtqxbwuepg.html

Py:   len(s)
来源：http://hz.jlsjyb.cn/gtvnygnzht.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.nwbrower.top/gtogbacdcu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.52xcode.cn/gtjrpgtixv.html

TS:   s.length
来源：http://hz.jyoumei.cn/gtxkvhhlde.html

Java: s.length()
来源：http://hz.ehwqpu.com/gtmodyybrp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.ehwqpu.com/gtudmakyea.html

Ruby: s.length
来源：http://hz.shanyushiyangkeji.top/gtklwhyzzq.html

C#:   s.Length
来源：http://hz.ydjk.org.cn/gtevkuffbx.html

[A23] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtjqqjnwag.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hammf.cn/gtqfwucgqw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ydjk.org.cn/gtfrmxryhp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zdqjudy.top/gtvyighlot.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.52xcode.cn/gtksmsrunx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.52xcode.cn/gtdesjlylg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinqigfzy.top/gtdpaglzbt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yuanzhike.top/gttfrhrmkm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhengqikj.top/gthihncgpn.html

[A24] 去除首尾空白
来源：http://hz.sufxvd.cn/gtdnexklvi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yueranfly.top/gtyvfznveg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.snrcjt.cn/gtzlyenmod.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.kuanghao11.cn/gtyszcxyrt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jiagoushi.top/gtmiqzygyh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hywenlv.cn/gtsyaqauww.html

Go:   strings.TrimSpace(s)
来源：http://hz.0kj1m.cn/gteeiifcpd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hnqzz.top/gtsgsdgbxf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.gotoacloud.top/gtreoapbno.html

[A25] 字符串比较
来源：http://hz.ivvv.top/gtbilrmjqk.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yj20258888.top/gtqwsnatdi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cheryme.top/gtfvutawep.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aibaodan.cn/gtreytgazw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gtvfidzeah.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ivvv.top/gtyckadxna.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.chenjidiqi.icu/gtpmeinity.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.nanxuanxn.top/gtyrjzvfsh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.c1oappe.top/gtikjokqfk.html

[A26] 类型转换总览
来源：http://hz.xuanzx.com/gtwzdjufks.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.0kj1m.cn/gtbxjfcijx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.mhx1999.top/gtdixotqsp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhengqikj.top/gthrlecbkg.html

TS:   Number() String() Boolean() x as number
来源：http://hz.hnqzz.top/gtimstadex.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.haohaochexian.top/gtgtgoyrgp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.redwolf501.top/gtuacmaynk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.tianlin.xyz/gtgrgoijjn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hnqzz.top/gtqlvxkeli.html

================================================================================
来源：http://hz.haohaochexian.top/gtwzqtelmx.html

B. 流程控制
来源：http://hz.nanxuanxn.top/gtvzvpnsfn.html

================================================================================
来源：http://hz.xinyue.icu/gtfxbmbhtr.html

[B01] 条件判断 if / else
来源：http://hz.ivvv.top/gtjbddqvtb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jqgufenzy.top/gtqypyaqft.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ybcxt.top/gtlmlvroar.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangkeji.top/gtzhpbgsqe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cheryme.top/gtahebutee.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gttvwfwcjv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dashuyun.cn/gtcyydaxkw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sweek.top/gtdmrtzqwv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtybkcodxk.html

[B02] 多分支 else if / elif
来源：http://hz.shanyushiyangkeji.top/gtrnincdow.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.meibo888.top/gtijjdmjrk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.nwbrower.top/gtdchdgbcu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtsuwxyqrn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ivvv.top/gtfzfqmlfj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtlblyqgkq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xingfuxueyuan.xyz/gtgxoogffn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jianghu66.top/gtnevloomp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtowdzionf.html

[B03] switch / match / case
来源：http://hz.hnqzz.top/gtxxbrmgfl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258888.top/gtecqevdce.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinqigfzy.top/gtgwdskgui.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cheryme.top/gtfvbytqku.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtnspwilpe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yvedp.cn/gtikhsbncx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinqigfzy.top/gtqgdlyqhl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yj20258.top/gtamoifctw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cheryme.top/gteopvmlxh.html

[B04] for 计数循环
来源：http://hz.jinqigufen.top/gtedugucia.html

Py:   for i in range(10): print(i)
来源：http://hz.chenlongwang.top/gtgiipehcg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.fengsongda.top/gtlbybcixr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.mhx1999.top/gtjilbzibz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shzxlz.cn/gtrpvzhfbd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.iojbl.cn/gtpyijlchv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.nanxuanxn.top/gtamxpflrc.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ywan-chungtsiang.top/gthcaokgwc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.havefunace.top/gtalljphcj.html

[B05] 遍历数组 / 列表
来源：http://hz.redwolf501.top/gtgrrnchzs.html

Py:   for item in arr: print(item)
来源：http://hz.yj20258.top/gtinaevjws.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.fengsongda.top/gtyqkzijkh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cqqwz.cn/gtikzbzrhr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hysaishi.cn/gtnqntlkok.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj202588.top/gtokuibedb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ppjwa.cn/gtwkqqbqrd.html

Ruby: arr.each { |item| puts item }
来源：http://hz.feifeiyinyue.top/gtpzmczhkn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangdashe.top/gtwydzvaae.html

[B06] 遍历字典 / 对象
来源：http://hz.cqqwz.cn/gtvnrmvbnu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.smart0.xyz/gtfnsndnxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.0kj1m.cn/gtaiweflmw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yanxiufei.cn/gtkmbmegkj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj202588.top/gtheqoczki.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aibaodan.cn/gtjwllzgok.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yangfankeji.com/gtsystchmz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.fengsongda.top/gtrhacjana.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jyoumei.cn/gtyujzwcng.html

[B07] while 循环
来源：http://hz.sysykeji.top/gtovhjccfh.html

Py:   while i < 10: i += 1
来源：http://hz.jinghuilouyu.cn/gtzqnrwazo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.birdmap.top/gtvpresdwc.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhengqikj.top/gtpfhmtchk.html

TS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtfujzdvvl.html

Java: while (i < 10) { i++; }
来源：http://hz.svipenyu.cn/gtgbzjrrxc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daria6918.cn/gtqmjuzsom.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtzuvxkgbj.html

C#:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtoqylmqtr.html

[B08] do-while（至少执行一次）
来源：http://hz.snrcjt.cn/gtaqbofhkv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.fzhhl.top/gtesxrrcor.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gzhubu.top/gtbymxzkmi.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtqnldixzg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gthqrkyrjj.html

Java: do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtdzsufvoz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jiagoushi.top/gtzulmcdgm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenjidiqi.icu/gtzfdyzetx.html

C#:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtlcoyqjfe.html

[B09] break 与 continue
来源：http://hz.shanyushiyangkeji.top/gtisrcnkdj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yanxiufei.cn/gtferhbirs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtmmfngoah.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtdzbmdmlo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtgpoensaa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtslcluiub.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.aizwys.cn/gtbblvikfm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hywenlv.cn/gtcgkviqbj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtjfytonax.html

[B10] 遍历同时拿索引
来源：http://hz.hysaishi.cn/gtmqhizdcr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.quarkkingdee.top/gtbsiwiaqu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.316326.xyz/gtyjnvvncx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daxiang520.top/gtnvzvieie.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jiagoushi.top/gtayaczcvl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtxbtxorvx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.daria6918.cn/gtjupfxukn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.daxiang520.top/gtjgijfdat.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj20258.top/gthlppklpk.html

[B11] 生成数字序列 / 区间
来源：http://hz.redwolf501.top/gtnfnmzqyd.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxuanxn.top/gtmdixmufl.html

PHP:  range(0, 10, 2);
来源：http://hz.birdmap.top/gtyacvnbhd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jlsjyb.cn/gtbhwilvha.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgufenzy.top/gtxflelvxg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jianghu66.top/gthtegbkxu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yuanzhike.top/gtrbeczoqv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gtgcrnojax.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtigbpihcn.html

[B12] 跳出多层循环
来源：http://hz.zhijiandao.cn/gtmncpzpno.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jianghu66.top/gtwrzpztmm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shangyingyoupin.top/gtzyshpuot.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtmvtubysk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtwxjzyofi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gttvtwwxut.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yonumen.top/gtuowaprxc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.andypj.xyz/gtaluojulu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tanke756.top/gtdnagtmbc.html

[B13] 判断是否为数字
来源：http://hz.aizwys.cn/gtsbzccxho.html

Py:   isinstance(x, (int, float))
来源：http://hz.hammf.cn/gtzslqwanz.html

PHP:  is_numeric($x)
来源：http://hz.feifeiyinyue.top/gtzmmmarvb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fengsongda.top/gtfhyvaxyq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ivvv.top/gteprhiyph.html

Java: x instanceof Number
来源：http://hz.jinyuanbaomall.cn/gtlwongwfx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.chenlongwang.top/gtxrloiabw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuanzhike.top/gtodmybzyb.html

C#:   x is int or double or decimal
来源：http://hz.jiagoushi.top/gtcucflocs.html

[B14] 判断值是否在集合内
来源：http://hz.9152youxi.cn/gtdsprmgyj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dianchejie.cn/gtpytfixxg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ppjwa.cn/gtuzpaepqz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtpnchvbwl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.bjfxy.top/gtgzckmvbd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhengqikj.top/gtqmryhepu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tian-w.cn/gtpdvyckrz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhijiandao.cn/gtvrwrjwba.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtisbtoand.html

[B15] 布尔运算与取反
来源：http://hz.feifeiyinyue.top/gtthgkfvjw.html

Py:   a and b or not c
来源：http://hz.zdqjudy.top/gtucejysub.html

PHP:  $a && $b || !$c
来源：http://hz.yuxming.cn/gtclqcxjnm.html

JS:   a && b || !c
来源：http://hz.chenlongwang.top/gtyyihjcyr.html

TS:   a && b || !c
来源：http://hz.ppjwa.cn/gtivdormsg.html

Java: a && b || !c
来源：http://hz.yanxiufei.cn/gthdshyryj.html

Go:   a && b || !c
来源：http://hz.316326.xyz/gttlviwuwj.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtsmfnqcpk.html

C#:   a && b || !c
来源：http://hz.0kj1m.cn/gtezglplpl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.mhx1999.top/gttcbiipzd.html

Py:   if not data: return
来源：http://hz.mhx1999.top/gtozhzsyld.html

PHP:  if (!$data) { return; }
来源：http://hz.cucudq.cn/gtmcckzmjn.html

JS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtodfwnupy.html

TS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtoywnpoxx.html

Java: if (data == null) return;
来源：http://hz.sysykeji.top/gtrhwsqfjc.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtqzrrwufd.html

Ruby: return if data.nil?
来源：http://hz.ppjwa.cn/gtsctenrwl.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtgobcahtx.html

================================================================================
来源：http://hz.gogol.net.cn/gtqfuxlufb.html

C. 函数与作用域
来源：http://hz.nanxuanxn.top/gttsgvkmwv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnfrqngbh.html

[C01] 定义函数
来源：http://hz.jqgufenzy.top/gtaoszhgky.html

Py:   def add(a, b): return a + b
来源：http://hz.jinghuilouyu.cn/gtxivagnub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gtdlneweow.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtaeqnudul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gttveispmd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtjwggsppv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sysykeji.top/gtsmwxysyl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zdqjudy.top/gtgijiiixr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtahcoqtdv.html

[C02] 默认参数
来源：http://hz.jqgfzy.top/gtdoqthgqe.html

Py:   def greet(name="World"): return name
来源：http://hz.fengsongda.top/gtkwgcotnm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.quarkkingdee.top/gtoxyzzhyk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtqiqqzuqb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.quarkkingdee.top/gthbladuzy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xingfuxueyuan.xyz/gthdsywxae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.vqdsnc.cn/gtjvfolyyc.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuxming.cn/gtbuwzswob.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sufxvd.cn/gtdujgvqzf.html

[C03] 可变参数
来源：http://hz.tian-w.cn/gtzyawfxix.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtcnnizxud.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhoulong.xyz/gtdbecjacs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtkuxozjwr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtlwalczpj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuanzx.com/gtnjttxblh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yanxiufei.cn/gtvmxqyffh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hammf.cn/gtzhivsymu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.52xcode.cn/gthxgowxpd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.guannengcc.top/gtpaxsotyy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuxming.cn/gtrvvkgjhz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.mhx1999.top/gtofogrqbx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtktmndqzn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtykeytnlw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinyuanbaomall.cn/gtuqmcguit.html

Go:   // 无：用配置结构体参数
来源：http://hz.yongpay.top/gtsnaosmlj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtrrmvlfie.html

C#:   f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtbohqubyh.html

[C05] 返回多个值
来源：http://hz.cashguo.top/gtnsuzcwhl.html

Py:   return a, b
来源：http://hz.52xcode.cn/gtycdrwifn.html

PHP:  return [$a, $b];
来源：http://hz.mhx1999.top/gtlgtjbgfh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenjidiqi.icu/gtftuhndcq.html

TS:   return { a, b };
来源：http://hz.hfpthk.cn/gtxvxabngg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxuanxn.top/gttvbycwqo.html

Go:   return a, b
来源：http://hz.aizwys.cn/gtxbbstgdx.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gtgsxhxlxd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.bjfxy.top/gttrixamqh.html


<!-- 参考信息 -->