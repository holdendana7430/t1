代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.pycfn.com/gtezxznruo.html

Ruby: gets.chomp
来源：http://hz.jinyuanbaomall.cn/gtjmwzsujn.html

C#:   Console.ReadLine();
来源：http://hz.hfpthk.cn/gtpknozqqq.html

[A21] 保留指定小数位输出
来源：http://hz.shuidangran.top/gtrbnxownn.html

Py:   f"{3.14159:.2f}"
来源：http://hz.feifeiyinyue.top/gthsteizdk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yueranfly.top/gtpskwcatr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.quarkkingdee.top/gtqmfblckg.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtrrmrtgqb.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yvedp.cn/gtgaqcskto.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.smart0.xyz/gtrcsdiasg.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtjauljdve.html

C#:   3.14159.ToString("F2")
来源：http://hz.sxryk.cn/gtklfivssy.html

[A22] 获取字符串长度
来源：http://hz.vqdsnc.cn/gtwncwqbss.html

Py:   len(s)
来源：http://hz.yangfankeji.com/gththucqye.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.sweek.top/gtumywjobb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.gaohongyu789.top/gtiekgmkmv.html

TS:   s.length
来源：http://hz.mhx1999.top/gtbjqwzmie.html

Java: s.length()
来源：http://hz.shzxlz.cn/gtcydqgwfx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.quarkkingdee.top/gthyiwynke.html

Ruby: s.length
来源：http://hz.fengsongda.top/gtbrlcaabt.html

C#:   s.Length
来源：http://hz.xinyue.icu/gtfzcqwgzc.html

[A23] 大小写转换
来源：http://hz.yanxiufei.cn/gtmextcoah.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gotoacloud.top/gtuaducfie.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.guannengcc.top/gtmtxqfvmp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gtvbnxyqdf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sufxvd.cn/gthvxscuom.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangtech.top/gtslqwprfg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.sxryk.cn/gtjfpmmckn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xylfe.cn/gtsolurbbl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.vqdsnc.cn/gtykdnhrlk.html

[A24] 去除首尾空白
来源：http://hz.hammf.cn/gtzpfvgiml.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shuidangran.top/gttelbcnil.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hnxiangtu.top/gtljhpuauc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.316326.xyz/gtwmxgyfyi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.havefunace.top/gtrcpsrmal.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hysaishi.cn/gtowzzzysy.html

Go:   strings.TrimSpace(s)
来源：http://hz.cqqwz.cn/gtmfqvsspi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ehwqpu.com/gtrfwcpgmq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.sxryk.cn/gtgjnsbyog.html

[A25] 字符串比较
来源：http://hz.sysykeji.top/gtwbomqehp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhaomingkeji.xyz/gtldbwzfov.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sweek.top/gtixhiycca.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sxryk.cn/gtktzeincj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhongyouzk.top/gtnilzveag.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.52xcode.cn/gtpqiiknps.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ehwqpu.com/gtkdqkunlk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.cqqwz.cn/gtnwpyvoxr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.quarkkingdee.top/gtggyiidkx.html

[A26] 类型转换总览
来源：http://hz.daria6918.cn/gtqztvldok.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.tanke756.top/gtvxzubnai.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.snrcjt.cn/gtvpannesx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sweek.top/gtjxnzdzdz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shuidangran.top/gtgwdalffe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jianghu66.top/gthjzgncrk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jinqigufen.top/gtjdtttfjc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.redwolf501.top/gtswepvgth.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.guannengcc.top/gtfctjjufm.html

================================================================================
来源：http://hz.ydzc1.top/gthllpbzup.html

B. 流程控制
来源：http://hz.cdnleiting.top/gtdorjkvic.html

================================================================================
来源：http://hz.havefunace.top/gtmhlzzyco.html

[B01] 条件判断 if / else
来源：http://hz.52xcode.cn/gtbdtryqdw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.chenzaomai.com/gtkcounnhd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yonumen.top/gtzkspvrjz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.andypj.xyz/gtcslctfsk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gthlkovinh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtragbzehz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xziqi.cn/gtogvfunpm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sufxvd.cn/gtywcabswv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtxrzvmbft.html

[B02] 多分支 else if / elif
来源：http://hz.zhoulong.xyz/gtqhxpqajt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yvedp.cn/gtbloxzxvi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jlsjyb.cn/gtzubhztjl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.bjfxy.top/gtiftoveom.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtozrkvkdl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtykvqphwh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.c1oappe.top/gtkbbfyubz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yj20258888.top/gtbgigdkod.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gtpcvuwzys.html

[B03] switch / match / case
来源：http://hz.guannengcc.top/gtoisgqzyn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cashguo.top/gtftinbqms.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.smart0.xyz/gtzhmuftza.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhiwuduotai.top/gtqnjyxrbr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gaohongyu789.top/gtvrtmyohe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jqgfzy.top/gtkfpjcnyg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.feifeiyinyue.top/gtsuzhdsji.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.tanke756.top/gtokkrgzbp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.wangdashe.top/gtzgakmpez.html

[B04] for 计数循环
来源：http://hz.gogol.net.cn/gtblnczzbt.html

Py:   for i in range(10): print(i)
来源：http://hz.xuetiantiany.cn/gtbbbivuxc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jlsjyb.cn/gtxaodbymw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.daria6918.cn/gtgklumrhh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fzhhl.top/gtyxcksuis.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ivvv.top/gthnvtkeks.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yonumen.top/gtmkizthtl.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhoulong.xyz/gtkvfudyhd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hammf.cn/gtjdowqsii.html

[B05] 遍历数组 / 列表
来源：http://hz.nanxinkj.top/gtcyjstilr.html

Py:   for item in arr: print(item)
来源：http://hz.hywenlv.cn/gtxkwqhadd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.fengsongda.top/gtxvwgcdrt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yongpay.top/gtxljzrjmg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.smart0.xyz/gtuekulzkb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhongyouzk.top/gtwfulabvl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.9152youxi.cn/gtbfaxkaxt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhoulong.xyz/gtywnjebty.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jiagoushi.top/gtgbkvcymn.html

[B06] 遍历字典 / 对象
来源：http://hz.hysaishi.cn/gtvavwxwcc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.svipenyu.cn/gtizkucfto.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shanyushiyangkeji.top/gtxlpddojj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.guowangkeji.top/gtqhakvsws.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinghuilouyu.cn/gtxsmltwtf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.andypj.xyz/gttsasrtig.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shanyushiyangtech.top/gtydiiprca.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xingfuxueyuan.xyz/gtypbgakpq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yj202588.top/gtaqdmflxa.html

[B07] while 循环
来源：http://hz.316326.xyz/gttmjmwzbj.html

Py:   while i < 10: i += 1
来源：http://hz.yangfankeji.com/gtgzoohrgl.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.havefunace.top/gtrevksile.html

JS:   while (i < 10) { i++; }
来源：http://hz.shzxlz.cn/gtlmqoblug.html

TS:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtwpblyoht.html

Java: while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtnkhrzjra.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gogol.net.cn/gtrhggzjga.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xingfuxueyuan.xyz/gtbfpzhpiv.html

C#:   while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtnasxucvn.html

[B08] do-while（至少执行一次）
来源：http://hz.daxiang520.top/gtwqlnpwfb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cheryme.top/gtawyirfoe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.birdmap.top/gtpkybjody.html

JS:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtmubigxrm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtuorkbytj.html

Java: do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtcskujoel.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cucudq.cn/gtlqgugcsv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cashguo.top/gthlhhytws.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtebzbffma.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gtvjuxgnhb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.0kj1m.cn/gtbellqtfe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zdqjudy.top/gtkwvrzpmg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gttjvtjrpp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtiyxgyaog.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtkajhggvk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258.top/gtlwbxvxfa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.havefunace.top/gthmvqbpsv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtvqeqmdln.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258888.top/gtmvxcxivu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenjidiqi.icu/gtkryycbxo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yuanzhike.top/gtfbgqztad.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.meibo888.top/gtkvaglsxg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtozdnnivq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hysaishi.cn/gtetroevhm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pengpengdd.cyou/gtsuxokltv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guannengcc.top/gtohlzxdla.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hongshengwenyu.top/gtdmcbsysu.html

[B11] 生成数字序列 / 区间
来源：http://hz.cucudq.cn/gtaaewihxs.html

Py:   list(range(0, 10, 2))
来源：http://hz.sufxvd.cn/gtbaxlektw.html

PHP:  range(0, 10, 2);
来源：http://hz.shangyingyoupin.top/gtnuyuynrt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aizwys.cn/gtyyyfgbak.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sysykeji.top/gtmjjnvwka.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.iojbl.cn/gtijjszmac.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.aizwys.cn/gtyelfratw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gzhubu.top/gtweijgfpi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shanyushiyangkeji.top/gtnsxygqgu.html

[B12] 跳出多层循环
来源：http://hz.pengpengdd.cyou/gttblkvvph.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ivvv.top/gtsazkfxhp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gotoacloud.top/gtmxxdtywx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtdyqqunlu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtnukjjyfq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gtztnsenig.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangtech.top/gthuduxiwg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ywan-chungtsiang.top/gtapzumgrr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yueranfly.top/gtlmmjrkcx.html

[B13] 判断是否为数字
来源：http://hz.hammf.cn/gtunzcermr.html

Py:   isinstance(x, (int, float))
来源：http://hz.kuanghao11.cn/gtqaehedpl.html

PHP:  is_numeric($x)
来源：http://hz.snrcjt.cn/gtoraqxssy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtmalrboif.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtcqacxixa.html

Java: x instanceof Number
来源：http://hz.hnxiangtu.top/gtuespevcr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ppjwa.cn/gtdgtcevca.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ppjwa.cn/gtefxccyiq.html

C#:   x is int or double or decimal
来源：http://hz.gogol.net.cn/gtdzxcseig.html

[B14] 判断值是否在集合内
来源：http://hz.xinyue.icu/gtkynoscig.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jyoumei.cn/gtranzyjnz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cheryme.top/gtczpopumr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtxhwdnyxw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gtxoqhdpvx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxinkj.top/gtxpyqseyv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.9152youxi.cn/gtbgusotrn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuetiantiany.cn/gtjhlbrcyo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj202588.top/gtjcpxyecs.html

[B15] 布尔运算与取反
来源：http://hz.iojbl.cn/gtytkvkvye.html

Py:   a and b or not c
来源：http://hz.daxiang520.top/gtvwkehcww.html

PHP:  $a && $b || !$c
来源：http://hz.guowangkeji.top/gtrcahwnto.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gteizeciwz.html

TS:   a && b || !c
来源：http://hz.ehwqpu.com/gtotmdwpvo.html

Java: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtbdpbfaua.html

Go:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtlbtwqdzx.html

Ruby: a && b || !c
来源：http://hz.shangyingyoupin.top/gtstunpcoy.html

C#:   a && b || !c
来源：http://hz.zhijiandao.cn/gtfuvnsfii.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtrnpaywtm.html

Py:   if not data: return
来源：http://hz.gogol.net.cn/gtvpiooxdl.html

PHP:  if (!$data) { return; }
来源：http://hz.c1oappe.top/gtzpfzusce.html

JS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gthgyzqryf.html

TS:   if (!data) return;
来源：http://hz.xziqi.cn/gtochkxffj.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtmkzwakbx.html

Go:   if data == nil { return }
来源：http://hz.ybcxt.top/gtlynrsxnj.html

Ruby: return if data.nil?
来源：http://hz.feifeiyinyue.top/gtdgmbsivn.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtkselilmk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkihcytku.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gtdbymhadj.html

================================================================================
来源：http://hz.cheryme.top/gtmlrabrzc.html

[C01] 定义函数
来源：http://hz.nanxinkj.top/gtzzxnjweu.html

Py:   def add(a, b): return a + b
来源：http://hz.mhx1999.top/gtxraycxlr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtpeezkbbi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtfshdfhgb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtfqvjldnv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gttjblbrzr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.0kj1m.cn/gtmgrkkcxr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.pengpengdd.cyou/gtrdpbjdeg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtpegzqpxs.html

[C02] 默认参数
来源：http://hz.yj20258.top/gtsjzlixwz.html

Py:   def greet(name="World"): return name
来源：http://hz.hammf.cn/gtaqaglifq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.vqdsnc.cn/gtyzyjsmoa.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ppjwa.cn/gttmrauggq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgufenzy.top/gtncarkuqk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dianchejie.cn/gtbhdwqybn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hammf.cn/gttunqyqnp.html

Ruby: def greet(name = "World") = name
来源：http://hz.52xcode.cn/gtcpymilyt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.haohaochexian.top/gtzutcuvvz.html

[C03] 可变参数
来源：http://hz.ybcxt.top/gtathtjpon.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtehfntnsp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pengpengdd.cyou/gtigsvdugg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtbqykuxhn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigufen.top/gtuyowjndk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.redwolf501.top/gtwsguiiov.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhengqikj.top/gtcsshtopf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtkjfofyci.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj202588.top/gtrgitajqx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj20258888.top/gtuedexxjm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangdashe.top/gtiaccmliy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cqqwz.cn/gtuaczgtvx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtnvbuiqlz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jiagoushi.top/gtldtdxdzh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.meibo888.top/gtxuuznelk.html

Go:   // 无：用配置结构体参数
来源：http://hz.pycfn.com/gtkforsxpw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtgjqnhzur.html

C#:   f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtblvuzugd.html

[C05] 返回多个值
来源：http://hz.kuanghao11.cn/gtwswpghjg.html

Py:   return a, b
来源：http://hz.jinqigufen.top/gtgqxnjpvz.html

PHP:  return [$a, $b];
来源：http://hz.feifeiyinyue.top/gtyoqwzfzu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj20258888.top/gtngipzzey.html

TS:   return { a, b };
来源：http://hz.redwolf501.top/gtkdqbxjja.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pycfn.com/gtianmoxob.html

Go:   return a, b
来源：http://hz.yuxming.cn/gtqxsrldqz.html

Ruby: return a, b
来源：http://hz.zycfv.cn/gtvnkmorxu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cdnleiting.top/gtrbkztwek.html

[C06] 匿名函数 / lambda
来源：http://hz.shanyushiyangtech.top/gtaqzimufn.html

Py:   square = lambda x: x * x
来源：http://hz.aizwys.cn/gtszgxkene.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tanke756.top/gtenynyvkz.html

JS:   const square = x => x * x;
来源：http://hz.aibaodan.cn/gtytyapffy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtyfgvoliu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtmodprdqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj202588.top/gtctpsiuxu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yuxming.cn/gtmyugajku.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.guowangkeji.top/gtwcenqqvc.html

[C07] 把函数作为参数传入
来源：http://hz.kuanghao11.cn/gttwydzyhv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.havefunace.top/gtwspwyfeh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nwbrower.top/gtsjmxzyqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ybcxt.top/gtlpzfjatq.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gtopbdgljw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yangfankeji.com/gttdtbqowe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shuidangran.top/gtbxqwscmx.html

Ruby: arr.map(&:upcase)
来源：http://hz.jlsjyb.cn/gtddhagyyq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gthsvyhrgh.html

[C08] 闭包
来源：http://hz.hnqzz.top/gtgaeazsyd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258888.top/gtxpkmbanp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xziqi.cn/gtlvtdhsio.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtwnyratbq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtqynmjcqq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jiagoushi.top/gtgvnodbgg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.andypj.xyz/gtmwrwigrs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.birdmap.top/gtleriwkvr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gthknphpyx.html

[C09] 递归
来源：http://hz.fzhhl.top/gtzfxqjeev.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtirglahet.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhixingplan.top/gtjyzirnwd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daria6918.cn/gtycclkrkt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hysaishi.cn/gtuuxdgirz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.vqdsnc.cn/gthlvilypc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yueranfly.top/gtmlqjppad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtbtbourir.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.snrcjt.cn/gtzbiwpdny.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtypoyabuj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gtulxyfpdq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangshuangyany.cn/gtuhpxlpdn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinghuilouyu.cn/gtzhhxftwe.html

TS:   同 JS
来源：http://hz.52xcode.cn/gtmkwxmhfu.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtmnueizty.html

Go:   花括号块级作用域
来源：http://hz.mhx1999.top/gtgyhapumn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yangfankeji.com/gtsggqvbru.html

C#:   块级作用域
来源：http://hz.guowangkeji.top/gtuqbmybim.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtlpduwzvq.html

Py:   from module import func
来源：http://hz.guowangkeji.top/gtuyzagryo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yonumen.top/gtehdbixyt.html


<!-- 参考信息 -->