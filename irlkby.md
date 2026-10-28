代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://hz.snrcjt.cn/gtyqtcyiby.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.fzhhl.top/gtwyanxnuw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhijiandao.cn/gtqjprpyfl.html

[A25] 字符串比较
来源：http://hz.chenjidiqi.icu/gtowpnmuom.html

Py:   s1 == s2; s1 != s2
来源：http://hz.mhx1999.top/gtxmxyxrvm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.mhx1999.top/gtayrpftem.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yonumen.top/gtvbasbceg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.haohaochexian.top/gtdkszgold.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.feifeiyinyue.top/gtgzttneyl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.andypj.xyz/gtmyrycurh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.haohaochexian.top/gtkfvhdkxt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.sysykeji.top/gtimayyunn.html

[A26] 类型转换总览
来源：http://hz.hammf.cn/gtopoblxad.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.aizwys.cn/gtsyjxmfnd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jinqigfzy.top/gtsxuctgzz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yvedp.cn/gtmvoqbiub.html

TS:   Number() String() Boolean() x as number
来源：http://hz.chenlongwang.top/gtyysfnzit.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cucudq.cn/gthwlbbrfe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.shangyingyoupin.top/gtnquckpkx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.birdmap.top/gtaqtxrtbv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.tian-w.cn/gtcnbampdl.html

================================================================================
来源：http://hz.yuxming.cn/gthayfciur.html

B. 流程控制
来源：http://hz.zhaomingkeji.xyz/gtuqsryizz.html

================================================================================
来源：http://hz.zhengqikj.top/gtmpxrsava.html

[B01] 条件判断 if / else
来源：http://hz.aibaodan.cn/gtxwkonvcy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hfpthk.cn/gtgddlzitw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.chenlongwang.top/gtcwarxeos.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtifpsbhpq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtyoznzwsu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.quarkkingdee.top/gtdvofnoqt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.sysykeji.top/gtwtuynfds.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cqqwz.cn/gtrcmlwmbl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.quarkkingdee.top/gtmvlfpniw.html

[B02] 多分支 else if / elif
来源：http://hz.ehwqpu.com/gtfqrepern.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gaohongyu789.top/gtvechakdv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.wangdashe.top/gtrqgsmndi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtkvaeaokw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtkqhhfrhf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.mhx1999.top/gtolpgutis.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shzxlz.cn/gtqeyexxhz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.shuidangran.top/gtegmclwrl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gttffhxwdu.html

[B03] switch / match / case
来源：http://hz.jinghuilouyu.cn/gtmwylduck.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fengsongda.top/gtxipuycba.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.guowangkeji.top/gtstdowurs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhengqikj.top/gtdbszrzoi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.havefunace.top/gtlzhcmcuw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhoulong.xyz/gtginusqfg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jiagoushi.top/gtabkohdjq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jianghu66.top/gtrvreqgff.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhengqikj.top/gtvocywxlb.html

[B04] for 计数循环
来源：http://hz.yuanzhike.top/gtcmimknmg.html

Py:   for i in range(10): print(i)
来源：http://hz.jlsjyb.cn/gtvbnupvvo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhoulong.xyz/gttfolcqlv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.mhx1999.top/gtkanalgsz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cheryme.top/gtqvcongqf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shuidangran.top/gttgcphozw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.quarkkingdee.top/gteihngzzz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daria6918.cn/gtuvjlilne.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.wangshuangyany.cn/gtfferiszh.html

[B05] 遍历数组 / 列表
来源：http://hz.52xcode.cn/gtiypknnbe.html

Py:   for item in arr: print(item)
来源：http://hz.haohaochexian.top/gtkxzgoczk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cdnleiting.top/gtvznvisgh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.fengsongda.top/gtryexclbs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zdqjudy.top/gtauiggapm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhixingplan.top/gtknojxfgp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.wangdashe.top/gtzxarujhp.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ivvv.top/gtdciflveo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xylfe.cn/gtbawxhsyt.html

[B06] 遍历字典 / 对象
来源：http://hz.gzhubu.top/gtswdkyayq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.52xcode.cn/gtvxrnpddw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shzxlz.cn/gtwiybvltl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gthhztsxmj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aizwys.cn/gtowifwmin.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yonumen.top/gtwovbgnmp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinghuilouyu.cn/gtlzylcxri.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jqgufenzy.top/gtmvpcqyid.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.wangshuangyany.cn/gtsbxfqnkj.html

[B07] while 循环
来源：http://hz.sysykeji.top/gtckvgxmtq.html

Py:   while i < 10: i += 1
来源：http://hz.yuxming.cn/gtabcfntbc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yvedp.cn/gtddsywsns.html

JS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtvsjfmwhw.html

TS:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtrqgkxhgx.html

Java: while (i < 10) { i++; }
来源：http://hz.zhengqikj.top/gtxquzqyjr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ywan-chungtsiang.top/gtldffsrdo.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinqigufen.top/gtlinqujkz.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtqhtnqxzv.html

[B08] do-while（至少执行一次）
来源：http://hz.xingfuxueyuan.xyz/gtevoeqjjn.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gttlbbnclm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yongpay.top/gtaaegsdhe.html

JS:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtcftivwbt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhixingplan.top/gtuiuvosyf.html

Java: do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtnnvonawg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.feifeiyinyue.top/gtygkuxloq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cqqwz.cn/gtkfvpowrp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtdlsyyiah.html

[B09] break 与 continue
来源：http://hz.xziqi.cn/gtjzwchnun.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.mhx1999.top/gtoyvpmfuy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.iojbl.cn/gtrluswcee.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gttlbfnblg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtajnxzlwg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtxsseqgnr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.quarkkingdee.top/gtoezzdyuj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tian-w.cn/gtunbycocs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtmpuoghfg.html

[B10] 遍历同时拿索引
来源：http://hz.quarkkingdee.top/gtsdfnwjrs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj20258888.top/gtapnrsinp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yuxming.cn/gtnjlwflrx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.c1oappe.top/gtrxijuapu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtasjqdcby.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sufxvd.cn/gthgazzbmx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jqgfzy.top/gturznuwji.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.smart0.xyz/gtgzsmdcnd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gaohongyu789.top/gtaowrvfwf.html

[B11] 生成数字序列 / 区间
来源：http://hz.aibaodan.cn/gtfjiuosmg.html

Py:   list(range(0, 10, 2))
来源：http://hz.0kj1m.cn/gtbjsinwnj.html

PHP:  range(0, 10, 2);
来源：http://hz.cdnleiting.top/gtsmvrqiqc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangkeji.top/gtwueggiou.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hfpthk.cn/gtgzodtsdr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ivvv.top/gttnvrpkmi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigfzy.top/gtrtfudxwp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangtech.top/gtvsifwhwn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.0kj1m.cn/gthpjrgzha.html

[B12] 跳出多层循环
来源：http://hz.smart0.xyz/gtmighkmwq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sweek.top/gtcvvvldoq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuxming.cn/gtejtponhr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtrzvnfppg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtxderqfqz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtyfgkzuxa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.andypj.xyz/gtmqffqaot.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.meibo888.top/gtvtbtacyd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydjk.org.cn/gtuyevfryx.html

[B13] 判断是否为数字
来源：http://hz.fzhhl.top/gtxhgvcojh.html

Py:   isinstance(x, (int, float))
来源：http://hz.tianlin.xyz/gtsavcrobl.html

PHP:  is_numeric($x)
来源：http://hz.xuanzx.com/gtrsheejiw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtzqpzovod.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtsuqhqtpj.html

Java: x instanceof Number
来源：http://hz.zhengqikj.top/gtdpljzxhc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sysykeji.top/gtagpssuet.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nwbrower.top/gtqmqmnoct.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtcwwamnsl.html

[B14] 判断值是否在集合内
来源：http://hz.yanxiufei.cn/gtzliyiiia.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuxming.cn/gtxlzeafft.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yangfankeji.com/gttylnhooi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtpyhyzgyw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zycfv.cn/gtzxwzoncr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sufxvd.cn/gtlgbhgqkf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yongpay.top/gtvlbjrfxz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yangfankeji.com/gtyhcnaqfr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenlongwang.top/gtjpotfmqp.html

[B15] 布尔运算与取反
来源：http://hz.cheryme.top/gtkvaperqe.html

Py:   a and b or not c
来源：http://hz.ppjwa.cn/gtaadhfdrj.html

PHP:  $a && $b || !$c
来源：http://hz.ydjk.org.cn/gtwbgmmlhy.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtfuetvsnh.html

TS:   a && b || !c
来源：http://hz.xylfe.cn/gtmynmqjol.html

Java: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtdaumeohe.html

Go:   a && b || !c
来源：http://hz.snrcjt.cn/gtmrklrjwn.html

Ruby: a && b || !c
来源：http://hz.yj20258888.top/gthjrafjay.html

C#:   a && b || !c
来源：http://hz.sufxvd.cn/gtudbfggid.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj20258888.top/gthnahvhjg.html

Py:   if not data: return
来源：http://hz.iojbl.cn/gtgijqjhvx.html

PHP:  if (!$data) { return; }
来源：http://hz.fengsongda.top/gtxcbjgzgi.html

JS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtnfamalra.html

TS:   if (!data) return;
来源：http://hz.sufxvd.cn/gtujrgtglm.html

Java: if (data == null) return;
来源：http://hz.gaohongyu789.top/gtzogefxvs.html

Go:   if data == nil { return }
来源：http://hz.zhoulong.xyz/gtdbgqndxl.html

Ruby: return if data.nil?
来源：http://hz.feifeiyinyue.top/gtmioyaudw.html

C#:   if (data == null) return;
来源：http://hz.xinyue.icu/gtrgskjvzx.html

================================================================================
来源：http://hz.jiagoushi.top/gthulqtwyq.html

C. 函数与作用域
来源：http://hz.xuanzx.com/gttookwojt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthkhgktut.html

[C01] 定义函数
来源：http://hz.sysykeji.top/gtjmtzldwr.html

Py:   def add(a, b): return a + b
来源：http://hz.jyoumei.cn/gthqvzedbg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gteqdsucwj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtplxnjmqy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gthngellac.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtqfcomeuc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jyoumei.cn/gtfltjhxyu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangdashe.top/gtjknhnjej.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtlfgugyos.html

[C02] 默认参数
来源：http://hz.jqgfzy.top/gtmzaefsjl.html

Py:   def greet(name="World"): return name
来源：http://hz.yueranfly.top/gtpozjbowf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gotoacloud.top/gtyjanqjqv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgufenzy.top/gteplwelbd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sweek.top/gtbjtvjpwb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhaomingkeji.xyz/gtwtxteqtj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj20258888.top/gtmiwjfhao.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gthnktkmbq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.smart0.xyz/gtfljxqjcm.html

[C03] 可变参数
来源：http://hz.meibo888.top/gtfgnpaqcw.html

Py:   def total(*args): return sum(args)
来源：http://hz.haohaochexian.top/gtyuewbafs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtcjqmblda.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jyoumei.cn/gtrdnwsdpz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtymbfggve.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenjidiqi.icu/gtqvchhjqy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.smart0.xyz/gtimbayxfi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.quarkkingdee.top/gtffslqsry.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinyuanbaomall.cn/gtilnqwban.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtkhunkvgc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cashguo.top/gtvtsbtnun.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dianchejie.cn/gtmwsnuebk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtbyroxgvf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258.top/gtjxlwdxhd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangkeji.top/gtlrftdcoc.html

Go:   // 无：用配置结构体参数
来源：http://hz.jianghu66.top/gtnmrumumw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtvtzrkxst.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtsdezhqqq.html

[C05] 返回多个值
来源：http://hz.jinyuanbaomall.cn/gtdqciaxea.html

Py:   return a, b
来源：http://hz.hysaishi.cn/gtzziqktlw.html

PHP:  return [$a, $b];
来源：http://hz.zhoulong.xyz/gthabahgkc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guowangkeji.top/gtauotgpdx.html

TS:   return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtcygqwogd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtldlteqdl.html

Go:   return a, b
来源：http://hz.daria6918.cn/gtivimpjzc.html

Ruby: return a, b
来源：http://hz.zhengqikj.top/gtxudvdnrx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shangyingyoupin.top/gtcaldpwje.html

[C06] 匿名函数 / lambda
来源：http://hz.zdqjudy.top/gtyyinqjsi.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gthinzbyon.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zdqjudy.top/gtauxplwgy.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtixsalnpz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yonumen.top/gtiacyofgr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tanke756.top/gtuqcddvxx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgfzy.top/gtlapbzjbs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.vqdsnc.cn/gtpmsywlhx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuanzhike.top/gtsxctxpqa.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtmidgamec.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nwbrower.top/gtxnurylcf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hammf.cn/gttwqfqewq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hongshengwenyu.top/gtsnewcdzq.html

TS:   arr.map(String)
来源：http://hz.dianchejie.cn/gtjzeczaws.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydzc1.top/gtpzfljxpk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hongshengwenyu.top/gtcrshsoou.html

Ruby: arr.map(&:upcase)
来源：http://hz.shangyingyoupin.top/gtmveoytcb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.birdmap.top/gtoaqdwqjz.html

[C08] 闭包
来源：http://hz.hongshengwenyu.top/gtemqsyvck.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cdnleiting.top/gtletzxyvq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgfzy.top/gtnwwyrmfh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtwaukmsqj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtrmtzqsqh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gtlremnsnx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cheryme.top/gtgzmjltlv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shangyingyoupin.top/gtkfwacnnk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtvbqpshac.html

[C09] 递归
来源：http://hz.yuxming.cn/gtlsftwrhn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtvcjcoqpd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pengpengdd.cyou/gttphiaygw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtiupusnla.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtqqrxkyis.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.quarkkingdee.top/gtveuokweu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.birdmap.top/gtqrmjsziy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gtlbrdnbvx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnxiangtu.top/gtxvxgoizw.html

[C10] 变量作用域
来源：http://hz.shanyushiyangtech.top/gtbxwvjaux.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cqqwz.cn/gtmutguxyl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yvedp.cn/gtgzhpuucu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuanzhike.top/gtlzygdbpx.html

TS:   同 JS
来源：http://hz.jqgfzy.top/gtestrfrmh.html

Java: 方法内为块级作用域
来源：http://hz.wangdashe.top/gthcmtoiaz.html

Go:   花括号块级作用域
来源：http://hz.daxiang520.top/gtkcvmjqsq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pycfn.com/gtgwlzpnif.html

C#:   块级作用域
来源：http://hz.mhx1999.top/gtomtamstg.html

[C11] 模块导入与导出
来源：http://hz.feifeiyinyue.top/gtsjxehqua.html

Py:   from module import func
来源：http://hz.yonumen.top/gtllhfocxu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jyoumei.cn/gtukxvzfmx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenzaomai.com/gtyezsryyb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zycfv.cn/gtwnnieigo.html

Java: import java.util.List;
来源：http://hz.ehwqpu.com/gtlcmjtgpq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tanke756.top/gtyursmouc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gtqthaeavi.html

C#:   using System.Text;
来源：http://hz.hongshengwenyu.top/gttgbddmec.html

[C12] 立即执行函数 IIFE
来源：http://hz.cheryme.top/gtuwhoymkd.html

Py:   (lambda: print("run"))()
来源：http://hz.wangdashe.top/gtzksyxntm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangkeji.top/gtppgdppks.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtoxjntdqn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtfajsgxrb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nwbrower.top/gtxvlekccp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.52xcode.cn/gttsagczuw.html

Ruby: -> { puts "run" }.call
来源：http://hz.daxiang520.top/gtjeiflemq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shzxlz.cn/gthjoyypqz.html

[C13] 类型声明 / 类型注解
来源：http://hz.hongshengwenyu.top/gthatbyipg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.svipenyu.cn/gtuzkmrpnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtqrzauqor.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.havefunace.top/gtdkrwhyfm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtihlnwbgc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtsresafwq.html

Go:   func add(a, b int) int
来源：http://hz.ywan-chungtsiang.top/gtzlcskgvk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.bjfxy.top/gtjljboqob.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.haohaochexian.top/gtctiqqjno.html

[C14] 泛型函数
来源：http://hz.xuanzx.com/gtfxsjktip.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtwinumsod.html

PHP:  // 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtwpmmggmn.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtmpjcebbd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtkopkgico.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gtlkfxsecb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhengqikj.top/gtgelwofzg.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtchiuxqag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yanxiufei.cn/gtzmrpyexp.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtkbyntsaw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sufxvd.cn/gtwzzpsdlt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nwbrower.top/gtctpknkwy.html


<!-- 参考信息 -->