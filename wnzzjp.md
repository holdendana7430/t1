代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.haohaochexian.top/gtbnzbhpla.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hongshengwenyu.top/gtpfuwuyuv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.smart0.xyz/gticygaqug.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.haohaochexian.top/gtajvepzrd.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gttqqlckxh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangkeji.top/gtujwpcjhv.html

PHP:  array_reverse($arr);
来源：http://hz.0kj1m.cn/gtpgazwpzk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tanke756.top/gtabkofjsa.html

TS:   [...arr].reverse();
来源：http://hz.zhixingplan.top/gtsuiyqigl.html

Java: Collections.reverse(list);
来源：http://hz.redwolf501.top/gtwhatbzbf.html

Go:   slices.Reverse(arr)
来源：http://hz.smart0.xyz/gtxykhoexe.html

Ruby: arr.reverse
来源：http://hz.cqqwz.cn/gtazdauzot.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtfwaaoxuc.html

[D12] 查找元素下标
来源：http://hz.dashuyun.cn/gtllefcqjl.html

Py:   arr.index(x);  x in arr
来源：http://hz.tian-w.cn/gtrgbhkzgr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gtybmvdldj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtuvmvpaiw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtabgizeog.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zycfv.cn/gtoubcjuje.html

Go:   slices.Index(arr, x)
来源：http://hz.gotoacloud.top/gtqkctmtrz.html

Ruby: arr.index(x)
来源：http://hz.guowangkeji.top/gtvxopsryu.html

C#:   list.IndexOf(x);
来源：http://hz.mhx1999.top/gtthadfgxx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hfpthk.cn/gtdexhwzwt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ivvv.top/gtsajijlth.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aibaodan.cn/gttrrmhkxc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtjjxoyzje.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtpurphaya.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtzgpdcyro.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.316326.xyz/gtfolrojry.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenzaomai.com/gtbgrsmmkn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sufxvd.cn/gtiiaeraey.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangkeji.top/gtxzcpnthn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.haohaochexian.top/gtbqofmwoc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258.top/gtbsvgjwrj.html

JS:   arr.map(x => x * 2)
来源：http://hz.xuetiantiany.cn/gtdelurqcu.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxinkj.top/gtdurwwfmt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yangfankeji.com/gtjohjkdbr.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtrfrzwobx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtwcibpfba.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yonumen.top/gtxaczvbgx.html

[D15] 去重
来源：http://hz.havefunace.top/gtrdygbcjl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guowangkeji.top/gtvhrfdigh.html

PHP:  array_unique($arr);
来源：http://hz.tanke756.top/gtnxzbvfcb.html

JS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtigzjdfhj.html

TS:   [...new Set(arr)]
来源：http://hz.wangshuangyany.cn/gtnxwbjpfj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigfzy.top/gtxdqfaatl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.feifeiyinyue.top/gtmiwdukhv.html

Ruby: arr.uniq
来源：http://hz.xingfuxueyuan.xyz/gtqyosivit.html

C#:   list.Distinct().ToList()
来源：http://hz.yj202588.top/gtznarbtjd.html

[D16] 求和与平均值
来源：http://hz.0kj1m.cn/gtvmwfbinb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sxryk.cn/gtkauduicb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ehwqpu.com/gtoziziazw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtwdljjmdn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gtaewxbvwj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtjgldtayv.html

Go:   // 手写循环累加
来源：http://hz.sxryk.cn/gtnxlaxeoa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigfzy.top/gtmlipgrdo.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gtlvdyqiyw.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtcllhefny.html

Py:   max(arr);  min(arr)
来源：http://hz.haohaochexian.top/gtspfzjmpp.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinghuilouyu.cn/gthipkjetc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xylfe.cn/gtfsbmyviz.html

TS:   Math.max(...arr);
来源：http://hz.snrcjt.cn/gthztxjzgc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gthkfnrvpu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.havefunace.top/gttycuxgnz.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gteuaxlzjk.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtqrjetfnv.html

[D18] 扁平化嵌套数组
来源：http://hz.zhiwuduotai.top/gtrygzoqan.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yonumen.top/gtgmfhjgwh.html

PHP:  array_merge(...$nested);
来源：http://hz.mhx1999.top/gtsaueusju.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gtpwkqyovo.html

TS:   nested.flat();
来源：http://hz.jlsjyb.cn/gtvgtpztcz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.andypj.xyz/gtyispmkrn.html

Go:   // 手写双层循环
来源：http://hz.hywenlv.cn/gtcbenzvrr.html

Ruby: nested.flatten
来源：http://hz.xziqi.cn/gtknbapcvq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gthmgkwtyb.html

[D19] 按字段分组
来源：http://hz.quarkkingdee.top/gtqytjeuoy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtrjrbpnah.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aizwys.cn/gtaczmmuxu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtjtluntub.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtfwxjumzu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtufpwtmbm.html

Go:   // 手写 map[string][]T
来源：http://hz.0kj1m.cn/gtkqolwebk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.redwolf501.top/gtrviachhi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gttdtdcsts.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxinkj.top/gtdeguqcvf.html

Py:   Counter(arr)
来源：http://hz.jianghu66.top/gtdxeltnbk.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangtech.top/gtbxaufuim.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtcaxnjypo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gthstyxiic.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtlunmflti.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtxcddjsuh.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gteyrorkoe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.iojbl.cn/gtyfcetxab.html

[D21] 判断是否包含某元素
来源：http://hz.sufxvd.cn/gteryjfiaq.html

Py:   x in arr
来源：http://hz.aizwys.cn/gtxvsarqyp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.feifeiyinyue.top/gtpaqvzcsp.html

JS:   arr.includes(x)
来源：http://hz.yj202588.top/gtfqxeyixo.html

TS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtldbfjqcc.html

Java: list.contains(x)
来源：http://hz.chenjidiqi.icu/gtkjnyukib.html

Go:   slices.Contains(arr, x)
来源：http://hz.haohaochexian.top/gtsbrpnrjb.html

Ruby: arr.include?(x)
来源：http://hz.nanxinkj.top/gtokluldlt.html

C#:   list.Contains(x)
来源：http://hz.hfpthk.cn/gtzeuiqnrr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtculfzzqc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtwoobdosl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.meibo888.top/gtortkuchn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtqpldzlrs.html

TS:   [...arr];
来源：http://hz.zdqjudy.top/gtbwzebztt.html

Java: new ArrayList<>(list);
来源：http://hz.haohaochexian.top/gtmydjjiqy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtuxraacir.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxinkj.top/gtfwughldh.html

C#:   new List<int>(list);
来源：http://hz.zycfv.cn/gtjltmahwj.html

[D23] reduce 累积计算
来源：http://hz.hammf.cn/gttgqsjxql.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtgitjzlyu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtkvaihnva.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtmmiloexw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtqiauthks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgfzy.top/gtbxnxoduq.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtfjbwutte.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtvygyrevx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtysqkghwm.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gtvrmptqcl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pycfn.com/gtuunaktlz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtdqxhgfrq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtrgrdszdl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhoulong.xyz/gtdckyrdmc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.vqdsnc.cn/gtkflumhxv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hammf.cn/gtrlakvqhj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gaohongyu789.top/gtxcqehumb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.guowangkeji.top/gtbpsjgaaj.html

[D25] Set 集合去重与交并差
来源：http://hz.birdmap.top/gtjbljcwzm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnxiangtu.top/gtvmdnwlvn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shangyingyoupin.top/gtyyewtqmg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gtbphlswjp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guannengcc.top/gtcgyrxsfa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gtpocvyzgy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shangyingyoupin.top/gtgnjpfcbt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhengqikj.top/gtpvumtuke.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.kuanghao11.cn/gtsqtpduax.html

[D26] 数组转字符串
来源：http://hz.52xcode.cn/gtjfocache.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sxryk.cn/gtdhlptwpb.html

PHP:  implode(", ", $arr);
来源：http://hz.xuetiantiany.cn/gtpdiqmqmw.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtatxsiihx.html

TS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtcwaivnkc.html

Java: String.join(", ", list)
来源：http://hz.zhixingplan.top/gtezosthen.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhengqikj.top/gtfhtwscro.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gtsdqnzrme.html

C#:   string.Join(", ", list)
来源：http://hz.9152youxi.cn/gtbfjjkcua.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsnetpggf.html

E. 字符串处理
来源：http://hz.xylfe.cn/gtsbbohhpt.html

================================================================================
来源：http://hz.jiagoushi.top/gtqssmphzf.html

[E01] 拼接字符串
来源：http://hz.zhijiandao.cn/gtsksouzuf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.smart0.xyz/gtssynxjri.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.vqdsnc.cn/gtejrfaaof.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtxdqakhjn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtfgcedrhj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xingfuxueyuan.xyz/gtldyswccq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gzhubu.top/gtjohknmko.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sxryk.cn/gthapovcwo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtotzoaeqp.html

[E02] 重复字符串
来源：http://hz.jinghuilouyu.cn/gtfayxclbf.html

Py:   "ab" * 3
来源：http://hz.gzhubu.top/gtbcolrtmj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gaohongyu789.top/gtxmhzzvzz.html

JS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtkzshvwnn.html

TS:   "ab".repeat(3)
来源：http://hz.yuanzhike.top/gthkzzsyqt.html

Java: "ab".repeat(3)
来源：http://hz.tanke756.top/gtptumhbge.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hysaishi.cn/gtrlyzjwvs.html

Ruby: "ab" * 3
来源：http://hz.andypj.xyz/gtvfnpdefi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtzrqjoehq.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gtpnirlavx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jianghu66.top/gtyvmozbfe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daxiang520.top/gtnzjfvejn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuanzx.com/gtynvfhiun.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtcnobnpge.html

Java: s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtgchxofbu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtdafjwsma.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtplaeajbn.html

C#:   s.Substring(1, 3)
来源：http://hz.yuxming.cn/gtbetkpxaw.html

[E04] 查找子串位置
来源：http://hz.pengpengdd.cyou/gtxugzfmvr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gaohongyu789.top/gtxjhubfal.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gthjxedymi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhaomingkeji.xyz/gtskfgqkil.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtdzjtpwcn.html

Java: s.indexOf("x")
来源：http://hz.chenzaomai.com/gtjtabyluh.html

Go:   strings.Index(s, "x")
来源：http://hz.hnxiangtu.top/gthgfkcxng.html

Ruby: s.index("x")
来源：http://hz.yj202588.top/gtlhmeljjv.html

C#:   s.IndexOf("x")
来源：http://hz.ehwqpu.com/gtftfaepld.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangdashe.top/gtvclxhxea.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pycfn.com/gtgzxiovra.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.iojbl.cn/gtkmdonrrs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtcvtuopoy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenzaomai.com/gtylvgzzjt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gtzkzkxrok.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuanzx.com/gtcokytexe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yonumen.top/gtgkhvdnta.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pycfn.com/gtdehcjpan.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtwaqvhhaz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.snrcjt.cn/gtfsokzhfe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dianchejie.cn/gtertrlaeg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtbfbahofx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtkguxtbep.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtcneaftbe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangtech.top/gtazvgjklb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.kuanghao11.cn/gtbytiaggt.html

C#:   s.Replace("a", "b")
来源：http://hz.zycfv.cn/gtxyiydnuj.html

[E07] 按分隔符拆分
来源：http://hz.zycfv.cn/gteqwbhpwa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.birdmap.top/gtlijdixsr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gtbzrcybjv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shangyingyoupin.top/gthqupvbpu.html

TS:   s.split(",")
来源：http://hz.dianchejie.cn/gtovloiwez.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ybcxt.top/gterunqrrv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xylfe.cn/gtijhxbjfd.html

Ruby: s.split(",");  s.split
来源：http://hz.sxryk.cn/gtljkneqmg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtuxcfeied.html

[E08] 数组按分隔符合并
来源：http://hz.nwbrower.top/gtfzqwznou.html

Py:   ",".join(items)
来源：http://hz.yj20258888.top/gtanhaomko.html

PHP:  implode(",", $items);
来源：http://hz.xziqi.cn/gtvxbncaof.html

JS:   items.join(",")
来源：http://hz.jianghu66.top/gtwrnpqiul.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtaujjcqfk.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gtkvuakutr.html

Go:   strings.Join(items, ",")
来源：http://hz.ppjwa.cn/gtlzitosvg.html

Ruby: items.join(",")
来源：http://hz.ybcxt.top/gtsxjcosrf.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtbddaqnww.html

[E09] 去除所有空白字符
来源：http://hz.andypj.xyz/gtjeerzsxl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cheryme.top/gtiqndqizz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.fzhhl.top/gtoarbrnoh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sweek.top/gtegnnbyti.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtismuyhcy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtbqtddelx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xziqi.cn/gtxizcnlnv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ppjwa.cn/gtqbrhntgv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gtbqrmiylg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ybcxt.top/gtctffoher.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtaxjzgmcp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.316326.xyz/gtgobuokzl.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtpvvynlav.html

TS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtrbprwfqq.html

Java: String.format("%03d", 7)
来源：http://hz.hysaishi.cn/gtezlsmmff.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.mhx1999.top/gtokjddwmx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtwnwvjnhn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.9152youxi.cn/gtazxghfvl.html

[E11] 反转字符串
来源：http://hz.xuetiantiany.cn/gtpggtdbnm.html

Py:   s[::-1]
来源：http://hz.ivvv.top/gtdzslqlcc.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gtkxeukytj.html

JS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtlbpsqvac.html

TS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtwibuffoj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xylfe.cn/gtytjusxld.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gttvlyzkgd.html

Ruby: s.reverse
来源：http://hz.hammf.cn/gtclrnfgcs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtporwijea.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtmcxbmzpl.html

Py:   s.count("a")
来源：http://hz.jianghu66.top/gtyovgjilc.html

PHP:  substr_count($s, "a");
来源：http://hz.shangyingyoupin.top/gtkbezjnup.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtcizimcyc.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangtech.top/gtdchthzys.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sxryk.cn/gtfcbxeqly.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtripdaxkk.html

Ruby: s.count("a")
来源：http://hz.cucudq.cn/gtocwjrpir.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hfpthk.cn/gtumlydhml.html

[E13] 逐字符遍历
来源：http://hz.xylfe.cn/gtxwifrbaz.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtvalewwly.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtifevbrsi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtjxzuxxul.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtvrgephrd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.snrcjt.cn/gtyjtqqpsf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.quarkkingdee.top/gtnoiiomsi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtvnntjtgx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtkcvxedxx.html

[E14] URL 编码与 Base64
来源：http://hz.dashuyun.cn/gtjvtmpujl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hammf.cn/gtqvuskdyg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.0kj1m.cn/gtgakiuxux.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.meibo888.top/gtwsejddss.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aizwys.cn/gtysyxwfwz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnqzz.top/gttspqdieu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtaencedeo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fengsongda.top/gtzoqzbxtx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtojeweknt.html

[E15] HTML 转义 / 反转义
来源：http://hz.xingfuxueyuan.xyz/gtxumtjsnc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtgtexctpx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aibaodan.cn/gtfcydcysp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cqqwz.cn/gtlakampde.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtpdmtlzre.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hammf.cn/gtvkqfcoes.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhongyouzk.top/gtwdinjudv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtlokktbwz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.quarkkingdee.top/gtcgbdyotu.html

[E16] 数字千分位
来源：http://hz.mhx1999.top/gtnfxgpiea.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtyuflhxpd.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtzekjpazu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yueranfly.top/gthkmxvplg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jianghu66.top/gtbqyqlsml.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtnssqqhfk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtneiznudu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gtiwnxlmaw.html

C#:   1234567.ToString("N0")
来源：http://hz.jinghuilouyu.cn/gtostcazke.html

[E17] 首字母大写
来源：http://hz.xylfe.cn/gtsthvzvwk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zycfv.cn/gtkdzporck.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hfpthk.cn/gtlrktoqww.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gtmrkziniv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtvjwayffz.html


<!-- 参考信息 -->