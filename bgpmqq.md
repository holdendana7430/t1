代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tianlin.xyz/gtqzovydfc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gthjryiyvk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtrqovxqcx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gttlyrywqq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangkeji.top/gttoezoyyk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhongyouzk.top/gtwifuxope.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhongyouzk.top/gtfupyxycp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuetiantiany.cn/gteavfsyiv.html

[D11] 反转数组
来源：http://hz.aizwys.cn/gtfbnjnfjg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aibaodan.cn/gtavtgyzkn.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtocwpqpoq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigufen.top/gtsjduufrs.html

TS:   [...arr].reverse();
来源：http://hz.svipenyu.cn/gtuqnqkpdo.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangkeji.top/gtqugciuor.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangkeji.top/gtysmtjtlv.html

Ruby: arr.reverse
来源：http://hz.chenlongwang.top/gtenpkaoea.html

C#:   list.Reverse();
来源：http://hz.0kj1m.cn/gtkiwpbbwq.html

[D12] 查找元素下标
来源：http://hz.zhixingplan.top/gtgtzmzljn.html

Py:   arr.index(x);  x in arr
来源：http://hz.vqdsnc.cn/gtbyahfosd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jianghu66.top/gtcbqzbhvw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtgpkdiwpf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtttrtavsc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yanxiufei.cn/gtxzprfgal.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gtcjaxhtji.html

Ruby: arr.index(x)
来源：http://hz.snrcjt.cn/gtwyfecgoo.html

C#:   list.IndexOf(x);
来源：http://hz.0kj1m.cn/gtcqlbwmna.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gotoacloud.top/gtxbqyohou.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtofbzcwll.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.havefunace.top/gtllslnlna.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtokedfwkj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gteppkplmv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guowangkeji.top/gtqodqhcpg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gotoacloud.top/gthtrxbbea.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gteswfwuvt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangkeji.top/gtaqljaczk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yonumen.top/gtlanshicw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ppjwa.cn/gtlgabcoli.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtiqclasop.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtjtidhorm.html

TS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gthluakvqx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.svipenyu.cn/gttksrfblm.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtxixwbooz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gtfttsjtvh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.mhx1999.top/gtctlcosgu.html

[D15] 去重
来源：http://hz.havefunace.top/gtrcgssuuq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtjsmrlejc.html

PHP:  array_unique($arr);
来源：http://hz.jinqigfzy.top/gtoogjrxuf.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtpxddpdgb.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gthrllabyc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.vqdsnc.cn/gtjkpobsgm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xziqi.cn/gtuhbynywg.html

Ruby: arr.uniq
来源：http://hz.xylfe.cn/gtivdrnfou.html

C#:   list.Distinct().ToList()
来源：http://hz.zhengqikj.top/gtivmyfqmb.html

[D16] 求和与平均值
来源：http://hz.jqgfzy.top/gtadfwmacc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtchnoypxq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtokbskxhq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gttqpphxfs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtzawxzvbx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtyvuarbnx.html

Go:   // 手写循环累加
来源：http://hz.hnxiangtu.top/gtwyeidffp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aizwys.cn/gtjzdrqwok.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gtvhtcwqom.html

[D17] 最大值与最小值
来源：http://hz.aibaodan.cn/gtntllfgff.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtspyxwyvl.html

PHP:  max($arr);  min($arr);
来源：http://hz.yongpay.top/gtkjzsbdqi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gthqurrvdv.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtqelhijvs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.pengpengdd.cyou/gtzfduslsa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gtuvjtnlpx.html

Ruby: arr.max;  arr.min
来源：http://hz.tanke756.top/gtchlmngcl.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtkbmumiwk.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtpjeqhvcl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.c1oappe.top/gtovyafltb.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gtbjvcswgt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ybcxt.top/gteummvymq.html

TS:   nested.flat();
来源：http://hz.gogol.net.cn/gtizgynmrx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtrleblskw.html

Go:   // 手写双层循环
来源：http://hz.sufxvd.cn/gtvwfziskz.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtbyvfsyao.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xziqi.cn/gtxrxlkccu.html

[D19] 按字段分组
来源：http://hz.daxiang520.top/gttuntthyv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tian-w.cn/gteigqmtsh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pycfn.com/gtjncvvhmb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.mhx1999.top/gtvxwyzenp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aizwys.cn/gtgywgusot.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daxiang520.top/gtbpykfmex.html

Go:   // 手写 map[string][]T
来源：http://hz.xuanzx.com/gtjksmohhq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtkaayrvzx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtztebowzq.html

[D20] 统计每个元素出现次数
来源：http://hz.kuanghao11.cn/gtjevlzhuj.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gtmxjuuhxf.html

PHP:  array_count_values($arr);
来源：http://hz.wangdashe.top/gtsxurbpkt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yongpay.top/gtqvaokinm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtmoebinoc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtfyzfcqde.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gtxoqslknq.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtefwycgja.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuetiantiany.cn/gtibjcqgov.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gtjfjckiju.html

Py:   x in arr
来源：http://hz.jinyuanbaomall.cn/gtfxdeelzm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhaomingkeji.xyz/gtixxqkuvf.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtdaylkzik.html

TS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtecrcmxmn.html

Java: list.contains(x)
来源：http://hz.jinqigfzy.top/gtpywkohki.html

Go:   slices.Contains(arr, x)
来源：http://hz.zdqjudy.top/gthtpensue.html

Ruby: arr.include?(x)
来源：http://hz.smart0.xyz/gthwuubbzt.html

C#:   list.Contains(x)
来源：http://hz.iojbl.cn/gtolsmlbrp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.havefunace.top/gtuxeofqhe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangdashe.top/gtmsxfddan.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangdashe.top/gtvzntnadf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cqqwz.cn/gthuahfdyj.html

TS:   [...arr];
来源：http://hz.meibo888.top/gtoxkjrazr.html

Java: new ArrayList<>(list);
来源：http://hz.sxryk.cn/gtzkzygnki.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhengqikj.top/gtzuwcmiif.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aizwys.cn/gtrckzrrko.html

C#:   new List<int>(list);
来源：http://hz.yueranfly.top/gtclifbqxu.html

[D23] reduce 累积计算
来源：http://hz.hnxiangtu.top/gtvtdqrncg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.havefunace.top/gteocujzkm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgfzy.top/gtxcxtmzki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtyktcfska.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtzznpocdx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhongyouzk.top/gtorlljjsc.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtxpmrijts.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinyuanbaomall.cn/gttolbtsob.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtsyvyphfc.html

[D24] 字典 / Map 基本操作
来源：http://hz.shuidangran.top/gtrldxegsv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258.top/gtaxlwkzos.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.andypj.xyz/gtpqewehbd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtpykdaiah.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258.top/gtkklewsey.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gtsiewbtxf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.redwolf501.top/gtxvlohepz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yanxiufei.cn/gtwnonloeh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtmxnshhab.html

[D25] Set 集合去重与交并差
来源：http://hz.dashuyun.cn/gtlpwvdaor.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtgeiaboof.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hammf.cn/gtvfjbhlwg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gttlsmljbz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigfzy.top/gtlglksxan.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigfzy.top/gtlydtayjp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtmnsmpkch.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gtqsojjgjx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yangfankeji.com/gtcauovwlu.html

[D26] 数组转字符串
来源：http://hz.svipenyu.cn/gtzgdgtfgn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gtaewdnugs.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtcsvmjhhl.html

JS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtneqehqsa.html

TS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtfudzmvgn.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtthqmdblw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258888.top/gtuoqhyscy.html

Ruby: arr.join(", ")
来源：http://hz.chenzaomai.com/gtqkutkrpx.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtjzdyqqao.html

================================================================================
来源：http://hz.hnqzz.top/gtpwamdpdf.html

E. 字符串处理
来源：http://hz.ppjwa.cn/gtbyucwoex.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtxnvtexyc.html

[E01] 拼接字符串
来源：http://hz.guannengcc.top/gtswwoewas.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jiagoushi.top/gtmhvljfqc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigufen.top/gtoloqhrqq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gttqyjvcpm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtsbbehumx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daria6918.cn/gtrpucvjmz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.dianchejie.cn/gtcrklkpct.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xziqi.cn/gtisoptoob.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jyoumei.cn/gtsipfcfgx.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gttyirczmb.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtahseqymn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhaomingkeji.xyz/gtvracwvwf.html

JS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtzlwdzdbj.html

TS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtpnspdlrz.html

Java: "ab".repeat(3)
来源：http://hz.mhx1999.top/gtmxybfxkc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtlpxtgdui.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtyeqvrvzl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtjhsxgecd.html

[E03] 截取子串
来源：http://hz.hfpthk.cn/gtsvelmtxt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.bjfxy.top/gtawetnzhi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.birdmap.top/gtrvpuncld.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gtgycrqrqi.html

TS:   s.slice(1, 4)
来源：http://hz.zycfv.cn/gthngoexos.html

Java: s.substring(1, 4)
来源：http://hz.xziqi.cn/gtrsyijznm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtsrzlcyns.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gtmbxhiuan.html

C#:   s.Substring(1, 3)
来源：http://hz.hnxiangtu.top/gtlkosbnop.html

[E04] 查找子串位置
来源：http://hz.ywan-chungtsiang.top/gtwqkpeihp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtukyyktzf.html

PHP:  strpos($s, "x");
来源：http://hz.havefunace.top/gtzmupzral.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydzc1.top/gtkbxogfvw.html

TS:   s.indexOf("x")
来源：http://hz.jinqigufen.top/gtztwmixxm.html

Java: s.indexOf("x")
来源：http://hz.hywenlv.cn/gtoxytnahi.html

Go:   strings.Index(s, "x")
来源：http://hz.wangshuangyany.cn/gtwoqlziyx.html

Ruby: s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtvqnupwme.html

C#:   s.IndexOf("x")
来源：http://hz.jiagoushi.top/gtjkyyhjkv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtjxugevmh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ybcxt.top/gtmaukymfn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gtdhikbumm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtbcqatjwi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.0kj1m.cn/gttdejovsk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cdnleiting.top/gtdewxujhc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtcgbkpigv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuanzhike.top/gtgbpirmjb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ivvv.top/gtcolveysi.html

[E06] 替换子串
来源：http://hz.wangshuangyany.cn/gtfgshaeqm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.smart0.xyz/gtyhmfvjdu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yvedp.cn/gtdxpgpeyi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtvqyiwtpi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtotugpmxy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtbkoyudyr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxuanxn.top/gtuanbefke.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gaohongyu789.top/gttqhatqqa.html

C#:   s.Replace("a", "b")
来源：http://hz.shangyingyoupin.top/gtpzdaqbug.html

[E07] 按分隔符拆分
来源：http://hz.jqgfzy.top/gtypmeojoa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gtfkbbfdhm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jlsjyb.cn/gtzcnfydod.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ppjwa.cn/gtzmfwcgzv.html

TS:   s.split(",")
来源：http://hz.chenzaomai.com/gtlpelpxxe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhijiandao.cn/gtdiuawiso.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenjidiqi.icu/gtmhzvierq.html

Ruby: s.split(",");  s.split
来源：http://hz.sweek.top/gtkxficqux.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuanzhike.top/gtgnrtyrwd.html

[E08] 数组按分隔符合并
来源：http://hz.nanxinkj.top/gtsxztylcq.html

Py:   ",".join(items)
来源：http://hz.sweek.top/gtvrrjkkoj.html

PHP:  implode(",", $items);
来源：http://hz.zhengqikj.top/gtqzbjznoo.html

JS:   items.join(",")
来源：http://hz.pycfn.com/gtwvpoqcgb.html

TS:   items.join(",")
来源：http://hz.svipenyu.cn/gtkbdgcadq.html

Java: String.join(",", items)
来源：http://hz.ydjk.org.cn/gtiftxlxac.html

Go:   strings.Join(items, ",")
来源：http://hz.ydjk.org.cn/gtbswndcpo.html

Ruby: items.join(",")
来源：http://hz.iojbl.cn/gtvgewaieb.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gtzpnjiznx.html

[E09] 去除所有空白字符
来源：http://hz.shuidangran.top/gttkjflqvz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.316326.xyz/gtotdgejts.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sweek.top/gtjnfzhcmt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtksgkkwdk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtbgwkbffs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtpxetrrmi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hongshengwenyu.top/gttwikekdi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhijiandao.cn/gtlmjlyoig.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yangfankeji.com/gtzttjcufb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gzhubu.top/gtawqnhtlb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gtipovautd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nwbrower.top/gtdbpcnxjx.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtroouotlw.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gteoxgaqad.html

Java: String.format("%03d", 7)
来源：http://hz.aizwys.cn/gtxawegevt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gtcaknaite.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtqofhsnkp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtdvjtbxug.html

[E11] 反转字符串
来源：http://hz.gotoacloud.top/gtajiksvbu.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtsaswltqa.html

PHP:  strrev($s);
来源：http://hz.dianchejie.cn/gtksbtsdhz.html

JS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtrjcbezjt.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gterilblag.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.smart0.xyz/gtzivphzac.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.smart0.xyz/gtkjidzbsg.html

Ruby: s.reverse
来源：http://hz.cqqwz.cn/gtechgwgjp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtjbdrmlfm.html

[E12] 统计某字符出现次数
来源：http://hz.xinyue.icu/gthoajzvde.html

Py:   s.count("a")
来源：http://hz.daria6918.cn/gtnywlzuih.html

PHP:  substr_count($s, "a");
来源：http://hz.xylfe.cn/gttgeojovg.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtkactnqzu.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtgsqiduhl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aibaodan.cn/gtpcvwapan.html

Go:   strings.Count(s, "a")
来源：http://hz.gzhubu.top/gtpptcbkif.html

Ruby: s.count("a")
来源：http://hz.nanxuanxn.top/gtupsnkukp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gtypjlzors.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gtilhlwghx.html

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gtdrlbnmur.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtkhqhfdau.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtgvuqtpjz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtjfmtmtus.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shangyingyoupin.top/gtndfvkxxr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtaukzhvax.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtpsztkido.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258888.top/gtpdwuvvkw.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangkeji.top/gteobgrvxf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.redwolf501.top/gtludpramh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gtlghweksd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gttpolcnah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenzaomai.com/gtwigfswrk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cqqwz.cn/gtcvmjxevf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhiwuduotai.top/gthesxlnql.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ydzc1.top/gtvbiyiahb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258888.top/gtgtlksinh.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinyuanbaomall.cn/gtodznkybu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xziqi.cn/gtrbhhuerm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gtjbjhnlpq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigfzy.top/gttqgonbtm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.52xcode.cn/gtmaalefnj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.redwolf501.top/gtopzqbjmw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhijiandao.cn/gtamsxhuht.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtmhfxmxyz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxuanxn.top/gtgbvipvnl.html

[E16] 数字千分位
来源：http://hz.mhx1999.top/gtvekvwlkl.html

Py:   f"{1234567:,}"
来源：http://hz.zhoulong.xyz/gtqsnkvhdg.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtvqfrxajd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtfqwlypdi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtxgcvvsjh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gtnjglugza.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fzhhl.top/gtmrznmbnc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gtcuvgqyqd.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtunuapzig.html

[E17] 首字母大写
来源：http://hz.52xcode.cn/gtbkgiepay.html


<!-- 参考信息 -->