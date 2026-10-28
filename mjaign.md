代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sweek.top/gttvyznlhz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtvsbszeac.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dashuyun.cn/gtpkktndhl.html

Go:   // 手写循环累加
来源：http://hz.yanxiufei.cn/gtbpbgrqfx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yueranfly.top/gtagtqtdsn.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gtcsljnnis.html

[D17] 最大值与最小值
来源：http://hz.yj202588.top/gtcamweezr.html

Py:   max(arr);  min(arr)
来源：http://hz.jianghu66.top/gtladxhvnq.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gtsnbnbkge.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gtymtdyxhs.html

TS:   Math.max(...arr);
来源：http://hz.jqgfzy.top/gtqpvlzopn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtfedqkcfm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yongpay.top/gtvjeworjx.html

Ruby: arr.max;  arr.min
来源：http://hz.zhoulong.xyz/gtorioidrz.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gtweoddjfl.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtolhbuymr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sysykeji.top/gtkfcitijm.html

PHP:  array_merge(...$nested);
来源：http://hz.tanke756.top/gtwjlpwsqt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jianghu66.top/gtekkipiay.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gtqvfnbtcp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtaeiuxuos.html

Go:   // 手写双层循环
来源：http://hz.yj202588.top/gtvpqkgqtf.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtpeukpwoe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ppjwa.cn/gtbfofinvi.html

[D19] 按字段分组
来源：http://hz.hywenlv.cn/gtrrtwtjjj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.316326.xyz/gtbpfqafxm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xziqi.cn/gtdtvaeabd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtcfzrnaya.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shangyingyoupin.top/gtxgjzrdvi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuanzx.com/gtiwulwdsu.html

Go:   // 手写 map[string][]T
来源：http://hz.fzhhl.top/gtqgesderh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenlongwang.top/gtossrstxj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtuyshyldq.html

[D20] 统计每个元素出现次数
来源：http://hz.jinqigufen.top/gtvudewuku.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtlffkxeog.html

PHP:  array_count_values($arr);
来源：http://hz.ehwqpu.com/gtosxqtwhc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtegwtrvyp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtcbtfwigg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtnngaynna.html

Go:   // 手写 map[T]int
来源：http://hz.aizwys.cn/gtxfmwuknk.html

Ruby: arr.tally
来源：http://hz.pycfn.com/gtxutgpvck.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.snrcjt.cn/gtlonulbml.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gtfrftyrir.html

Py:   x in arr
来源：http://hz.jinqigfzy.top/gtsnrmgqiy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangshuangyany.cn/gtsqfzjrac.html

JS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtykkyotss.html

TS:   arr.includes(x)
来源：http://hz.yvedp.cn/gtkaojhxqu.html

Java: list.contains(x)
来源：http://hz.redwolf501.top/gtuogucmny.html

Go:   slices.Contains(arr, x)
来源：http://hz.hysaishi.cn/gtlifpiaha.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtxnlablcp.html

C#:   list.Contains(x)
来源：http://hz.zhongyouzk.top/gttjzrepyq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gtvywahyll.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gtqpbejzqj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.0kj1m.cn/gtvhkscpdb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.haohaochexian.top/gtwzawawuw.html

TS:   [...arr];
来源：http://hz.yanxiufei.cn/gtzortxsnn.html

Java: new ArrayList<>(list);
来源：http://hz.jianghu66.top/gtfvulsqwx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jyoumei.cn/gtcuuapscy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.mhx1999.top/gtnqdevwjo.html

C#:   new List<int>(list);
来源：http://hz.feifeiyinyue.top/gteddygymu.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gttewcjxpi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gtuhmbhocp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtwwwqiwam.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtpkiilpzx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtpwrmiszf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtljkwduvz.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtummimstu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gtautamemp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hongshengwenyu.top/gtbejtjyql.html

[D24] 字典 / Map 基本操作
来源：http://hz.pycfn.com/gtupapiqrj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydzc1.top/gtskniedxp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtcgudqanu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgufenzy.top/gtmpudbucj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gtyyfrhvww.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gtrtvbpjbm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gtvvkykwjb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jlsjyb.cn/gtzhmajjor.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhixingplan.top/gtxyrtfusv.html

[D25] Set 集合去重与交并差
来源：http://hz.gogol.net.cn/gtafdzudzd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgufenzy.top/gtjjndpqmr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinghuilouyu.cn/gtfycmdxtx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.316326.xyz/gthrbsapzf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jianghu66.top/gtafiqqmen.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhoulong.xyz/gtkwdgwsxn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuanzx.com/gtemhecaab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gtwkyqazxy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cqqwz.cn/gtivwaymqz.html

[D26] 数组转字符串
来源：http://hz.chenzaomai.com/gtsiitcvdt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sxryk.cn/gtddljhbta.html

PHP:  implode(", ", $arr);
来源：http://hz.sysykeji.top/gtnlqlhrzw.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtahewmryv.html

TS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtkupieokc.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtbzkhnvnr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.feifeiyinyue.top/gtcnimjujf.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gteijepbdd.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtgsgfokmg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtllwbiivv.html

E. 字符串处理
来源：http://hz.fzhhl.top/gtxxnmngen.html

================================================================================
来源：http://hz.tianlin.xyz/gttwgmtslj.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtafmkozqc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtwvkppmrb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangshuangyany.cn/gtsnzxgede.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtibnlwyfg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtkgtbhzgx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cdnleiting.top/gtfoctaqac.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.redwolf501.top/gtrefmnidz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gzhubu.top/gtwfsiezyd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.redwolf501.top/gtsgsprzyk.html

[E02] 重复字符串
来源：http://hz.xuetiantiany.cn/gteaqhmdzu.html

Py:   "ab" * 3
来源：http://hz.jlsjyb.cn/gtjjxxghzm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtaxuglnrp.html

JS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gthdqoqepj.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtawqftzrb.html

Java: "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtbtzngvqv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jiagoushi.top/gteyhmevhh.html

Ruby: "ab" * 3
来源：http://hz.sweek.top/gtpmvdhimd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jlsjyb.cn/gtknyferae.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtoyrkxpfn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.bjfxy.top/gtrcjjotsl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yonumen.top/gtpwwzsfue.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.havefunace.top/gtahzxeteu.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtazoilfww.html

Java: s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtcmosjhkc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gzhubu.top/gttdlfveeb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.smart0.xyz/gteovdsfby.html

C#:   s.Substring(1, 3)
来源：http://hz.shzxlz.cn/gtrsessdvv.html

[E04] 查找子串位置
来源：http://hz.cucudq.cn/gttzqjubjp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtttoneyat.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtlihdmpyj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.dashuyun.cn/gtrhsetcie.html

TS:   s.indexOf("x")
来源：http://hz.yvedp.cn/gtjzwllyaw.html

Java: s.indexOf("x")
来源：http://hz.sxryk.cn/gtckdqxdel.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtclqpxqlf.html

Ruby: s.index("x")
来源：http://hz.shangyingyoupin.top/gtjchfikzi.html

C#:   s.IndexOf("x")
来源：http://hz.quarkkingdee.top/gtnlhrcllj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtfwxgjpgs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnxiangtu.top/gtzmwohnmw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinghuilouyu.cn/gtrywwlcqv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gttkbfwley.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtjfcvokbm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtbohngdoc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cucudq.cn/gtyvxlkqvz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.iojbl.cn/gtcopjyysa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhengqikj.top/gtrwinalzc.html

[E06] 替换子串
来源：http://hz.yonumen.top/gtpdkkyhzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtyjdilyhn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinghuilouyu.cn/gttegtsisq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtkqnjlqny.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtfktubfpg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtvbfjnebc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xylfe.cn/gtaazqifxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.feifeiyinyue.top/gtwftlswkp.html

C#:   s.Replace("a", "b")
来源：http://hz.shangyingyoupin.top/gtttgiddzm.html

[E07] 按分隔符拆分
来源：http://hz.redwolf501.top/gtziogigbp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.haohaochexian.top/gtoixxdvoz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dianchejie.cn/gtfmrrnhzs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtswggxxry.html

TS:   s.split(",")
来源：http://hz.yj202588.top/gtpqiyfofd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhiwuduotai.top/gtkzsqljhb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhengqikj.top/gtzukdpiep.html

Ruby: s.split(",");  s.split
来源：http://hz.guannengcc.top/gtwcafgnjx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangdashe.top/gtvwplzeid.html

[E08] 数组按分隔符合并
来源：http://hz.daxiang520.top/gtokswxuvh.html

Py:   ",".join(items)
来源：http://hz.aibaodan.cn/gtrfxzorme.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtzwjdlptw.html

JS:   items.join(",")
来源：http://hz.zhixingplan.top/gtpjfozxrn.html

TS:   items.join(",")
来源：http://hz.yj202588.top/gtuekpdihp.html

Java: String.join(",", items)
来源：http://hz.svipenyu.cn/gtkgukqwxx.html

Go:   strings.Join(items, ",")
来源：http://hz.yj202588.top/gtmlcuufni.html

Ruby: items.join(",")
来源：http://hz.svipenyu.cn/gtkaxcsncy.html

C#:   string.Join(",", items)
来源：http://hz.iojbl.cn/gtdclgrwqt.html

[E09] 去除所有空白字符
来源：http://hz.hammf.cn/gtcmigziag.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yvedp.cn/gtwktttufs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gogol.net.cn/gtgyhbydzy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtwwdglauy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtwygqodlx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangtech.top/gtgdahtxjz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cqqwz.cn/gtllaackyj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shzxlz.cn/gtxcietruv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yueranfly.top/gtpekzzbyb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtqcicyffx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yongpay.top/gtccopvjbf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xinyue.icu/gtysweuqgs.html

JS:   "7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtpdxaaawn.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtosahfwzv.html

Java: String.format("%03d", 7)
来源：http://hz.nanxinkj.top/gtqojncyhy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtnzqkpmxl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtgoqcmfvs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tanke756.top/gtbvdgxqou.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gtzxrqtiiw.html

Py:   s[::-1]
来源：http://hz.cashguo.top/gthowloetl.html

PHP:  strrev($s);
来源：http://hz.hnxiangtu.top/gtyonkoijk.html

JS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtqpytcmgc.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtihknthha.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.haohaochexian.top/gtuqnaebnf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydzc1.top/gteragoqix.html

Ruby: s.reverse
来源：http://hz.xziqi.cn/gtcuhqiuvl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtyhgadgiy.html

[E12] 统计某字符出现次数
来源：http://hz.feifeiyinyue.top/gtvlowjtul.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtydcgubfb.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gtjwesrfws.html

JS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtyiofynkf.html

TS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtnbreamjn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gtwtcffdco.html

Go:   strings.Count(s, "a")
来源：http://hz.xziqi.cn/gtsabdocyw.html

Ruby: s.count("a")
来源：http://hz.sufxvd.cn/gtfjwrcnmm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ehwqpu.com/gtsomnddlc.html

[E13] 逐字符遍历
来源：http://hz.aizwys.cn/gtptwjnsii.html

Py:   for ch in s: print(ch)
来源：http://hz.ehwqpu.com/gtgjcbuofh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258.top/gtxhufajqw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtgpaxyjad.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtduffuykh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtjkqzncvw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.birdmap.top/gtdvepjiqk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dianchejie.cn/gtvvoaivgl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhaomingkeji.xyz/gtiuctegro.html

[E14] URL 编码与 Base64
来源：http://hz.gaohongyu789.top/gtivpxpjkz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yonumen.top/gtrafhaowv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtjhfetwjx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jiagoushi.top/gtkdrmgtxg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tian-w.cn/gtfsawpzyt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinyuanbaomall.cn/gtowgwwgpe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydzc1.top/gtlrslxgnv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtxjbzwbso.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xylfe.cn/gtpnrvzllb.html

[E15] HTML 转义 / 反转义
来源：http://hz.ehwqpu.com/gtfkhnrrin.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.vqdsnc.cn/gtvihjusyl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tanke756.top/gtmvwakhfp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtvsmmjsws.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gogol.net.cn/gtkifbgchx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuanzhike.top/gtfkjmqzqd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangtech.top/gtenommluz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jianghu66.top/gtfpdcdssg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xingfuxueyuan.xyz/gtvhughdij.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtyaeoodho.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtvlybhvbu.html

PHP:  number_format(1234567);
来源：http://hz.zhijiandao.cn/gtnocpwiyu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtnxycdnzb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtjnqvzbuc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sysykeji.top/gtvfqqcmbt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zycfv.cn/gtoqduisfz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gthipetzfr.html

C#:   1234567.ToString("N0")
来源：http://hz.jiagoushi.top/gtcjbqyxbf.html

[E17] 首字母大写
来源：http://hz.shangyingyoupin.top/gtbeswxtll.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj202588.top/gtlxykwzrk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sufxvd.cn/gtuspxfcsz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtnxgnqmyj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtuwzchaby.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cucudq.cn/gtdluqkjbv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cheryme.top/gtjmwbrxxo.html

Ruby: s.capitalize
来源：http://hz.yuanzhike.top/gturvrqgwc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pengpengdd.cyou/gtcnbmeaee.html

[E18] 模板占位符替换
来源：http://hz.ybcxt.top/gtvfhzlqmu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhengqikj.top/gtmloafwje.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hongshengwenyu.top/gtkrqarjqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtnwlurmyg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gteumdtkdq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xinyue.icu/gtcxrcyjyo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tanke756.top/gtyfmghupy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtizipceil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxinkj.top/gtummmwyki.html

[E19] 多行文本按行拆分
来源：http://hz.jinqigfzy.top/gtpnvzliuo.html

Py:   s.splitlines()
来源：http://hz.chenjidiqi.icu/gtajumynnr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnxiangtu.top/gtuujfswrf.html

JS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtmloxsqxv.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtdasckxnf.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtyfjqvkvm.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtxltgotil.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtarqberjy.html

C#:   s.Split('\n')
来源：http://hz.jlsjyb.cn/gtwfqbvbgp.html

[E20] 判断字符串是否为空
来源：http://hz.52xcode.cn/gtewgbwqug.html

Py:   if not s:
来源：http://hz.ywan-chungtsiang.top/gtroogqrzn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtoikvpowo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhixingplan.top/gtjiohjlxg.html

TS:   if (s === "") {}
来源：http://hz.52xcode.cn/gtzprqldfk.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtdolobyvc.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtrjoacolr.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtturvjjmr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xingfuxueyuan.xyz/gttbojeocq.html

[E21] 超长截断加省略号
来源：http://hz.dianchejie.cn/gtmnwwwhki.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtenbujubn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gthrkpxdap.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtnrrhrpmt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtjjqrtmqh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtbmdkwlhh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtxheyofdc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cqqwz.cn/gtbbkdsuim.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtcxocwjpd.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtxvupuvjl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj202588.top/gttgcwggak.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtojbadjsd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtzaaiyxgw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtufrtzxxd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtijayhywu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtbcinszus.html

Ruby: s.bytesize;  s.length
来源：http://hz.tian-w.cn/gterzpyoun.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuanzhike.top/gtuzjsjtlb.html

================================================================================
来源：http://hz.hysaishi.cn/gtjhboyeoo.html

F. 文件与目录
来源：http://hz.cdnleiting.top/gtweryzlog.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxnlpotta.html


<!-- 参考信息 -->