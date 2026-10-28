代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zhengqikj.top/gtprxfiekl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.bjfxy.top/gtqvajrdwx.html

TS:   // Node.js：readline 模块
来源：http://hz.tianlin.xyz/gtxorctkwb.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.gzhubu.top/gtgnaqchvm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.haohaochexian.top/gtpmescmoa.html

Ruby: gets.chomp
来源：http://hz.fzhhl.top/gtvfcnvvdb.html

C#:   Console.ReadLine();
来源：http://hz.daria6918.cn/gtsscsdcar.html

[A21] 保留指定小数位输出
来源：http://hz.dianchejie.cn/gtyfamvqhc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jinyuanbaomall.cn/gtrkhjuawm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jlsjyb.cn/gtdciflxli.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yuanzhike.top/gtzrxetgkb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ydzc1.top/gthdnknxhb.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gtakwvacec.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.havefunace.top/gtxoblaefc.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shanyushiyangkeji.top/gtuswoomoh.html

C#:   3.14159.ToString("F2")
来源：http://hz.sxryk.cn/gtvpjilitk.html

[A22] 获取字符串长度
来源：http://hz.smart0.xyz/gtliukqnek.html

Py:   len(s)
来源：http://hz.yonumen.top/gtskvetxif.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yj202588.top/gtkkefibad.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.sweek.top/gtosswizdq.html

TS:   s.length
来源：http://hz.dianchejie.cn/gtrmpxzfgb.html

Java: s.length()
来源：http://hz.chenzaomai.com/gthgkbiofn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yueranfly.top/gtxtkjnbyl.html

Ruby: s.length
来源：http://hz.yuxming.cn/gtjjecquei.html

C#:   s.Length
来源：http://hz.nanxuanxn.top/gtjrhaobpq.html

[A23] 大小写转换
来源：http://hz.hnqzz.top/gtigmjwqyn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ydjk.org.cn/gtkinjrnir.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhiwuduotai.top/gtckkmlfvb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.iojbl.cn/gtwbqtsbto.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xziqi.cn/gtjdrugrry.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ehwqpu.com/gtazdjbgsx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.guannengcc.top/gtdlobrdbv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hnqzz.top/gtcolyabcz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.vqdsnc.cn/gttiwstpto.html

[A24] 去除首尾空白
来源：http://hz.snrcjt.cn/gtoamzawrb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ybcxt.top/gtmjtuokzw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yuanzhike.top/gtydfjmcra.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhoulong.xyz/gtocplnrsg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.daxiang520.top/gtbmaphnva.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.vqdsnc.cn/gtmopaevqx.html

Go:   strings.TrimSpace(s)
来源：http://hz.xziqi.cn/gtpxiyvjzz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hysaishi.cn/gtfvgcqkhx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jyoumei.cn/gthjigoccs.html

[A25] 字符串比较
来源：http://hz.wangshuangyany.cn/gtybvtjnlg.html

Py:   s1 == s2; s1 != s2
来源：http://hz.redwolf501.top/gtoxwqfxli.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cqqwz.cn/gtumjohrdq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinyuanbaomall.cn/gtsgbaeyiu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jlsjyb.cn/gtbwyppxfe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.pycfn.com/gtomiiyyfh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.daria6918.cn/gtbcjfhonu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.fengsongda.top/gthzmbqodn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.aizwys.cn/gtcketcwbx.html

[A26] 类型转换总览
来源：http://hz.ppjwa.cn/gtkkdsshdo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zdqjudy.top/gtdzwfnwii.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.snrcjt.cn/gtacqzyptn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jyoumei.cn/gtdpkxogim.html

TS:   Number() String() Boolean() x as number
来源：http://hz.birdmap.top/gtbfcihcoy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hysaishi.cn/gthdefnuau.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.kuanghao11.cn/gtmxdazhvd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sufxvd.cn/gtfjafsdyb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shuidangran.top/gthkbdwqmi.html

================================================================================
来源：http://hz.xuanzx.com/gtowepvjos.html

B. 流程控制
来源：http://hz.xylfe.cn/gtxucbutmu.html

================================================================================
来源：http://hz.ppjwa.cn/gtirpkpbrc.html

[B01] 条件判断 if / else
来源：http://hz.pengpengdd.cyou/gtedthyhgt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jiagoushi.top/gtfyydafek.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.9152youxi.cn/gtykazmnax.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtlzsvmdtz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yvedp.cn/gtcpdubwee.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yueranfly.top/gtkljqdlak.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.snrcjt.cn/gtfqbbwgtb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.quarkkingdee.top/gtzsarxeni.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtzmkeqyvo.html

[B02] 多分支 else if / elif
来源：http://hz.havefunace.top/gtrncrmnvl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jqgufenzy.top/gtluecxsaf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yueranfly.top/gtydmleywh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.fzhhl.top/gtgnertmkh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtvezpkxpo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtaktnkoqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.meibo888.top/gtknyiiycc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yuxming.cn/gtsduvbcdv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtsswyzzon.html

[B03] switch / match / case
来源：http://hz.yuanzhike.top/gtbxfiyokn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.52xcode.cn/gtkvhiswjz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.iojbl.cn/gtuvymsmuw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jyoumei.cn/gtguiqyfko.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtjpyzouxw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.mhx1999.top/gtjhsdzxcr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.guannengcc.top/gtsrvyrilx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yuanzhike.top/gtcfuhoncj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.birdmap.top/gttesvultu.html

[B04] for 计数循环
来源：http://hz.wangshuangyany.cn/gtocpchibn.html

Py:   for i in range(10): print(i)
来源：http://hz.zhoulong.xyz/gthqpomefp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.mhx1999.top/gtuckxcvzb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yvedp.cn/gtgrchvoix.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sysykeji.top/gtgxayrjaj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yanxiufei.cn/gtypmobvnk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tian-w.cn/gtwkkjhary.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ivvv.top/gtiqzmgakp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jqgufenzy.top/gteskgjdrm.html

[B05] 遍历数组 / 列表
来源：http://hz.jinqigufen.top/gtxjxqwttj.html

Py:   for item in arr: print(item)
来源：http://hz.xylfe.cn/gtwaubeeam.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.svipenyu.cn/gtrubhwfia.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xylfe.cn/gtztwkutow.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenlongwang.top/gttjuuyfpu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.guowangkeji.top/gttiyinbvz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hywenlv.cn/gtpmlhctul.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yangfankeji.com/gtalthzlpj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.316326.xyz/gtkpmcozjq.html

[B06] 遍历字典 / 对象
来源：http://hz.gogol.net.cn/gtmvcmvqdd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.kuanghao11.cn/gtsgwnzhli.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.fzhhl.top/gtmcdgrofk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yvedp.cn/gtmovpuije.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sweek.top/gtarjuptcp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtkmakheca.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.meibo888.top/gtqvcrxbci.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.svipenyu.cn/gtddsoplmj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.vqdsnc.cn/gtakpgyrzn.html

[B07] while 循环
来源：http://hz.fengsongda.top/gtzmsgpaiw.html

Py:   while i < 10: i += 1
来源：http://hz.aizwys.cn/gtoanledwo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.316326.xyz/gtxcibduvd.html

JS:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtafvboted.html

TS:   while (i < 10) { i++; }
来源：http://hz.nwbrower.top/gtdspjqyro.html

Java: while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtveyxhjkj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hnxiangtu.top/gtzwpxrvmg.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hammf.cn/gtyfdumzdx.html

C#:   while (i < 10) { i++; }
来源：http://hz.52xcode.cn/gtraxzwdjo.html

[B08] do-while（至少执行一次）
来源：http://hz.chenjidiqi.icu/gtdpnzbfyt.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cqqwz.cn/gttqmmrqnn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hongshengwenyu.top/gtdqgnzhfx.html

JS:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtcyktebys.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtsucqakts.html

Java: do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtouiaopmx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.chenlongwang.top/gtnevphrvh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pycfn.com/gtgncmeldt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtqqraqyey.html

[B09] break 与 continue
来源：http://hz.gzhubu.top/gtfbmhaenj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tianlin.xyz/gtbzpnkyqs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.dashuyun.cn/gtnvehjrkb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtmfjssolu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtvvmihojl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtskpgzlvr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenzaomai.com/gtvteyjbmn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yangfankeji.com/gtiqkkbrxi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zycfv.cn/gttohzeaso.html

[B10] 遍历同时拿索引
来源：http://hz.tian-w.cn/gtrcqszmmy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hysaishi.cn/gtbwxzlurk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.smart0.xyz/gtekwzzyfp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ppjwa.cn/gtuflmltyh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.iojbl.cn/gtnriwadbo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtopbncrke.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aizwys.cn/gtfylztxya.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangshuangyany.cn/gtpvfrmfbl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinghuilouyu.cn/gtubppajwv.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj202588.top/gtnjtklsmi.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj202588.top/gtolsomfsl.html

PHP:  range(0, 10, 2);
来源：http://hz.zdqjudy.top/gtdxxfoyvi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gttafarzud.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtrrujyogk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.svipenyu.cn/gtkdxnymcy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yangfankeji.com/gtxdkhopel.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhiwuduotai.top/gtoksthamu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj20258.top/gtienzlkdg.html

[B12] 跳出多层循环
来源：http://hz.cdnleiting.top/gtdorhuqec.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jlsjyb.cn/gtnoowmqzm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shanyushiyangkeji.top/gtzrwdojvw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtuicwzjil.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtpsknjdaj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.havefunace.top/gtxpdsvcbx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258.top/gtqpweqhay.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yanxiufei.cn/gtjyzufyev.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhixingplan.top/gtxelwrczn.html

[B13] 判断是否为数字
来源：http://hz.redwolf501.top/gtgdvspmbf.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigufen.top/gtjayammzl.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gthgnoxruy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gtlvpryrkq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fengsongda.top/gtwsuxcuvj.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtzeidmzqm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.mhx1999.top/gtxmfsqcje.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gtqtcipfll.html

C#:   x is int or double or decimal
来源：http://hz.jqgufenzy.top/gtjiurtyym.html

[B14] 判断值是否在集合内
来源：http://hz.52xcode.cn/gtnyfofoxw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sysykeji.top/gtmgnakcrh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gzhubu.top/gtzjivoqat.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtqtqgnich.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtqhfewdsq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtticmnmti.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhongyouzk.top/gtkyypkqwt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangtech.top/gtlrungggq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aizwys.cn/gtnmjkukdm.html

[B15] 布尔运算与取反
来源：http://hz.daria6918.cn/gtcxpgykbg.html

Py:   a and b or not c
来源：http://hz.dianchejie.cn/gtymjqqfpb.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gtchjxbzil.html

JS:   a && b || !c
来源：http://hz.jyoumei.cn/gthiwbwbuw.html

TS:   a && b || !c
来源：http://hz.hammf.cn/gteeddzwuk.html

Java: a && b || !c
来源：http://hz.guannengcc.top/gttlpgnjaq.html

Go:   a && b || !c
来源：http://hz.yj20258.top/gthrewgrvw.html

Ruby: a && b || !c
来源：http://hz.316326.xyz/gtqpszoyrp.html

C#:   a && b || !c
来源：http://hz.jianghu66.top/gtgdveyycu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.smart0.xyz/gtzqvempeh.html

Py:   if not data: return
来源：http://hz.iojbl.cn/gtmbbcfnix.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gthxmxqujl.html

JS:   if (!data) return;
来源：http://hz.smart0.xyz/gtaiwttzae.html

TS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtorbirlrx.html

Java: if (data == null) return;
来源：http://hz.tian-w.cn/gtrviuhlqz.html

Go:   if data == nil { return }
来源：http://hz.fzhhl.top/gtxevtxrwm.html

Ruby: return if data.nil?
来源：http://hz.ydjk.org.cn/gtvdhlscak.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtntsqsmoz.html

================================================================================
来源：http://hz.wangdashe.top/gtqdpkhnhx.html

C. 函数与作用域
来源：http://hz.snrcjt.cn/gtgeogzilb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvoduwiqz.html

[C01] 定义函数
来源：http://hz.52xcode.cn/gthdvcsrnn.html

Py:   def add(a, b): return a + b
来源：http://hz.shangyingyoupin.top/gtepywsdfc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtqmiadfkp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtrjozycdf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtemjpaqte.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gtvysvpywy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gttmuqzusg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yangfankeji.com/gthumtlosa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtsvskqaqm.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtqsyadxyi.html

Py:   def greet(name="World"): return name
来源：http://hz.hysaishi.cn/gtqqfdmwwb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxuanxn.top/gtacktbnpv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtfvfnlunr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gtnoioekdo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ywan-chungtsiang.top/gtbiaoxysf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.feifeiyinyue.top/gtortotlyr.html

Ruby: def greet(name = "World") = name
来源：http://hz.yangfankeji.com/gtsbwlghfd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtwehrbqoe.html

[C03] 可变参数
来源：http://hz.jinghuilouyu.cn/gtkswbqpks.html

Py:   def total(*args): return sum(args)
来源：http://hz.hnxiangtu.top/gtjlbwangn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fzhhl.top/gtjjkwvhdc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtnykaqrrs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sysykeji.top/gtpqrfsrau.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fzhhl.top/gtuyyozenk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuetiantiany.cn/gtkgeqmuea.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ywan-chungtsiang.top/gthekvmkyh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gtzqsltmgi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sufxvd.cn/gtmgevuazd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj20258888.top/gthpmlhtye.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.feifeiyinyue.top/gtfcllecik.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.haohaochexian.top/gtnnemfylt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhijiandao.cn/gtynkhiybp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xylfe.cn/gtlrrkzura.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinghuilouyu.cn/gtmwrrksyf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtprcyfmjh.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtdtqpjdtg.html

[C05] 返回多个值
来源：http://hz.sweek.top/gtuzfxjlsq.html

Py:   return a, b
来源：http://hz.ydzc1.top/gtwncjnfcr.html

PHP:  return [$a, $b];
来源：http://hz.yueranfly.top/gtrnpjuwhb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtcojbvztq.html

TS:   return { a, b };
来源：http://hz.snrcjt.cn/gtfxauxgth.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuxming.cn/gtyhcvsvxu.html

Go:   return a, b
来源：http://hz.gaohongyu789.top/gtpzjuytdl.html

Ruby: return a, b
来源：http://hz.yuxming.cn/gthauxiajm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtgobpgcho.html

[C06] 匿名函数 / lambda
来源：http://hz.vqdsnc.cn/gtpmjkxozn.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigfzy.top/gtfqwbffxj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangkeji.top/gtekahlyta.html

JS:   const square = x => x * x;
来源：http://hz.tian-w.cn/gtkcodoalh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenjidiqi.icu/gtzukccvht.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yuanzhike.top/gtnjyorrdd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinyuanbaomall.cn/gtrivcbrqf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xingfuxueyuan.xyz/gtmqfvyxpk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.guowangkeji.top/gtxpvbqiyz.html

[C07] 把函数作为参数传入
来源：http://hz.birdmap.top/gtvujklrjs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ybcxt.top/gtixmjjczn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinqigufen.top/gthpogqoao.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dianchejie.cn/gtjfvltfuq.html

TS:   arr.map(String)
来源：http://hz.sweek.top/gtkrobttzr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnqzz.top/gtjpkjtqre.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangshuangyany.cn/gttdsgaghu.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gtavpquqso.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigufen.top/gtiolerzuo.html

[C08] 闭包
来源：http://hz.ydjk.org.cn/gttcpacmfr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.0kj1m.cn/gtzwdbuonh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.smart0.xyz/gtvxlyegha.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gthrsuycpb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtjengxdwc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.andypj.xyz/gtoectoqpv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sufxvd.cn/gtrvucamfv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zdqjudy.top/gtndtcgunh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtpsdhirux.html

[C09] 递归
来源：http://hz.yj20258.top/gtluodgmtt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtmsagnjga.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj20258.top/gtbmquuuav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.quarkkingdee.top/gtqrboilvk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gtmohkusum.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.kuanghao11.cn/gtmajcuade.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gtfxgrpkba.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xinyue.icu/gtjnuwihmi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangshuangyany.cn/gtznqvrtbq.html

[C10] 变量作用域
来源：http://hz.fzhhl.top/gtztrwuikr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sxryk.cn/gtrwycginl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnxiangtu.top/gtpksjdvvs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258888.top/gtvxmnmqov.html

TS:   同 JS
来源：http://hz.tanke756.top/gtcwfifckj.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtrrtmrqrj.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtcesysmpq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgufenzy.top/gteumfhlvs.html


<!-- 参考信息 -->