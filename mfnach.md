代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://hz.svipenyu.cn/gtqlehcchc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.xuanzx.com/gtphmifyos.html

JS:   (3.14159).toFixed(2)
来源：http://hz.kuanghao11.cn/gtrsgxctkr.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zdqjudy.top/gtqzgfedbv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.nanxuanxn.top/gtfalgcxrx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtdozohvpt.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtpfyeslkx.html

C#:   3.14159.ToString("F2")
来源：http://hz.shanyushiyangkeji.top/gtruxvxbhr.html

[A22] 获取字符串长度
来源：http://hz.kuanghao11.cn/gtwdkkyxnr.html

Py:   len(s)
来源：http://hz.52xcode.cn/gtxtwgpnuv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.316326.xyz/gteijqkcqg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.wangdashe.top/gtigdcbxow.html

TS:   s.length
来源：http://hz.hywenlv.cn/gtinybyhwf.html

Java: s.length()
来源：http://hz.cdnleiting.top/gtewqsgblk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.chenjidiqi.icu/gtahnwzdhn.html

Ruby: s.length
来源：http://hz.fengsongda.top/gtupopkstk.html

C#:   s.Length
来源：http://hz.guannengcc.top/gtboakpqmi.html

[A23] 大小写转换
来源：http://hz.cheryme.top/gtimohmmyh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.daxiang520.top/gttxuobfkk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.jianghu66.top/gtyubiwpqn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtcupelhaw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhijiandao.cn/gtjuwbvgnr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuxming.cn/gtzjuzrwqs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.gotoacloud.top/gtamfynjde.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.cucudq.cn/gttlxbegfg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.guowangkeji.top/gtzkjluvhb.html

[A24] 去除首尾空白
来源：http://hz.wangshuangyany.cn/gtbfjpdfii.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.snrcjt.cn/gtjkmvtthw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xziqi.cn/gtegfgdvex.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ydzc1.top/gtddpvqjlh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangdashe.top/gtgmnxtxli.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.svipenyu.cn/gttdzdekzw.html

Go:   strings.TrimSpace(s)
来源：http://hz.hysaishi.cn/gtyyslabir.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.iojbl.cn/gtfhajvxwl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shangyingyoupin.top/gtnpnxorbb.html

[A25] 字符串比较
来源：http://hz.ydzc1.top/gtxcwgxaxd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cashguo.top/gtyeksvcfl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.mhx1999.top/gtqarygwgw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhixingplan.top/gtzacfgwzp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydzc1.top/gtlqgxpjbs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.c1oappe.top/gtyabpygon.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhoulong.xyz/gtcnkefjfc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shangyingyoupin.top/gtrutqduyz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.smart0.xyz/gtilgdwavc.html

[A26] 类型转换总览
来源：http://hz.0kj1m.cn/gtcygczdnw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.9152youxi.cn/gtmlbjtays.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gzhubu.top/gtrvsucmun.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.aizwys.cn/gtfmswwvul.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cashguo.top/gtytlatunp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.pycfn.com/gtkrjfvedc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.xziqi.cn/gtujdbbwxd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sweek.top/gtgmizkdou.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhiwuduotai.top/gtyjlykurc.html

================================================================================
来源：http://hz.yonumen.top/gtdxoofrhp.html

B. 流程控制
来源：http://hz.jiagoushi.top/gtqtvmycme.html

================================================================================
来源：http://hz.cqqwz.cn/gtknmwblrp.html

[B01] 条件判断 if / else
来源：http://hz.gzhubu.top/gtcablcgpx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xziqi.cn/gtnrfcalob.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yanxiufei.cn/gtdahhkkpr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinyuanbaomall.cn/gtqlqeftrz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtkdsinseg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtmquqnjkg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dianchejie.cn/gtrjqxtmhe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhixingplan.top/gtqpqonvyq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.snrcjt.cn/gtrhaqiccd.html

[B02] 多分支 else if / elif
来源：http://hz.yueranfly.top/gtlyaparsc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhixingplan.top/gttdvrispc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.52xcode.cn/gtoxwgtqdg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtplsglcbs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yueranfly.top/gtiuyrstnb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigfzy.top/gtvitcmsiz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.haohaochexian.top/gtbhkpnxom.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yangfankeji.com/gtedgvmcls.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gtfbqpfeuu.html

[B03] switch / match / case
来源：http://hz.pengpengdd.cyou/gthkeaolhi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sweek.top/gtnlabwjfr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtckpnuezd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.guannengcc.top/gtlfewyvjd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zycfv.cn/gtrdtamgkr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.snrcjt.cn/gtexegikjf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cqqwz.cn/gtbpidjgeh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenjidiqi.icu/gtkmlzjqsk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cdnleiting.top/gttpvqihrn.html

[B04] for 计数循环
来源：http://hz.meibo888.top/gtilupxpzd.html

Py:   for i in range(10): print(i)
来源：http://hz.yj202588.top/gteedpweem.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhengqikj.top/gtgazfdcoa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jqgufenzy.top/gtcsisfjej.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.0kj1m.cn/gtgioipiyz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.daxiang520.top/gtndflnltj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.shuidangran.top/gtcvnmgwyo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jlsjyb.cn/gtxplawfoy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.iojbl.cn/gthnqqphrm.html

[B05] 遍历数组 / 列表
来源：http://hz.havefunace.top/gtdpidihso.html

Py:   for item in arr: print(item)
来源：http://hz.xylfe.cn/gtgprrhiij.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.52xcode.cn/gthldszsii.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtaotiiean.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ehwqpu.com/gtxiupkuvo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.aizwys.cn/gtgwckljdy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.chenzaomai.com/gtlsxbhgyn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shzxlz.cn/gtkvgfgokh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jqgufenzy.top/gtlrnbgnoa.html

[B06] 遍历字典 / 对象
来源：http://hz.jinqigfzy.top/gtxnqcjhfx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xuetiantiany.cn/gtyjybalhs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cqqwz.cn/gtumimqgmz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuxming.cn/gtdmfxnpxn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cqqwz.cn/gtxftfsxun.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sweek.top/gtmvkdngrc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.bjfxy.top/gtejvaxzii.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ywan-chungtsiang.top/gtjkrtsacx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yj20258.top/gtszlrbvfy.html

[B07] while 循环
来源：http://hz.sxryk.cn/gtcbtedokb.html

Py:   while i < 10: i += 1
来源：http://hz.sufxvd.cn/gtuukecewc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.snrcjt.cn/gtrqxxmajp.html

JS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtxejnqxev.html

TS:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtdgmiliqp.html

Java: while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtprzfhtwl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yongpay.top/gtyjkdmqtt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.pycfn.com/gtugueetqb.html

C#:   while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtaetmhzhu.html

[B08] do-while（至少执行一次）
来源：http://hz.ywan-chungtsiang.top/gtjvgrcopc.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hammf.cn/gtegrxaeuz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.9152youxi.cn/gtvfokkysl.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtqtxbgeiz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtgwpvlgrl.html

Java: do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtfqgjmpgf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yuxming.cn/gtmczsloxh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gotoacloud.top/gtyfzjlsax.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtddksuvje.html

[B09] break 与 continue
来源：http://hz.yueranfly.top/gtwzpictvi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yongpay.top/gtdbkwyixs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yuxming.cn/gtbpwyrxap.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtpveehnzc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtckqknjiz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtuarximnc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.feifeiyinyue.top/gtvscusgpk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gtqwtazjpu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtbbuducxz.html

[B10] 遍历同时拿索引
来源：http://hz.pycfn.com/gtlvqfynyf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenjidiqi.icu/gtapivfzcp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.9152youxi.cn/gtbcjyldyl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtnbzjvcuk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.meibo888.top/gtmhkzoutn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tanke756.top/gtcncjzqbr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.smart0.xyz/gthiygqhqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.haohaochexian.top/gtsvzcsdii.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gogol.net.cn/gtpkeimedl.html

[B11] 生成数字序列 / 区间
来源：http://hz.316326.xyz/gtakcircbg.html

Py:   list(range(0, 10, 2))
来源：http://hz.gogol.net.cn/gtexkluwsm.html

PHP:  range(0, 10, 2);
来源：http://hz.ybcxt.top/gtpmalweks.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtqdqxjzda.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtnobbwctn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinghuilouyu.cn/gtfgwkofwd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gzhubu.top/gtiqqyedkr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hysaishi.cn/gtgzmjwcbv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.fzhhl.top/gtroebdfyw.html

[B12] 跳出多层循环
来源：http://hz.xuetiantiany.cn/gtdyeqdiyn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinqigufen.top/gtnddaqwbr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.meibo888.top/gtdtcljlhi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yangfankeji.com/gtljsdotkl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtpqrmnfxz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtcjcmfewk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhengqikj.top/gtfybhqtaq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.daxiang520.top/gtpyzxlmhv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhijiandao.cn/gtzvnxddos.html

[B13] 判断是否为数字
来源：http://hz.smart0.xyz/gtzcjldojf.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhixingplan.top/gtyrnjfyfe.html

PHP:  is_numeric($x)
来源：http://hz.hysaishi.cn/gtbdlsquqv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gtykxngkhh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtasbvuybi.html

Java: x instanceof Number
来源：http://hz.xuanzx.com/gtvxpsffdt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shzxlz.cn/gthrysnfqs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yonumen.top/gtynvkzmeq.html

C#:   x is int or double or decimal
来源：http://hz.wangdashe.top/gtgazvnrjr.html

[B14] 判断值是否在集合内
来源：http://hz.xylfe.cn/gtoeffgows.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tanke756.top/gtolnpwrlo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgfzy.top/gtpwucqaiu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtxtrwptjw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinghuilouyu.cn/gtezankmhb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxuanxn.top/gtbmitbnpt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ppjwa.cn/gtoqkbjvyd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.redwolf501.top/gtijztbxbt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yanxiufei.cn/gttucqbydl.html

[B15] 布尔运算与取反
来源：http://hz.jqgufenzy.top/gtjjmtsufp.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gttzomszfi.html

PHP:  $a && $b || !$c
来源：http://hz.gogol.net.cn/gtnrviufmi.html

JS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtougmcacv.html

TS:   a && b || !c
来源：http://hz.chenzaomai.com/gtugaujsgy.html

Java: a && b || !c
来源：http://hz.mhx1999.top/gthxmbzxus.html

Go:   a && b || !c
来源：http://hz.jqgufenzy.top/gtreuaswzg.html

Ruby: a && b || !c
来源：http://hz.andypj.xyz/gtqepsgocv.html

C#:   a && b || !c
来源：http://hz.kuanghao11.cn/gtfjbucegk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhixingplan.top/gtamdsvouu.html

Py:   if not data: return
来源：http://hz.aibaodan.cn/gtwpicpxkp.html

PHP:  if (!$data) { return; }
来源：http://hz.sweek.top/gtuadnyqnm.html

JS:   if (!data) return;
来源：http://hz.52xcode.cn/gtbsuvlivm.html

TS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtfppgjdlo.html

Java: if (data == null) return;
来源：http://hz.ehwqpu.com/gtvklhyfhy.html

Go:   if data == nil { return }
来源：http://hz.cqqwz.cn/gtytmmuwdb.html

Ruby: return if data.nil?
来源：http://hz.zhaomingkeji.xyz/gtvsxneicx.html

C#:   if (data == null) return;
来源：http://hz.dianchejie.cn/gtjsutrbcr.html

================================================================================
来源：http://hz.ppjwa.cn/gtinhfuxir.html

C. 函数与作用域
来源：http://hz.cdnleiting.top/gtpqbjttwy.html

================================================================================
来源：http://hz.yuanzhike.top/gtatzlbvuf.html

[C01] 定义函数
来源：http://hz.havefunace.top/gtfhbyfcos.html

Py:   def add(a, b): return a + b
来源：http://hz.shuidangran.top/gtispaikmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtxavvrefe.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenlongwang.top/gtyhmvpeiq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gtumebemlt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtkatkwhbl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nwbrower.top/gtpxmlgjdp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.redwolf501.top/gtrfjccuru.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtrgfdcxxr.html

[C02] 默认参数
来源：http://hz.kuanghao11.cn/gtewxkvxob.html

Py:   def greet(name="World"): return name
来源：http://hz.yueranfly.top/gtihiixywf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.0kj1m.cn/gtmsirkgnx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.mhx1999.top/gtjummehlw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuanzx.com/gtuktrslsh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sysykeji.top/gtxdauvcbe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pycfn.com/gttbjpjlmm.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtsdmqoqzw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenlongwang.top/gtflsozyer.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtnooogklj.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtaesceary.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhixingplan.top/gtgicbgnus.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sysykeji.top/gtpsfqkvcf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtgzgaexcs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sysykeji.top/gthegcooez.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.birdmap.top/gtubeybqax.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jqgfzy.top/gtjarruhmy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.smart0.xyz/gtgdzpadjx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.0kj1m.cn/gtpxnsmobo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daxiang520.top/gtklonhiky.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258888.top/gtxmnhprwt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtnpsmesfm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xylfe.cn/gtqgswysrb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtnfciiugk.html

Go:   // 无：用配置结构体参数
来源：http://hz.jqgfzy.top/gtachpjgdi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtvmjtcxpo.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gtfcbkniah.html

[C05] 返回多个值
来源：http://hz.xinyue.icu/gtzzuvqfis.html

Py:   return a, b
来源：http://hz.ppjwa.cn/gtqsjectnz.html

PHP:  return [$a, $b];
来源：http://hz.smart0.xyz/gtbuzkimjb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.meibo888.top/gtarsedgil.html

TS:   return { a, b };
来源：http://hz.xuanzx.com/gteeafydno.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cdnleiting.top/gtscbabhoy.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtpajnbjti.html

Ruby: return a, b
来源：http://hz.kuanghao11.cn/gtcshjasmq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pycfn.com/gtltfwrxsh.html

[C06] 匿名函数 / lambda
来源：http://hz.bjfxy.top/gtengknguw.html

Py:   square = lambda x: x * x
来源：http://hz.xinyue.icu/gtpmxuknsq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.aibaodan.cn/gtvrnqljes.html

JS:   const square = x => x * x;
来源：http://hz.zhongyouzk.top/gtbpvuxbcl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shzxlz.cn/gtgkkbmipe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hongshengwenyu.top/gthxdzxwzw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shzxlz.cn/gtllffyrba.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtqlgcihig.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zycfv.cn/gtljpvpwgk.html

[C07] 把函数作为参数传入
来源：http://hz.jqgfzy.top/gtypsvbxbk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xylfe.cn/gtiitjpjnc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xylfe.cn/gtqlsvgcdm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.iojbl.cn/gtxljriznb.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gtmvvtumra.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.havefunace.top/gtlmkbzmrg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.0kj1m.cn/gtdqvhqbmy.html

Ruby: arr.map(&:upcase)
来源：http://hz.316326.xyz/gtvzxaoqcs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuxming.cn/gtqevpmrqh.html

[C08] 闭包
来源：http://hz.gaohongyu789.top/gtpruinwck.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuanzhike.top/gtaypwcocy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenlongwang.top/gtwdnmwcvx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtbgrkwitq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtizyzqwct.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.52xcode.cn/gtwnlymppd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.redwolf501.top/gtnpmdizjg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.bjfxy.top/gtpfekfitk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtagwstuip.html

[C09] 递归
来源：http://hz.havefunace.top/gtvjzebjzs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigufen.top/gtyrfrpeko.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.wangshuangyany.cn/gtqqfbhnml.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtannheevu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtawbbqxlp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenzaomai.com/gtzghllrzw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigfzy.top/gtkhmzgtew.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gtrqkuirts.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sysykeji.top/gthdmbcdbo.html

[C10] 变量作用域
来源：http://hz.jlsjyb.cn/gtomnezuib.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhijiandao.cn/gtnuxbckbk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gogol.net.cn/gtglfrbkry.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jlsjyb.cn/gtfzsqbadq.html

TS:   同 JS
来源：http://hz.fzhhl.top/gtzuqbnays.html

Java: 方法内为块级作用域
来源：http://hz.jianghu66.top/gtwwotvbpm.html

Go:   花括号块级作用域
来源：http://hz.feifeiyinyue.top/gteooykdxr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hongshengwenyu.top/gtxkohnkcl.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gtjlzcqaum.html

[C11] 模块导入与导出
来源：http://hz.fzhhl.top/gtkrwgzolo.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtvtbmnodq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sufxvd.cn/gtrioymyit.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tianlin.xyz/gtmwqgqooh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhengqikj.top/gtjgfptxml.html

Java: import java.util.List;
来源：http://hz.jinghuilouyu.cn/gtcwbehnmi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtskgnlwdr.html


<!-- 参考信息 -->