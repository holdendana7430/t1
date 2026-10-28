代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tanke756.top/gtevthoidw.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtrjyaxbmj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gtruaqyovb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydjk.org.cn/gtxgsfybwu.html

[D15] 去重
来源：http://hz.dashuyun.cn/gtoannrkuu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtmigltwmm.html

PHP:  array_unique($arr);
来源：http://hz.mhx1999.top/gtfrrxaaoq.html

JS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtdiuxaqfi.html

TS:   [...new Set(arr)]
来源：http://hz.hysaishi.cn/gteqlzccsb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gtowzyqovf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgufenzy.top/gtdfvagtqs.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtorpudzyq.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtfobndjvz.html

[D16] 求和与平均值
来源：http://hz.quarkkingdee.top/gtzaticpji.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yangfankeji.com/gtfuhnkcig.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cqqwz.cn/gtpurgqfjt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gttybdbszy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gtqckhbvox.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhengqikj.top/gtoqbfynul.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtduyrgnsr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gthxfbddni.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtgcuirsqi.html

[D17] 最大值与最小值
来源：http://hz.dashuyun.cn/gtqwlpqnrn.html

Py:   max(arr);  min(arr)
来源：http://hz.jianghu66.top/gtbusadcab.html

PHP:  max($arr);  min($arr);
来源：http://hz.yangfankeji.com/gtlwbkxqsd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhixingplan.top/gtepalzywh.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtjoaqgkvg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tian-w.cn/gtyynsjzet.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gthesasrdt.html

Ruby: arr.max;  arr.min
来源：http://hz.shuidangran.top/gtqkvjqizq.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtgnlqlhok.html

[D18] 扁平化嵌套数组
来源：http://hz.aibaodan.cn/gtrmbfdjoh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtqoabcooi.html

PHP:  array_merge(...$nested);
来源：http://hz.xuetiantiany.cn/gteocpweln.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.aibaodan.cn/gtimzvbzdi.html

TS:   nested.flat();
来源：http://hz.yueranfly.top/gtkjnlqlki.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ivvv.top/gthxjauaun.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtifpseqfg.html

Ruby: nested.flatten
来源：http://hz.shangyingyoupin.top/gtmzugnhob.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.svipenyu.cn/gtpcgqrueq.html

[D19] 按字段分组
来源：http://hz.hywenlv.cn/gtwsmyqnxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuxming.cn/gtmbnpepxk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.mhx1999.top/gtvluiugrt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zdqjudy.top/gtknsbslfq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtevozoebu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtpftcmfbz.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gtctbbelrr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ywan-chungtsiang.top/gtfbdwgtqs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtcltpsrww.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258.top/gtlxaluudx.html

Py:   Counter(arr)
来源：http://hz.yj202588.top/gtbuqmvsrs.html

PHP:  array_count_values($arr);
来源：http://hz.jlsjyb.cn/gtepgnludm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtymwmhdnp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtetqqhrsw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.haohaochexian.top/gtfioyilrc.html

Go:   // 手写 map[T]int
来源：http://hz.zhixingplan.top/gtckqunawu.html

Ruby: arr.tally
来源：http://hz.pycfn.com/gtwqntkenl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhoulong.xyz/gtwnmaeozs.html

[D21] 判断是否包含某元素
来源：http://hz.sweek.top/gtpskzsioo.html

Py:   x in arr
来源：http://hz.gotoacloud.top/gtyhwtxgze.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dianchejie.cn/gtbvqlduds.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gthnvlbmzy.html

TS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gtwwgdrosu.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtalwysmfz.html

Go:   slices.Contains(arr, x)
来源：http://hz.jyoumei.cn/gtvbrbcwxg.html

Ruby: arr.include?(x)
来源：http://hz.haohaochexian.top/gtmvbwcvxj.html

C#:   list.Contains(x)
来源：http://hz.zdqjudy.top/gtyvtsogne.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gttkjeveby.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuxming.cn/gtvndymquv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.havefunace.top/gttzzaxxzu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhijiandao.cn/gtpelxedod.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtsbjlyonm.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gtfdtibxkd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aibaodan.cn/gttoyobtxh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtjhftyoqq.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtpjouukgm.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtkjriaxzh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gtyggyadcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtxwhcugiu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtcdqbpert.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtqqjtauug.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangdashe.top/gtoplzuuiy.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gtlkdsxhii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ehwqpu.com/gtyzvprbxu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtuiytumgn.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuxming.cn/gtszjclouq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgufenzy.top/gtzbkmjoda.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.birdmap.top/gtahijuwde.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shuidangran.top/gtlmopahdg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gtvjcbrmyq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.birdmap.top/gthbhxiauv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtwmkdoxdj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.havefunace.top/gtpmomrayp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gttjgigfpm.html

[D25] Set 集合去重与交并差
来源：http://hz.vqdsnc.cn/gttlhvbvho.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinyuanbaomall.cn/gtllxgvafd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cdnleiting.top/gtcglpxmxx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtxsxqtybu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gtdoemxcwe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yonumen.top/gtbgrhjnlw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gtvxnzncux.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.iojbl.cn/gtbqtuctiw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pycfn.com/gtglucdlhv.html

[D26] 数组转字符串
来源：http://hz.xziqi.cn/gtvqjhprkn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sufxvd.cn/gtvpveywba.html

PHP:  implode(", ", $arr);
来源：http://hz.iojbl.cn/gtwcwbtfwq.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtnqyznzhk.html

TS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtchkvzcxf.html

Java: String.join(", ", list)
来源：http://hz.fengsongda.top/gtrblyejoy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tanke756.top/gtfbwozfkm.html

Ruby: arr.join(", ")
来源：http://hz.ivvv.top/gtgbbhikcn.html

C#:   string.Join(", ", list)
来源：http://hz.fzhhl.top/gtodlfpwfy.html

================================================================================
来源：http://hz.cucudq.cn/gtsahqowdq.html

E. 字符串处理
来源：http://hz.shangyingyoupin.top/gtlksgqrzk.html

================================================================================
来源：http://hz.jinqigufen.top/gtcxpncxgj.html

[E01] 拼接字符串
来源：http://hz.ehwqpu.com/gtwnowsouc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gtfiwyejnr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.andypj.xyz/gtulwyobvs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.redwolf501.top/gtvfaqrqwh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtgfxddhlt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigufen.top/gtygjicnrk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cheryme.top/gtmyaqiazn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ivvv.top/gtvlmszsvs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cashguo.top/gtthgsemve.html

[E02] 重复字符串
来源：http://hz.shanyushiyangkeji.top/gtsukddvdb.html

Py:   "ab" * 3
来源：http://hz.fzhhl.top/gtnhvkribx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pengpengdd.cyou/gtcwusuphh.html

JS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtxxwuzhmb.html

TS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtscsdwlpw.html

Java: "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtnbirvobs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.guannengcc.top/gtorenwiqu.html

Ruby: "ab" * 3
来源：http://hz.daria6918.cn/gtxarpwutv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gzhubu.top/gtqzrebaqe.html

[E03] 截取子串
来源：http://hz.shuidangran.top/gtwfntlqwo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtodarxtuy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jyoumei.cn/gthpkhjirq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sufxvd.cn/gterluwsdu.html

TS:   s.slice(1, 4)
来源：http://hz.zhongyouzk.top/gttmuueblf.html

Java: s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gttrjmvqvx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.bjfxy.top/gtwwsllmwt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinghuilouyu.cn/gtaqidpssc.html

C#:   s.Substring(1, 3)
来源：http://hz.wangdashe.top/gtwjvvzhov.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gtidikamts.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sxryk.cn/gtourbrmmc.html

PHP:  strpos($s, "x");
来源：http://hz.yongpay.top/gtewwlcott.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtchvzrith.html

TS:   s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtmyzeloku.html

Java: s.indexOf("x")
来源：http://hz.guannengcc.top/gtshlsqvmj.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gtmmewbqwk.html

Ruby: s.index("x")
来源：http://hz.chenlongwang.top/gtsnoejecp.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtjxzfhqyk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gotoacloud.top/gtqbdgcanu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258888.top/gtdiaxlpqf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cheryme.top/gtuiihveqy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtuwxsisfv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zycfv.cn/gtfkglpqum.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtllrywzwf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tianlin.xyz/gttrdbihur.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.mhx1999.top/gtqxvdibjo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuanzhike.top/gtqjwhfoyn.html

[E06] 替换子串
来源：http://hz.nanxuanxn.top/gtrwurpeqt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shzxlz.cn/gtlfyclrsv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtzapdliew.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtidnnuhur.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtvzpkptfb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtocwaxbdq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtdgmmocrm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jianghu66.top/gtuwbgmnpc.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtzxeclipr.html

[E07] 按分隔符拆分
来源：http://hz.feifeiyinyue.top/gtqmgfjlbx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yanxiufei.cn/gtrowhcmlu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gtbxvvkztu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jqgufenzy.top/gtdbfnzfww.html

TS:   s.split(",")
来源：http://hz.yueranfly.top/gttmpxutsk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenlongwang.top/gtqwhvjlmg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.haohaochexian.top/gtklvcvtvn.html

Ruby: s.split(",");  s.split
来源：http://hz.daria6918.cn/gtqefilkhq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jlsjyb.cn/gtuxzpenti.html

[E08] 数组按分隔符合并
来源：http://hz.quarkkingdee.top/gthbbjyqul.html

Py:   ",".join(items)
来源：http://hz.zhijiandao.cn/gtmeytzqdb.html

PHP:  implode(",", $items);
来源：http://hz.hywenlv.cn/gtusgjzwaa.html

JS:   items.join(",")
来源：http://hz.cqqwz.cn/gtfiyibvdy.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtakhmrgpr.html

Java: String.join(",", items)
来源：http://hz.guowangkeji.top/gtfwgllbuo.html

Go:   strings.Join(items, ",")
来源：http://hz.zhijiandao.cn/gtxbdeznot.html

Ruby: items.join(",")
来源：http://hz.pengpengdd.cyou/gtcjpdctgw.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gtsaqyvxwn.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtoszuvpgl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtwvrpxilx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hammf.cn/gtyeptyojn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtvfzqwehh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.vqdsnc.cn/gtxkbabjuo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtcosaprix.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.vqdsnc.cn/gtsrehukkn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gtqnedjvhu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sufxvd.cn/gtvjwvjolk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangtech.top/gtmutesnqq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.meibo888.top/gtpmgpwpko.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenjidiqi.icu/gtecaquged.html

JS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gttheiplfx.html

TS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtqwxrjvcp.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtqcuzisqo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tianlin.xyz/gtoicnwnxd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtnmqyequd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.316326.xyz/gtdbjxfeyx.html

[E11] 反转字符串
来源：http://hz.52xcode.cn/gttzdjaadc.html

Py:   s[::-1]
来源：http://hz.xziqi.cn/gtukjfgcss.html

PHP:  strrev($s);
来源：http://hz.zycfv.cn/gtqltxkrhj.html

JS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtmojlkged.html

TS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtqpyjajlx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sufxvd.cn/gttecdtcvz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sweek.top/gtzjyuyvgw.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtfxwiliio.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtiiqnookc.html

[E12] 统计某字符出现次数
来源：http://hz.yangfankeji.com/gtczoqqien.html

Py:   s.count("a")
来源：http://hz.hfpthk.cn/gttrwqtgbb.html

PHP:  substr_count($s, "a");
来源：http://hz.jyoumei.cn/gtevjuhhew.html

JS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtfqglsgud.html

TS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gteudckrkm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtmrxxfmyo.html

Go:   strings.Count(s, "a")
来源：http://hz.zhixingplan.top/gtwlwbykhg.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtldtwgjjp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.c1oappe.top/gtupirleec.html

[E13] 逐字符遍历
来源：http://hz.jyoumei.cn/gtmnfokxza.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtlsaepdkq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xylfe.cn/gtijpgdtli.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gthfkycbxr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtamhslzsn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yanxiufei.cn/gtyweyzpsb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xylfe.cn/gtnwpqvjjh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hammf.cn/gtpzgnifaf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtjgblbopv.html

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtwbmryfom.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgfzy.top/gtcgywicmh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtmkgzyick.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtogrellny.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dianchejie.cn/gtdzgmyqua.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtvuagnwja.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ywan-chungtsiang.top/gtmzaycufi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gtpcvnmsbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtulbjzwql.html

[E15] HTML 转义 / 反转义
来源：http://hz.yangfankeji.com/gthecbbjhv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnqzz.top/gtpalbjytu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sxryk.cn/gtcoacbspn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuxming.cn/gtvflrcuqz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jiagoushi.top/gtyfsaganm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sweek.top/gtgvosltzo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guannengcc.top/gtbopcohrn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jlsjyb.cn/gtgukracij.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtdhtlynic.html

[E16] 数字千分位
来源：http://hz.wangshuangyany.cn/gtseybfruw.html

Py:   f"{1234567:,}"
来源：http://hz.snrcjt.cn/gtcrtnrykg.html

PHP:  number_format(1234567);
来源：http://hz.jinqigufen.top/gtnctbtjkw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.9152youxi.cn/gthkqisheh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtkfwcpwsw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtsvindifr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yangfankeji.com/gtxugekbpe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.c1oappe.top/gtgdmkmkvh.html

C#:   1234567.ToString("N0")
来源：http://hz.shzxlz.cn/gttuparyxu.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtpltsfgoo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tianlin.xyz/gtnxjipshu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nwbrower.top/gtmxgozuac.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtmwniypoz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gturudxxxc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yueranfly.top/gtqsymeyeu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cheryme.top/gtfococfpu.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtoxethyua.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hfpthk.cn/gtgxfpxnbg.html

[E18] 模板占位符替换
来源：http://hz.fzhhl.top/gtxmdqyhev.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuetiantiany.cn/gtsfvtefiz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yongpay.top/gtmrcytkij.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtfpiixuze.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtxptterpp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gtmcyatexa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pycfn.com/gtfagzyfst.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtbmrcphak.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cqqwz.cn/gtsyjyevuj.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtaqordnid.html

Py:   s.splitlines()
来源：http://hz.hfpthk.cn/gtrcokxpme.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtgcnybqoz.html

JS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtyxltsnsd.html

TS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtktcsppnb.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtamezlnfd.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtvnkdafiy.html

Ruby: s.lines
来源：http://hz.shuidangran.top/gtesucyjpn.html

C#:   s.Split('\n')
来源：http://hz.jinqigufen.top/gtkrxdmavm.html

[E20] 判断字符串是否为空
来源：http://hz.9152youxi.cn/gtystpxztx.html

Py:   if not s:
来源：http://hz.ehwqpu.com/gtkhxaxlvo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nwbrower.top/gtzuwhpmfn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtijwhxrri.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtbpebldhj.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gthkvqpgav.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gthzqjjbpm.html

Ruby: if s.empty?
来源：http://hz.daria6918.cn/gtgnhuimsu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pycfn.com/gtwdanoygt.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gturheyyqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtrfzzxxix.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gtnacfvdqi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtquhlvvjz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtlvrfivsm.html


<!-- 参考信息 -->