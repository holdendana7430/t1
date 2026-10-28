代发 wailian999

PHP:  sort($arr);
来源：http://hz.shangyingyoupin.top/gtrmkprwmd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.feifeiyinyue.top/gtebhvhrhj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.havefunace.top/gthwqjfzgn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gogol.net.cn/gtailergdn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtrzmwpsjl.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtnihxjiuj.html

C#:   list.Sort();
来源：http://hz.dashuyun.cn/gthpjwopms.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhiwuduotai.top/gttydkwrex.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yonumen.top/gtxyfrdjfs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtyxiqodjb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtzaipjcwf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtxbfqtsxn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guowangkeji.top/gtagpmlcio.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhijiandao.cn/gtbjoyphwu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xingfuxueyuan.xyz/gtddyofgwr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258.top/gttkciqgtz.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtxybiuxfc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cheryme.top/gtluuickdg.html

PHP:  array_reverse($arr);
来源：http://hz.jqgufenzy.top/gtbfrllomt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zycfv.cn/gtjjscnjgb.html

TS:   [...arr].reverse();
来源：http://hz.meibo888.top/gtewjdfzxp.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtqdnabmzl.html

Go:   slices.Reverse(arr)
来源：http://hz.ydzc1.top/gtnqmaqrma.html

Ruby: arr.reverse
来源：http://hz.svipenyu.cn/gtpauhalzo.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtnvqwrdgx.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gtvxrlwyzd.html

Py:   arr.index(x);  x in arr
来源：http://hz.vqdsnc.cn/gthtnyhruc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dianchejie.cn/gtpvogqpdh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtjrqzsjiz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.0kj1m.cn/gtlvisjhsz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gtiwznsyyc.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gtieucxrfh.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtknaffpmt.html

C#:   list.IndexOf(x);
来源：http://hz.ydjk.org.cn/gtasfjqlxh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guowangkeji.top/gtsuqnxlhe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.havefunace.top/gtvkpzcssh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xinyue.icu/gtddlwyzzw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gttmvdseby.html

TS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtdligbcmk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gtgpqcnaie.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gtxtilcviy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnxiangtu.top/gtmqdsjzsk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.andypj.xyz/gtkzwnsdcc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinghuilouyu.cn/gtsdgzxxrr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gtpphyevru.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gtulovzwbi.html

JS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtvixmfdot.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenlongwang.top/gtcffieeld.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cdnleiting.top/gtiyyxdjbf.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtcsqkmetp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.mhx1999.top/gtvjftgmtq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtkmxrfgjw.html

[D15] 去重
来源：http://hz.meibo888.top/gtrgkrhrun.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtjkjykyul.html

PHP:  array_unique($arr);
来源：http://hz.sufxvd.cn/gtjccduigl.html

JS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtwwqkjmus.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtywgzlvpg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtxsnasnwh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtnsruzurd.html

Ruby: arr.uniq
来源：http://hz.nanxuanxn.top/gtziyirmro.html

C#:   list.Distinct().ToList()
来源：http://hz.dashuyun.cn/gtdufsuzgk.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtbkqbzwvh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydzc1.top/gtyjuztheg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pengpengdd.cyou/gtvswoeeki.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtpvsbrkgq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtwhdptdzz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtdrzhmskh.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangkeji.top/gtproyshdk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtplpssunn.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhijiandao.cn/gtbnoimpxg.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtvwnjsumu.html

Py:   max(arr);  min(arr)
来源：http://hz.zycfv.cn/gtbiflaccs.html

PHP:  max($arr);  min($arr);
来源：http://hz.yuxming.cn/gtrkntpfsf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtklolkauq.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtjmbmxpfr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj202588.top/gtadgyhorz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenzaomai.com/gtdtrxvqwi.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtjkxajqpj.html

C#:   list.Max();  list.Min()
来源：http://hz.zhengqikj.top/gtfhbxcrey.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gtlequxyid.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtelzfvciy.html

PHP:  array_merge(...$nested);
来源：http://hz.shzxlz.cn/gtraevuqxi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.52xcode.cn/gtejaxtdoh.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtpyhastht.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.snrcjt.cn/gtufafuslj.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtwnqcllhr.html

Ruby: nested.flatten
来源：http://hz.yongpay.top/gtrcqmpcyl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.kuanghao11.cn/gtnajtyrrm.html

[D19] 按字段分组
来源：http://hz.nanxuanxn.top/gtdeeumcyr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yueranfly.top/gtznqsgvzn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtoubkpdeq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gtzfznxqcj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shangyingyoupin.top/gtlseeaytq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtasvougzo.html

Go:   // 手写 map[string][]T
来源：http://hz.jiagoushi.top/gtjyfmgyzz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigufen.top/gtnkznqwjs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jyoumei.cn/gtozxowppe.html

[D20] 统计每个元素出现次数
来源：http://hz.aizwys.cn/gtiblcgaxj.html

Py:   Counter(arr)
来源：http://hz.yj20258.top/gtbmhijfps.html

PHP:  array_count_values($arr);
来源：http://hz.fzhhl.top/gtndkmhjvl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtcrwzldqm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtaeyullbz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtwtqdfrbc.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gtzbxfepom.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtiqinhrgi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigufen.top/gtramucgna.html

[D21] 判断是否包含某元素
来源：http://hz.redwolf501.top/gtmmdagbgt.html

Py:   x in arr
来源：http://hz.zhixingplan.top/gtzzaznvyg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenlongwang.top/gtfadpytsa.html

JS:   arr.includes(x)
来源：http://hz.zhijiandao.cn/gtporlidaz.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtwoykvfuj.html

Java: list.contains(x)
来源：http://hz.xuanzx.com/gtvaabqqjw.html

Go:   slices.Contains(arr, x)
来源：http://hz.tianlin.xyz/gtcywnfaqp.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gtghparrdp.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtbdbgnewl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cashguo.top/gtmmolcjzj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pengpengdd.cyou/gtwdvryfxo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtzzwiwlwd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jlsjyb.cn/gtnaxjgjiy.html

TS:   [...arr];
来源：http://hz.xingfuxueyuan.xyz/gtzycmdvds.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtsdtkyhot.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gogol.net.cn/gteurpjnht.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenjidiqi.icu/gtcqrvnrkd.html

C#:   new List<int>(list);
来源：http://hz.zhiwuduotai.top/gtiygnavok.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gttiewrouj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenzaomai.com/gtscweebir.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258.top/gtutzkjljd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtqhbtjhwb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cqqwz.cn/gtqpxtwmhy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.quarkkingdee.top/gtleuiwixi.html

Go:   // 手写循环
来源：http://hz.ydzc1.top/gtqwjsilwe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nwbrower.top/gtzgarhpnc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtpvwkjrin.html

[D24] 字典 / Map 基本操作
来源：http://hz.c1oappe.top/gtfkgbagns.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gtlkrvlhgd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhongyouzk.top/gtgfvqmxua.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aibaodan.cn/gtldtjkbrx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtawhsqtbj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hongshengwenyu.top/gtxhtozloa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtqzqvirvm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hysaishi.cn/gtxobfhwyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sysykeji.top/gtvhmlmjxb.html

[D25] Set 集合去重与交并差
来源：http://hz.tanke756.top/gtiapkjqdp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cdnleiting.top/gtderdjrzk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhiwuduotai.top/gtviqocpci.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtpkkcdcca.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gthuynvbca.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shangyingyoupin.top/gtjgrukewo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gogol.net.cn/gtmetkywvl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shuidangran.top/gtgyvvugtj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenjidiqi.icu/gtngcnwomz.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gttquvehkk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fzhhl.top/gtvepocvnr.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtpvtruplc.html

JS:   arr.join(", ")
来源：http://hz.pycfn.com/gtoucedzqc.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtpypmkrsv.html

Java: String.join(", ", list)
来源：http://hz.andypj.xyz/gtfovlcfjw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtdiuewrev.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gtbidzpfgw.html

C#:   string.Join(", ", list)
来源：http://hz.yueranfly.top/gtwspgttco.html

================================================================================
来源：http://hz.yueranfly.top/gtuvsgyhxa.html

E. 字符串处理
来源：http://hz.xylfe.cn/gtpbnlnoqa.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmyibxfoa.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtnmdupjzm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenlongwang.top/gtrnhbjlcw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ehwqpu.com/gtdxmzdqer.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtafrgazoq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cheryme.top/gtwzircpol.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.snrcjt.cn/gtrjevnsxh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.c1oappe.top/gtfeghqeus.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhaomingkeji.xyz/gtbkejzxjo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtmcsmjaze.html

[E02] 重复字符串
来源：http://hz.kuanghao11.cn/gtenvpsxja.html

Py:   "ab" * 3
来源：http://hz.sufxvd.cn/gtihnmpruo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tian-w.cn/gtxrsmtlyi.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtuuvzkiwg.html

TS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtvmwubqlw.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtzuqcimnb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258888.top/gtzendjuhb.html

Ruby: "ab" * 3
来源：http://hz.pengpengdd.cyou/gtndydhxrn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xinyue.icu/gtxzacogyw.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtfoluqiwh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hywenlv.cn/gtlkkqwjuo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtvajulgxp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtqfmouaak.html

TS:   s.slice(1, 4)
来源：http://hz.sysykeji.top/gthnrmrfix.html

Java: s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtmlakknjp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gtmuvdnauj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhoulong.xyz/gtpdkreavd.html

C#:   s.Substring(1, 3)
来源：http://hz.redwolf501.top/gtdxmosnxp.html

[E04] 查找子串位置
来源：http://hz.jyoumei.cn/gtatehnncd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hammf.cn/gtkneoyahs.html

PHP:  strpos($s, "x");
来源：http://hz.zycfv.cn/gtvdiuzqlx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydjk.org.cn/gtjhuelbsj.html

TS:   s.indexOf("x")
来源：http://hz.sysykeji.top/gttutolnzr.html

Java: s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtmehspacu.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gtlwfuxtch.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtjhoyvbii.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gttlmrjvnz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtklcbpzxq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ivvv.top/gtablhkpto.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gteauawgsj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtlxxwridh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hysaishi.cn/gtwccfbxxq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtulziyhdz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.birdmap.top/gtiiizysgt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258.top/gtmqegirni.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pengpengdd.cyou/gtosycqtyn.html

[E06] 替换子串
来源：http://hz.daria6918.cn/gtaxrmnhov.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtiquggqoi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.feifeiyinyue.top/gtpcvnqhbl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtoyewqwsl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtryxeiile.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtjqlfcbzv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenlongwang.top/gtowhxqwlo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.52xcode.cn/gttprxysar.html

C#:   s.Replace("a", "b")
来源：http://hz.cucudq.cn/gtezackvkk.html

[E07] 按分隔符拆分
来源：http://hz.fengsongda.top/gtyqqygeid.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.snrcjt.cn/gtvvntheln.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hysaishi.cn/gthblgwkqo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhixingplan.top/gtbadomkaz.html

TS:   s.split(",")
来源：http://hz.shanyushiyangkeji.top/gtcrunlodb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gtndnonxoo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.haohaochexian.top/gtdbfkmjpb.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gtjazpwhop.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sxryk.cn/gthgusuukq.html

[E08] 数组按分隔符合并
来源：http://hz.yangfankeji.com/gtgrwhpvvj.html

Py:   ",".join(items)
来源：http://hz.havefunace.top/gtogpocogy.html

PHP:  implode(",", $items);
来源：http://hz.hnqzz.top/gtbwrhltbn.html

JS:   items.join(",")
来源：http://hz.sufxvd.cn/gtntimdjmz.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtosrvnwxn.html

Java: String.join(",", items)
来源：http://hz.jqgufenzy.top/gthqhafwhf.html

Go:   strings.Join(items, ",")
来源：http://hz.ehwqpu.com/gtinasctdd.html

Ruby: items.join(",")
来源：http://hz.quarkkingdee.top/gtzgojyjzc.html

C#:   string.Join(",", items)
来源：http://hz.dashuyun.cn/gtgrgtsqof.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangtech.top/gtyymlawiz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhengqikj.top/gtyykidpwj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.316326.xyz/gtsakqrbuw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtqfvdqtou.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtjwcqgelh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtawztmsta.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dashuyun.cn/gtqteimovz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guannengcc.top/gtvaaynvrq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.andypj.xyz/gtbxjydjih.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jyoumei.cn/gtyvjvqhsh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtbcbnbilc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhixingplan.top/gtwiehyypw.html

JS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtivkdctmt.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gteyoufber.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gthjnozapu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cdnleiting.top/gtbftfxlhx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zdqjudy.top/gtobdxuctp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.iojbl.cn/gtaxvasuxm.html

[E11] 反转字符串
来源：http://hz.zhiwuduotai.top/gtdoihbayw.html

Py:   s[::-1]
来源：http://hz.chenjidiqi.icu/gtftrohcrn.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtdqaenpem.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gttxxnorny.html

TS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtbnptsneb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtulemnchr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtdnuvhiky.html

Ruby: s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtbxwplemk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtrjtvbric.html

[E12] 统计某字符出现次数
来源：http://hz.cucudq.cn/gtuxkjldja.html

Py:   s.count("a")
来源：http://hz.hammf.cn/gtofyyflkp.html

PHP:  substr_count($s, "a");
来源：http://hz.sysykeji.top/gtclwczemf.html

JS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtynyczrur.html

TS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtgotnctap.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fengsongda.top/gtmqffdfra.html

Go:   strings.Count(s, "a")
来源：http://hz.wangdashe.top/gtwhspwmzb.html

Ruby: s.count("a")
来源：http://hz.hnxiangtu.top/gtiodwvoov.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tian-w.cn/gtpzbssuob.html

[E13] 逐字符遍历
来源：http://hz.vqdsnc.cn/gtmhxdngeo.html

Py:   for ch in s: print(ch)
来源：http://hz.316326.xyz/gtvvttkntz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gtotasdgfn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gthcjrtswf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtyftjnefc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.dianchejie.cn/gtccrcjzcc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtcssyhvdf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gzhubu.top/gtiyxkhihy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gtkbrhxngz.html

[E14] URL 编码与 Base64
来源：http://hz.wangdashe.top/gticnpufjx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtidihyjcr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hongshengwenyu.top/gthqnakypc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.andypj.xyz/gtpshotvsr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258.top/gtdtfpyrtp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.svipenyu.cn/gttphjlvsv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtunlkagen.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.snrcjt.cn/gtbvgzekkh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtibetexbg.html

[E15] HTML 转义 / 反转义
来源：http://hz.jianghu66.top/gtgfjkvegv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtcooscaai.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jyoumei.cn/gttfhsxoqq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenjidiqi.icu/gtcpmwmqiz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gtdpaghumb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cucudq.cn/gtmxraooeg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sxryk.cn/gthlvkmcwy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zycfv.cn/gtvtnxkmhb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtmdezkekj.html

[E16] 数字千分位
来源：http://hz.9152youxi.cn/gtkxxsayhl.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gtmbavjkhz.html


<!-- 参考信息 -->