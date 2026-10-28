代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hysaishi.cn/gtyrcoioto.html

TS:   [...a, ...b];
来源：http://hz.xziqi.cn/gtwlekmmfv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gtbbxhctvv.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gtviusyfya.html

Ruby: a + b;  a.concat(b)
来源：http://hz.pengpengdd.cyou/gtivzvnrxu.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangdashe.top/gtuoxxtqss.html

[D09] 排序（升序）
来源：http://hz.iojbl.cn/gtfuchzrrh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gthcjgzgux.html

PHP:  sort($arr);
来源：http://hz.mhx1999.top/gtuxijghwg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhongyouzk.top/gtceupdshl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhijiandao.cn/gtrvyjneus.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jlsjyb.cn/gtrezczlst.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtlqwrpzqr.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtfputeoxc.html

C#:   list.Sort();
来源：http://hz.shuidangran.top/gtfmfiuigb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtsogyhlru.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhoulong.xyz/gtbeccvhsf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtwbccfmzm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtcyatzwua.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtgetqqxis.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.9152youxi.cn/gtvlccufik.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhiwuduotai.top/gtisiejham.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhixingplan.top/gtzxiuufsz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtkjhtfjgl.html

[D11] 反转数组
来源：http://hz.ywan-chungtsiang.top/gtqxlhmmel.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenjidiqi.icu/gtrvhygzvp.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gtdacnzncq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gzhubu.top/gteffufleg.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtvmzdbslq.html

Java: Collections.reverse(list);
来源：http://hz.dianchejie.cn/gtnhxzhdeu.html

Go:   slices.Reverse(arr)
来源：http://hz.wangdashe.top/gtcskfswjk.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtvnnykyao.html

C#:   list.Reverse();
来源：http://hz.zhoulong.xyz/gtotjjwvgb.html

[D12] 查找元素下标
来源：http://hz.cashguo.top/gtczfqqmku.html

Py:   arr.index(x);  x in arr
来源：http://hz.cashguo.top/gtianafdbn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ywan-chungtsiang.top/gttkplpmfg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtuzywbsjl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtwqsrfmwr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sweek.top/gtrusooucg.html

Go:   slices.Index(arr, x)
来源：http://hz.9152youxi.cn/gtajkekexi.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtakrzoptz.html

C#:   list.IndexOf(x);
来源：http://hz.shangyingyoupin.top/gtcvzelyzo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj202588.top/gtwyqhxkyo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ywan-chungtsiang.top/gtieldrsbd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.redwolf501.top/gtmzlqzbps.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hammf.cn/gtzzoqschl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtblwvraui.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenlongwang.top/gtnrgkjrfn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jiagoushi.top/gtraefltvh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.iojbl.cn/gtrfptgrra.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.andypj.xyz/gttryiktzs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtdwjttvef.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tian-w.cn/gtmrjismzq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.vqdsnc.cn/gtveianpcu.html

JS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtbdycrygd.html

TS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtazwxsejc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cdnleiting.top/gtgfovwavu.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtnntaxktb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yanxiufei.cn/gtwribitct.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtobjksooj.html

[D15] 去重
来源：http://hz.aizwys.cn/gtbexhzoee.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtigaxuulh.html

PHP:  array_unique($arr);
来源：http://hz.jqgufenzy.top/gttvcjrhwj.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtzvmaduqv.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtklaqlvwk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtbcjcbwwh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenlongwang.top/gtxatinldk.html

Ruby: arr.uniq
来源：http://hz.meibo888.top/gtradszihb.html

C#:   list.Distinct().ToList()
来源：http://hz.shzxlz.cn/gtmusrptll.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gtgqxffinb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shzxlz.cn/gtkcwmynpd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gaohongyu789.top/gtbpxndzua.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtslrsguau.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtysrfngqs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtpkmtzfcw.html

Go:   // 手写循环累加
来源：http://hz.wangshuangyany.cn/gtazizlbgf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtychpzack.html

C#:   list.Sum();  list.Average()
来源：http://hz.gogol.net.cn/gteflilcch.html

[D17] 最大值与最小值
来源：http://hz.yueranfly.top/gtqdgycxwe.html

Py:   max(arr);  min(arr)
来源：http://hz.ydzc1.top/gtywribjwe.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtzhtmmjxc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.andypj.xyz/gtucocybdd.html

TS:   Math.max(...arr);
来源：http://hz.fzhhl.top/gttdoeiwdp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.andypj.xyz/gthrojlrpb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ehwqpu.com/gtbeettnxr.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gtflzidlkg.html

C#:   list.Max();  list.Min()
来源：http://hz.zhiwuduotai.top/gtxctupnry.html

[D18] 扁平化嵌套数组
来源：http://hz.redwolf501.top/gtsjxxhjwj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuanzhike.top/gtrhctqjrl.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtpgizydog.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hysaishi.cn/gtazvgisyw.html

TS:   nested.flat();
来源：http://hz.jiagoushi.top/gtpaakyrhe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jiagoushi.top/gtnqyzxdfc.html

Go:   // 手写双层循环
来源：http://hz.kuanghao11.cn/gtkgnymoze.html

Ruby: nested.flatten
来源：http://hz.yangfankeji.com/gtkmumoqmx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtudrpgznt.html

[D19] 按字段分组
来源：http://hz.quarkkingdee.top/gtqjrdpnax.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.snrcjt.cn/gtmmhzobyi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guannengcc.top/gtlbvuifzq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yvedp.cn/gtjqdsmbnj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtodurqnsc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gtirtmecsw.html

Go:   // 手写 map[string][]T
来源：http://hz.wangshuangyany.cn/gtnxeqilwx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258.top/gtfjvvjrtq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fengsongda.top/gtpwrpwxwx.html

[D20] 统计每个元素出现次数
来源：http://hz.vqdsnc.cn/gtctneqkgn.html

Py:   Counter(arr)
来源：http://hz.ywan-chungtsiang.top/gtmlvbxlcc.html

PHP:  array_count_values($arr);
来源：http://hz.ydjk.org.cn/gteohbmkma.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtblijhpya.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtipdcgcbj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gtoecqiwvd.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gthmzcisxc.html

Ruby: arr.tally
来源：http://hz.fzhhl.top/gtuhrtgajm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenjidiqi.icu/gtnpnfmilo.html

[D21] 判断是否包含某元素
来源：http://hz.xinyue.icu/gtcrezqnbb.html

Py:   x in arr
来源：http://hz.andypj.xyz/gtflgdehhq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtozfbjurt.html

JS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtgcqteqvp.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtbiejutia.html

Java: list.contains(x)
来源：http://hz.yj202588.top/gtxhducchq.html

Go:   slices.Contains(arr, x)
来源：http://hz.jiagoushi.top/gteoqnwkch.html

Ruby: arr.include?(x)
来源：http://hz.fengsongda.top/gtxlgsxcyb.html

C#:   list.Contains(x)
来源：http://hz.gogol.net.cn/gtgxjvvvxw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fzhhl.top/gtolnnchfq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhiwuduotai.top/gtuaygcnww.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cucudq.cn/gtbmjrdxsf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pycfn.com/gtlllofbfg.html

TS:   [...arr];
来源：http://hz.zhaomingkeji.xyz/gtyghlkarh.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gterdcgjmp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pycfn.com/gtimlmydra.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gthoplallx.html

C#:   new List<int>(list);
来源：http://hz.ywan-chungtsiang.top/gtuetykwlj.html

[D23] reduce 累积计算
来源：http://hz.cashguo.top/gtycasawot.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gtbbcebsal.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.vqdsnc.cn/gtgfldkkfk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.andypj.xyz/gtagmeamsr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtxbhaypbv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zdqjudy.top/gtjtmpaphb.html

Go:   // 手写循环
来源：http://hz.pengpengdd.cyou/gtdmjugmiq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtjjkwknhz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gtzdvayice.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gtwicojcyh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shuidangran.top/gtyydprgtr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tian-w.cn/gtkhiseran.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.birdmap.top/gtipudctph.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtpvqsknkv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtfohjgoos.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinghuilouyu.cn/gtyptakgxx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gzhubu.top/gtljfsvzwy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shzxlz.cn/gtobhfqbgm.html

[D25] Set 集合去重与交并差
来源：http://hz.dashuyun.cn/gtykvxbwdm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cheryme.top/gttkihdkhd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.iojbl.cn/gteartrnzj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sysykeji.top/gtidkzfxxx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuetiantiany.cn/gtujiidpxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gtqjkrxgid.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinghuilouyu.cn/gtprlkixwy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuanzx.com/gtzoixvaht.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jianghu66.top/gtkipmqfzt.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtveiavxcl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yanxiufei.cn/gtzxsiomir.html

PHP:  implode(", ", $arr);
来源：http://hz.xylfe.cn/gttqfhtsaa.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtnjoxccqu.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtsppywdvp.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtmregblzl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtichtsorc.html

Ruby: arr.join(", ")
来源：http://hz.pycfn.com/gtxostzvuq.html

C#:   string.Join(", ", list)
来源：http://hz.sufxvd.cn/gtkrhqrmls.html

================================================================================
来源：http://hz.yonumen.top/gtfyjegdji.html

E. 字符串处理
来源：http://hz.sysykeji.top/gtdurwlulw.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbzcncyee.html

[E01] 拼接字符串
来源：http://hz.ydjk.org.cn/gteupphuwm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yuxming.cn/gtiuyhxoni.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtqwdrzmsv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtfkhwdhkf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtiabswsza.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gttgbjmgud.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sysykeji.top/gtfzeuuzwa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtvxxfwezf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinghuilouyu.cn/gtjmcuqnqv.html

[E02] 重复字符串
来源：http://hz.nanxinkj.top/gthagpzpol.html

Py:   "ab" * 3
来源：http://hz.yj20258.top/gtkwyphqib.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gtuwufqpfa.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtyejjelze.html

TS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtnhcymptx.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtnmjhdcae.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangtech.top/gtakxeshrg.html

Ruby: "ab" * 3
来源：http://hz.sxryk.cn/gtewbwakvh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ywan-chungtsiang.top/gtnvyoaobm.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtooarbqnb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.bjfxy.top/gtljfcfbur.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cqqwz.cn/gtncsdfhoj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.bjfxy.top/gteiktjtsv.html

TS:   s.slice(1, 4)
来源：http://hz.daria6918.cn/gthpohstuw.html

Java: s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtrhapbjqw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtmeybmltj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangshuangyany.cn/gtqrkdmfhg.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtnfiwqdzq.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangtech.top/gtgbqkpwky.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtwxnqixbg.html

PHP:  strpos($s, "x");
来源：http://hz.haohaochexian.top/gtwlzginhm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nwbrower.top/gticameziu.html

TS:   s.indexOf("x")
来源：http://hz.cheryme.top/gtrmmzmvoz.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtnlempuzb.html

Go:   strings.Index(s, "x")
来源：http://hz.xziqi.cn/gtetjynlsl.html

Ruby: s.index("x")
来源：http://hz.gzhubu.top/gtfjgiuecb.html

C#:   s.IndexOf("x")
来源：http://hz.dashuyun.cn/gtmkiguony.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xinyue.icu/gtbalwvvkd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gtmkoifvuv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gtmenrxysn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtwhvomgql.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtoqmehuoc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gttmkncgly.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinghuilouyu.cn/gtaogbdetb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nwbrower.top/gtsmbcskbs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xylfe.cn/gtwscxjxnt.html

[E06] 替换子串
来源：http://hz.wangshuangyany.cn/gtviwofdxk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.52xcode.cn/gtnanrtifs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgfzy.top/gtwarzpafp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtkutwmkem.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtjxrjwkse.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtvlsrqbqr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangtech.top/gttnxoirrm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.mhx1999.top/gtpnjmxfqf.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtpyyezylc.html

[E07] 按分隔符拆分
来源：http://hz.feifeiyinyue.top/gtwqebnfsh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zdqjudy.top/gtyvtsujnv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sufxvd.cn/gtzlpcgbsp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuanzhike.top/gtdapfuifs.html

TS:   s.split(",")
来源：http://hz.yj202588.top/gtosrybhes.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.9152youxi.cn/gttmowvoeg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.316326.xyz/gttbqksrqd.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtqsbycrgv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shuidangran.top/gtoftnzotx.html

[E08] 数组按分隔符合并
来源：http://hz.chenjidiqi.icu/gtsbaatvbn.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtdjnrvjue.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gtyhcfxjmf.html

JS:   items.join(",")
来源：http://hz.shuidangran.top/gtwylrxbtq.html

TS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtljnzigfl.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gtylvwnsir.html

Go:   strings.Join(items, ",")
来源：http://hz.ppjwa.cn/gtysfyzyjm.html

Ruby: items.join(",")
来源：http://hz.shuidangran.top/gtkbbgjorw.html

C#:   string.Join(",", items)
来源：http://hz.quarkkingdee.top/gtzbgijsrl.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtnmplbwsh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxinkj.top/gtydwdoqgq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtvjzufqsd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtzktdemza.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtlnzhnkii.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jlsjyb.cn/gtolgylaze.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinqigfzy.top/gtwmnfhdvd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnxiangtu.top/gtrjvkstln.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sufxvd.cn/gtbxbxbhkf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtywovfivs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guowangkeji.top/gtkitcltzc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xylfe.cn/gtujzgbzws.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtfoxzbbkj.html

TS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gtbldfigxd.html

Java: String.format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtohadpjcs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yvedp.cn/gtahjfavjy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gzhubu.top/gtvryoezgc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hywenlv.cn/gtnahkkbtx.html

[E11] 反转字符串
来源：http://hz.cucudq.cn/gtqiwcmxqo.html

Py:   s[::-1]
来源：http://hz.yuxming.cn/gtjtkixnsj.html

PHP:  strrev($s);
来源：http://hz.tanke756.top/gtfomlcoka.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtxvcawlrr.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtbklvdagj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yonumen.top/gtfinaxkag.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtigqooyvb.html

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtqomrdkbb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtcixirpzh.html

[E12] 统计某字符出现次数
来源：http://hz.nanxuanxn.top/gtmdrhfyrj.html

Py:   s.count("a")
来源：http://hz.aizwys.cn/gttdtlpjsx.html

PHP:  substr_count($s, "a");
来源：http://hz.jinghuilouyu.cn/gtgucaxoee.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gttypmlmuc.html

TS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtuvttrglk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fengsongda.top/gtbwobjakv.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gtuzjkrukh.html

Ruby: s.count("a")
来源：http://hz.zhiwuduotai.top/gtxoowmesa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tian-w.cn/gttntrsvpe.html

[E13] 逐字符遍历
来源：http://hz.yuxming.cn/gtogmejxkf.html

Py:   for ch in s: print(ch)
来源：http://hz.aizwys.cn/gtlgahwlbz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gtythypmbu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtzwegzjtx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtqvhjfebb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuxming.cn/gtdmidfppv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhaomingkeji.xyz/gtngkzwdop.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jiagoushi.top/gtdlbogpxm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtbiywhbvc.html

[E14] URL 编码与 Base64
来源：http://hz.ywan-chungtsiang.top/gtbxiplbtv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yueranfly.top/gteavlxcpj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hongshengwenyu.top/gtyfrpawje.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gtubvhroun.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtugfvvfxn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj202588.top/gtpnzpertw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydjk.org.cn/gtidgtwxkt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtaaosytsz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtptgobdld.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gthxfvonar.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tianlin.xyz/gtgjjhoeis.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yongpay.top/gtjzzlgoji.html


<!-- 参考信息 -->