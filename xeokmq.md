代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenlongwang.top/gttsudgfcc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gtklkwehqf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gzhubu.top/gtqeszycuh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gteoxwtudb.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtbznzizcl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.smart0.xyz/gtmmnwtwoo.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtwekcfomd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxinkj.top/gtirjmvpfl.html

TS:   [...arr].reverse();
来源：http://hz.wangshuangyany.cn/gtctsmhrgf.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gtmvgnecir.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gtsfvmjybs.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtxoxboptp.html

C#:   list.Reverse();
来源：http://hz.9152youxi.cn/gtcpsjutaz.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtrvnqpodb.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhaomingkeji.xyz/gtqzkyekjx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yongpay.top/gtgmqbxhki.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtvheylfjk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtuqgblohn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhiwuduotai.top/gtfkliymlp.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gttpogmbul.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtzbainwyg.html

C#:   list.IndexOf(x);
来源：http://hz.zdqjudy.top/gtrhcuvoqq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cheryme.top/gtdmptbnsf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtazapjqdt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258.top/gtxogcfutr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtkifyarnd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hammf.cn/gtxecoekyr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ehwqpu.com/gtxsemvwkm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gzhubu.top/gtlrnbkhvr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gthahznvwu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtvgiqhdjr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangshuangyany.cn/gtviraluqo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuanzx.com/gtbapavtdl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.kuanghao11.cn/gtdeqnssrd.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtequoljwo.html

TS:   arr.map(x => x * 2)
来源：http://hz.tian-w.cn/gtpzrtsxxy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydzc1.top/gtqhqozbmb.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtyrochiss.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtqiedtqca.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fzhhl.top/gtziywybvy.html

[D15] 去重
来源：http://hz.tian-w.cn/gtjwipiuvc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtldvnfkjj.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtapcfibss.html

JS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtujzzyruu.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtbdtckzsj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sxryk.cn/gtewuxafpz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtrcbtytgu.html

Ruby: arr.uniq
来源：http://hz.svipenyu.cn/gtwgvdtzne.html

C#:   list.Distinct().ToList()
来源：http://hz.yuxming.cn/gtqjhcdnji.html

[D16] 求和与平均值
来源：http://hz.sxryk.cn/gtwwwslwig.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtlxeljcgy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.vqdsnc.cn/gtapvapzkv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtcbscyepf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtowwwqsrj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgfzy.top/gtswcmfbuw.html

Go:   // 手写循环累加
来源：http://hz.hfpthk.cn/gtoereslxi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.c1oappe.top/gtoudngbcr.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtwrvbkmij.html

[D17] 最大值与最小值
来源：http://hz.xingfuxueyuan.xyz/gtwcxukksz.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gtjjbyuexm.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gtxxkisbug.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtjntsrvjo.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtcsicitgq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.52xcode.cn/gtjidyxmwl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtfmjbutvc.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gtboqvjnbr.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtjwpxlppf.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtnlqunmrd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgfzy.top/gtldcnzdce.html

PHP:  array_merge(...$nested);
来源：http://hz.kuanghao11.cn/gtgcpsmppn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jyoumei.cn/gtsmpmmoyp.html

TS:   nested.flat();
来源：http://hz.wangshuangyany.cn/gthszegtsk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.9152youxi.cn/gtzqbhjuko.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gtejtwadhj.html

Ruby: nested.flatten
来源：http://hz.zycfv.cn/gtgmcnrbkz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhiwuduotai.top/gtzxytneyg.html

[D19] 按字段分组
来源：http://hz.xziqi.cn/gtvftizkah.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnxiangtu.top/gtghluqjfe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ivvv.top/gtxscyokcq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenjidiqi.icu/gtsliotizb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aizwys.cn/gtlemkwgle.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shangyingyoupin.top/gtvqjydgdt.html

Go:   // 手写 map[string][]T
来源：http://hz.dianchejie.cn/gtroarkhuz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fengsongda.top/gtyyvoezga.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tanke756.top/gtgrwcjmyt.html

[D20] 统计每个元素出现次数
来源：http://hz.daxiang520.top/gtahgchtbh.html

Py:   Counter(arr)
来源：http://hz.bjfxy.top/gtmmorjbgz.html

PHP:  array_count_values($arr);
来源：http://hz.jiagoushi.top/gtcjsrtolr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtagtaicki.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtywjcbqgb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gtcfczeesu.html

Go:   // 手写 map[T]int
来源：http://hz.havefunace.top/gtcgzjpmfv.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtycccuiro.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.iojbl.cn/gtdownmzpv.html

[D21] 判断是否包含某元素
来源：http://hz.chenzaomai.com/gtsucfuoxt.html

Py:   x in arr
来源：http://hz.pycfn.com/gtrsearzcq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aizwys.cn/gtzrkwuwsu.html

JS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtmlvxakdw.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtsctrtpxx.html

Java: list.contains(x)
来源：http://hz.hongshengwenyu.top/gtyyryuofq.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gtdbeekpxc.html

Ruby: arr.include?(x)
来源：http://hz.ywan-chungtsiang.top/gtwfthvstv.html

C#:   list.Contains(x)
来源：http://hz.xuanzx.com/gthkzdkjei.html

[D22] 复制数组（避免共享引用）
来源：http://hz.0kj1m.cn/gtyptxhzuf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dianchejie.cn/gtmjdjftss.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ivvv.top/gtrqpwdlmt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cdnleiting.top/gtbtyqgrur.html

TS:   [...arr];
来源：http://hz.jlsjyb.cn/gtdmvzifdt.html

Java: new ArrayList<>(list);
来源：http://hz.wangshuangyany.cn/gtuueuauvf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.fzhhl.top/gtujvveknl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.quarkkingdee.top/gtijfgwqbf.html

C#:   new List<int>(list);
来源：http://hz.gotoacloud.top/gtaybhldjv.html

[D23] reduce 累积计算
来源：http://hz.chenzaomai.com/gtxwihlznu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guowangkeji.top/gtyfmtmayl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zycfv.cn/gtuklliiwv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtqgebrewu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtreukmaum.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhiwuduotai.top/gtrrtmmxau.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtnjbqnyor.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenzaomai.com/gtmohqvzka.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.feifeiyinyue.top/gtirgdyftp.html

[D24] 字典 / Map 基本操作
来源：http://hz.shuidangran.top/gthzbogpcy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtjmkeojfx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pycfn.com/gthojrqgfr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aizwys.cn/gtbpdynkdq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sxryk.cn/gtqwsxusbw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gtfcfvrjnw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.havefunace.top/gtofbbrjvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.c1oappe.top/gtxryssoyh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.havefunace.top/gtqjvbnekp.html

[D25] Set 集合去重与交并差
来源：http://hz.havefunace.top/gttdsbxlcx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigufen.top/gtpfgxhadj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yueranfly.top/gtpvxginmw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxinkj.top/gtsxkfzogl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.andypj.xyz/gtmpxcsxfl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gtcbdqbsqu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtyezpeejs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xziqi.cn/gtpuaqxyce.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgufenzy.top/gtkvyipexm.html

[D26] 数组转字符串
来源：http://hz.yueranfly.top/gtlqkewabm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.bjfxy.top/gtjupbpxjz.html

PHP:  implode(", ", $arr);
来源：http://hz.tianlin.xyz/gtwsrlpapy.html

JS:   arr.join(", ")
来源：http://hz.cucudq.cn/gtplglpffi.html

TS:   arr.join(", ")
来源：http://hz.sweek.top/gthhlwxpdu.html

Java: String.join(", ", list)
来源：http://hz.quarkkingdee.top/gtrrjvgevg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hongshengwenyu.top/gtziiyroji.html

Ruby: arr.join(", ")
来源：http://hz.yj202588.top/gtayyxyxgr.html

C#:   string.Join(", ", list)
来源：http://hz.hongshengwenyu.top/gtpghnhexv.html

================================================================================
来源：http://hz.yj20258888.top/gtweneaivm.html

E. 字符串处理
来源：http://hz.chenzaomai.com/gtywluqwkr.html

================================================================================
来源：http://hz.chenzaomai.com/gtnodqxykd.html

[E01] 拼接字符串
来源：http://hz.svipenyu.cn/gtmpxzhhxn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cucudq.cn/gttcejfvhr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtmbbxqacg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtgtesgxel.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtrmdjaong.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtwpjkppax.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yangfankeji.com/gtnputuyiv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydjk.org.cn/gtqdlvscfn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.haohaochexian.top/gttwoabrli.html

[E02] 重复字符串
来源：http://hz.yvedp.cn/gtstbnscjz.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gtyipqmbfy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.snrcjt.cn/gtyjmrxkhy.html

JS:   "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtvxvkrpuh.html

TS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtwkhwmhmd.html

Java: "ab".repeat(3)
来源：http://hz.pycfn.com/gtcheguucs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gthpvvzepp.html

Ruby: "ab" * 3
来源：http://hz.316326.xyz/gtdklccjhv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shzxlz.cn/gtmdzcecou.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtinrgadhk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhiwuduotai.top/gtbscitmyv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jlsjyb.cn/gtgqigiwqu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtalafvbdh.html

TS:   s.slice(1, 4)
来源：http://hz.jqgfzy.top/gtxugrfqvj.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtlzdqcbuw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.9152youxi.cn/gtrunursan.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.mhx1999.top/gtbkdhtbua.html

C#:   s.Substring(1, 3)
来源：http://hz.iojbl.cn/gtrojbbnuw.html

[E04] 查找子串位置
来源：http://hz.yuxming.cn/gtyhjxzqqg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.feifeiyinyue.top/gttknvsymq.html

PHP:  strpos($s, "x");
来源：http://hz.jinyuanbaomall.cn/gthkuiyhhz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtaqygeydj.html

TS:   s.indexOf("x")
来源：http://hz.mhx1999.top/gtjzwupzkk.html

Java: s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtisbwnizw.html

Go:   strings.Index(s, "x")
来源：http://hz.zhengqikj.top/gtynusjtxb.html

Ruby: s.index("x")
来源：http://hz.dashuyun.cn/gtxihjroaj.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gtzhpjiwtu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtaaqitwyj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shzxlz.cn/gtodgxgmtq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtdywqzxjm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtbdjgdxyu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gtzdkdrnzr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtjqytjpmx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhengqikj.top/gtwotcpxqi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tanke756.top/gtftpysaqo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtplnadkpb.html

[E06] 替换子串
来源：http://hz.hnqzz.top/gtkwixuchh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.mhx1999.top/gtmrmlftij.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xziqi.cn/gtfjlskslq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtdtjiwqko.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtxlxbogpp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtpazlxflw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtsivnzvhp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtkgfpuibp.html

C#:   s.Replace("a", "b")
来源：http://hz.gzhubu.top/gtdosqgdtc.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gttursqisq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gzhubu.top/gtpfxzwfph.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtuhmzsqco.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtujrwtbqp.html

TS:   s.split(",")
来源：http://hz.9152youxi.cn/gtfabagxyy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cheryme.top/gtecyzrssb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxinkj.top/gtbyqhxtzg.html

Ruby: s.split(",");  s.split
来源：http://hz.vqdsnc.cn/gtlwecxyif.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daria6918.cn/gtfxzyabub.html

[E08] 数组按分隔符合并
来源：http://hz.jinghuilouyu.cn/gtayqivakd.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangtech.top/gtdpqyfmem.html

PHP:  implode(",", $items);
来源：http://hz.hfpthk.cn/gtaillwkvs.html

JS:   items.join(",")
来源：http://hz.dashuyun.cn/gtyykiaayv.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtcvlhgmdu.html

Java: String.join(",", items)
来源：http://hz.nanxuanxn.top/gtbzstpgwh.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gtoutczhof.html

Ruby: items.join(",")
来源：http://hz.sweek.top/gtjznfvxyv.html

C#:   string.Join(",", items)
来源：http://hz.ydzc1.top/gtgwecigbk.html

[E09] 去除所有空白字符
来源：http://hz.aizwys.cn/gtrmdmyhwz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuxming.cn/gtkrxngzli.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtljevcjca.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtrhqkzuqb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtiitclous.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gttjnrdpug.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yvedp.cn/gtcaxemymo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.316326.xyz/gtvszqjrje.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtheptcamc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.snrcjt.cn/gtgorlipjb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jiagoushi.top/gtcyqjxukb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtdlmqnlhx.html

JS:   "7".padStart(3, "0")
来源：http://hz.jlsjyb.cn/gtygeftnpl.html

TS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtrpghfhjy.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigufen.top/gtczcnhafl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gtupuoedun.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.redwolf501.top/gtjktivrgz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gtdzapwnve.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtwnldcjix.html

Py:   s[::-1]
来源：http://hz.hywenlv.cn/gtnpjqnacq.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtwklncefm.html

JS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtkiggtdxf.html

TS:   [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtfvscfzpn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.quarkkingdee.top/gtzvnxmoxo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtfjdtvait.html

Ruby: s.reverse
来源：http://hz.hfpthk.cn/gtyuddjrjm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtqkkasvrg.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtkdiqevfw.html

Py:   s.count("a")
来源：http://hz.sufxvd.cn/gtzrwomlqi.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtyupobeud.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtrwuwdbsy.html

TS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtpsfqjbbl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gtashgufrf.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gtsqankmwn.html

Ruby: s.count("a")
来源：http://hz.hongshengwenyu.top/gtueckkjjp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.svipenyu.cn/gtjqzdttln.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtoijlqvjv.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gthqkqkgkn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.vqdsnc.cn/gtwdkggpzr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtxejyevjm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtatpkwlov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gthlelncve.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hfpthk.cn/gtouuzzuof.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtibnitals.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinghuilouyu.cn/gtafykrrhx.html

[E14] URL 编码与 Base64
来源：http://hz.zhixingplan.top/gtjmpbevle.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.feifeiyinyue.top/gtvhvtxtay.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.snrcjt.cn/gtoyndhkwr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuetiantiany.cn/gtdrggvfxf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtakyizvvr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tian-w.cn/gtcycxfxhz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sufxvd.cn/gtkjkykfuv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangkeji.top/gtvtsiezpl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangshuangyany.cn/gttfkwlhle.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtyoqmlqya.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtioicvzvz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtiwtybend.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtemxyuevq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtqabvgqkw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhijiandao.cn/gtodcleqny.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jyoumei.cn/gttidrpesi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenzaomai.com/gtyqugtdxr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shangyingyoupin.top/gtipxdiygc.html

[E16] 数字千分位
来源：http://hz.yueranfly.top/gtclyaajzz.html

Py:   f"{1234567:,}"
来源：http://hz.nwbrower.top/gthstydioi.html

PHP:  number_format(1234567);
来源：http://hz.jqgufenzy.top/gtosbjrghj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtorgzykxx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtswexasuf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydzc1.top/gtiqyjgrqj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.wangdashe.top/gttwnxhlgg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dianchejie.cn/gtcxslmebm.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtxltancqy.html

[E17] 首字母大写
来源：http://hz.0kj1m.cn/gtnaharvbt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinqigufen.top/gtptjhwtlo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gtlfihuudt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtqeheqrkc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtcpumkflt.html


<!-- 参考信息 -->