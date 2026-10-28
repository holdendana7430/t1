代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.yuanzhike.top/gtkaxemdas.html

Java: Collections.reverse(list);
来源：http://hz.gzhubu.top/gtrzsvnsgl.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgufenzy.top/gttvgsssee.html

Ruby: arr.reverse
来源：http://hz.ydzc1.top/gtfxilmcoz.html

C#:   list.Reverse();
来源：http://hz.zhixingplan.top/gtxgxxwcit.html

[D12] 查找元素下标
来源：http://hz.yonumen.top/gtnojubnme.html

Py:   arr.index(x);  x in arr
来源：http://hz.gzhubu.top/gtyipqscgh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nwbrower.top/gtndidftko.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtljeqwmzh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtwgpgsefc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtdzoiwuid.html

Go:   slices.Index(arr, x)
来源：http://hz.ydzc1.top/gtyrdrnjtb.html

Ruby: arr.index(x)
来源：http://hz.ywan-chungtsiang.top/gtnnjqyrht.html

C#:   list.IndexOf(x);
来源：http://hz.yvedp.cn/gtcktxskfd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtewyvbsfe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.smart0.xyz/gtoawwzakf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xziqi.cn/gtgyqsevga.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtqtyqlruk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangshuangyany.cn/gtizgwladm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258.top/gtzkgdtohn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.haohaochexian.top/gtmhlkamia.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhixingplan.top/gtkudwifzf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgufenzy.top/gtudtuydtt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guannengcc.top/gtswlxgetg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hfpthk.cn/gtmhcpytlq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtzoeonbph.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtewkpxebv.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtskgqbkmw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.bjfxy.top/gtyviryziz.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtspvmtmqn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuanzhike.top/gthknwqnas.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.guowangkeji.top/gtvzrmpvug.html

[D15] 去重
来源：http://hz.c1oappe.top/gtbyrksgeb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtytimsvtc.html

PHP:  array_unique($arr);
来源：http://hz.fzhhl.top/gtygtrdzld.html

JS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gthplanjsx.html

TS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtsxlreghw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zycfv.cn/gtowtxvucm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhiwuduotai.top/gtrkahijmy.html

Ruby: arr.uniq
来源：http://hz.zdqjudy.top/gtnaoxynxr.html

C#:   list.Distinct().ToList()
来源：http://hz.snrcjt.cn/gtizzlqtxv.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gtdusvsipw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gotoacloud.top/gtdsrwqose.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtpxosvzlk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtspdoahjq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtauahctzn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dianchejie.cn/gteqljnctt.html

Go:   // 手写循环累加
来源：http://hz.daria6918.cn/gtvdsjojpt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fzhhl.top/gtbrdglpyt.html

C#:   list.Sum();  list.Average()
来源：http://hz.ivvv.top/gtamgeyevl.html

[D17] 最大值与最小值
来源：http://hz.ybcxt.top/gtexqkyknf.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtacwjmusk.html

PHP:  max($arr);  min($arr);
来源：http://hz.jiagoushi.top/gtqvfgrmqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sysykeji.top/gtaxvzxiwq.html

TS:   Math.max(...arr);
来源：http://hz.feifeiyinyue.top/gtcbhzdiqq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yangfankeji.com/gtfvsvchoc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtitulwtdm.html

Ruby: arr.max;  arr.min
来源：http://hz.snrcjt.cn/gtuqffcwzu.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtidlygrfe.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtbfyffzyk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.mhx1999.top/gtwebpiurw.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtfnicxloy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sufxvd.cn/gtgntmnlvd.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gtldoxafwi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gtivufnglm.html

Go:   // 手写双层循环
来源：http://hz.sweek.top/gtjgogijse.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtellqwcqs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.0kj1m.cn/gtprxmriif.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtdnxfhisd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sweek.top/gtrllketqt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sxryk.cn/gtbkzfpakd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gtshyykgqv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtfnqvlzsk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zdqjudy.top/gtkcnvrpjz.html

Go:   // 手写 map[string][]T
来源：http://hz.redwolf501.top/gtlnwwymyk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.9152youxi.cn/gtckxmzuaq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenjidiqi.icu/gtfkeunxmm.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gtonjwoqui.html

Py:   Counter(arr)
来源：http://hz.cucudq.cn/gtilasvwmu.html

PHP:  array_count_values($arr);
来源：http://hz.cucudq.cn/gtgymnyuzm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtmfecntpq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtbvgroqap.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258888.top/gtytfhdgfh.html

Go:   // 手写 map[T]int
来源：http://hz.gaohongyu789.top/gtxgwvrvmq.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtmvjuagee.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangshuangyany.cn/gtsaxbvfwj.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtlojqcmkq.html

Py:   x in arr
来源：http://hz.snrcjt.cn/gtjaqlobum.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xinyue.icu/gtbdpjpifb.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtgqabvhay.html

TS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtjbiafrhv.html

Java: list.contains(x)
来源：http://hz.ppjwa.cn/gtiyxyujvy.html

Go:   slices.Contains(arr, x)
来源：http://hz.ehwqpu.com/gthsdhyjiv.html

Ruby: arr.include?(x)
来源：http://hz.hnqzz.top/gtigjaxtbj.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtmhmzglns.html

[D22] 复制数组（避免共享引用）
来源：http://hz.316326.xyz/gtefcqzzxh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtsuzrjipa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daria6918.cn/gtkcywvvsa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenjidiqi.icu/gtiovgopbb.html

TS:   [...arr];
来源：http://hz.tanke756.top/gtumjocjwi.html

Java: new ArrayList<>(list);
来源：http://hz.gzhubu.top/gtfokzwele.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gtqxxiabsk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtigikceee.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangtech.top/gtqvujnmgp.html

[D23] reduce 累积计算
来源：http://hz.yj20258.top/gtiocbdena.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hammf.cn/gtvttnfenn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtdxoimloh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtqminktdt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtnvlwsxxx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtguhcnfzn.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtfmlhguqe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pycfn.com/gtxygxviyo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cqqwz.cn/gtnihfylpp.html

[D24] 字典 / Map 基本操作
来源：http://hz.svipenyu.cn/gtkonafqyg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ehwqpu.com/gtwanafvwu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtybxedeqg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydzc1.top/gttvvtkyfv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhixingplan.top/gtyzhvzsmm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhoulong.xyz/gtgfstljbe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhaomingkeji.xyz/gtjqlnuvvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.iojbl.cn/gtxzbxmzyt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tian-w.cn/gtucvvkojg.html

[D25] Set 集合去重与交并差
来源：http://hz.vqdsnc.cn/gtpxqeqnbe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.aizwys.cn/gttpizmvag.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtbrfrobwn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenjidiqi.icu/gtqrxqablz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258.top/gtplnfizuw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtqbgpewve.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pengpengdd.cyou/gtxallbapa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.redwolf501.top/gtcrqrgpag.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aibaodan.cn/gtluuzazml.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtwkniusal.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtwatqnzyk.html

PHP:  implode(", ", $arr);
来源：http://hz.dianchejie.cn/gtasrzlnju.html

JS:   arr.join(", ")
来源：http://hz.jlsjyb.cn/gtslgfjggt.html

TS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtkolbckda.html

Java: String.join(", ", list)
来源：http://hz.wangdashe.top/gtanlhukqn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yonumen.top/gtplfghofh.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gttylvltbd.html

C#:   string.Join(", ", list)
来源：http://hz.pycfn.com/gtjpalwvxi.html

================================================================================
来源：http://hz.dianchejie.cn/gtzeqqnzpu.html

E. 字符串处理
来源：http://hz.sysykeji.top/gtifrhdzwc.html

================================================================================
来源：http://hz.guannengcc.top/gtzwzqwovt.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtxaqfatsf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtrscampgs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangtech.top/gtsaniuvlf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhoulong.xyz/gtlkpeizmn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gtamdpzfyc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhoulong.xyz/gtwgenujtq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtpapmjpzz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hfpthk.cn/gtyrnsuuji.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydjk.org.cn/gtxluatjue.html

[E02] 重复字符串
来源：http://hz.haohaochexian.top/gttzzygoju.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gtahjugbpe.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jqgfzy.top/gtcyrtaght.html

JS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtjoiqdwik.html

TS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtvhsakefq.html

Java: "ab".repeat(3)
来源：http://hz.tanke756.top/gtnwnzohwm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cheryme.top/gtkmvhkqdq.html

Ruby: "ab" * 3
来源：http://hz.ydzc1.top/gtpzbwkwlx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jiagoushi.top/gtioygacje.html

[E03] 截取子串
来源：http://hz.tian-w.cn/gtrwjwpquv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yongpay.top/gtbdkrcwbv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dianchejie.cn/gtiienzwge.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtvzlkygwy.html

TS:   s.slice(1, 4)
来源：http://hz.sufxvd.cn/gtylqgbcpr.html

Java: s.substring(1, 4)
来源：http://hz.ppjwa.cn/gteqxmgpwd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gtzkevoacw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.mhx1999.top/gttmjvwxpm.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtgszuywkq.html

[E04] 查找子串位置
来源：http://hz.yueranfly.top/gtfggxjxfo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shangyingyoupin.top/gtqbghvyqz.html

PHP:  strpos($s, "x");
来源：http://hz.chenlongwang.top/gthgiiladi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pycfn.com/gtxzlnlbtu.html

TS:   s.indexOf("x")
来源：http://hz.nwbrower.top/gtmkqfjsai.html

Java: s.indexOf("x")
来源：http://hz.nwbrower.top/gtvbjiywhz.html

Go:   strings.Index(s, "x")
来源：http://hz.yueranfly.top/gtledemdts.html

Ruby: s.index("x")
来源：http://hz.pycfn.com/gtntuyvxnf.html

C#:   s.IndexOf("x")
来源：http://hz.redwolf501.top/gtjujabmll.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zdqjudy.top/gtmtrisobj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenzaomai.com/gtgvwmyyzy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xziqi.cn/gtqdxszmwh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gtvoplflpw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hongshengwenyu.top/gteidhjksc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gteawwbcss.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.kuanghao11.cn/gtzsgldwaz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jianghu66.top/gtewiqylis.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ybcxt.top/gtlupniclv.html

[E06] 替换子串
来源：http://hz.ydjk.org.cn/gtcgfjimoh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gttujdivlw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.birdmap.top/gtbogznrid.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtboygzuvf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtrsqzvsee.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gteikxjytz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.vqdsnc.cn/gtfshrohdt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xinyue.icu/gtetfmbjon.html

C#:   s.Replace("a", "b")
来源：http://hz.sysykeji.top/gtaixfoqej.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtuedyniqr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtxixfxple.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.0kj1m.cn/gtuziqmjgp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtfzhqvfje.html

TS:   s.split(",")
来源：http://hz.shanyushiyangkeji.top/gtdkycqbtj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.meibo888.top/gtqrfoildu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zdqjudy.top/gthfwwmomo.html

Ruby: s.split(",");  s.split
来源：http://hz.cqqwz.cn/gtuqdervkr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydjk.org.cn/gtmvgnfglz.html

[E08] 数组按分隔符合并
来源：http://hz.yonumen.top/gtedayiyyd.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtlxdiuyqu.html

PHP:  implode(",", $items);
来源：http://hz.bjfxy.top/gtlewojcfk.html

JS:   items.join(",")
来源：http://hz.iojbl.cn/gtybvwdbmi.html

TS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtqcbunxdg.html

Java: String.join(",", items)
来源：http://hz.sysykeji.top/gtywvaiebn.html

Go:   strings.Join(items, ",")
来源：http://hz.vqdsnc.cn/gtgbvhxrdn.html

Ruby: items.join(",")
来源：http://hz.svipenyu.cn/gtnwjzpluj.html

C#:   string.Join(",", items)
来源：http://hz.zhijiandao.cn/gtixcbpwhm.html

[E09] 去除所有空白字符
来源：http://hz.mhx1999.top/gtchiqppcw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtmmszswti.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj202588.top/gtzfsanzhn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtujivhtyt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gtxovypdut.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtgrnwzqut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ybcxt.top/gtctotxuub.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuanzx.com/gtjgistclw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.meibo888.top/gtvrolfovx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dashuyun.cn/gtocbwpyaa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.9152youxi.cn/gtbeatgufl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fzhhl.top/gtzvnfryfg.html

JS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtrgsobtcd.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtbpyolgpt.html

Java: String.format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtyelmqvfh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtjqurydyo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guannengcc.top/gtryqgzxsv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cqqwz.cn/gtwesrvgcq.html

[E11] 反转字符串
来源：http://hz.guowangkeji.top/gtgpadyzto.html

Py:   s[::-1]
来源：http://hz.guannengcc.top/gtzessxbtr.html

PHP:  strrev($s);
来源：http://hz.cucudq.cn/gtcecknros.html

JS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtvyihphwc.html

TS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gttevvdimd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ywan-chungtsiang.top/gtzztipyjv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtbyssqdkj.html

Ruby: s.reverse
来源：http://hz.chenjidiqi.icu/gtrvmczmus.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtywgpknfd.html

[E12] 统计某字符出现次数
来源：http://hz.wangdashe.top/gtnkmxsysv.html

Py:   s.count("a")
来源：http://hz.tian-w.cn/gtqxdwdkmr.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gthdargfcl.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtpsofafig.html

TS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtwiqofmxf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gtklnjwcbn.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtityueomm.html

Ruby: s.count("a")
来源：http://hz.yuanzhike.top/gtfjtydnit.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtzvxkxaxs.html

[E13] 逐字符遍历
来源：http://hz.hnqzz.top/gtbjiezpky.html

Py:   for ch in s: print(ch)
来源：http://hz.fengsongda.top/gthblcrnhg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tianlin.xyz/gtmghpnbjq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtszypmsfd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtncgntugk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtblunencj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ydzc1.top/gtpxawdyto.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxuanxn.top/gtkzwcctsd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dashuyun.cn/gtqpcgkwxd.html

[E14] URL 编码与 Base64
来源：http://hz.daxiang520.top/gtwskjdpmz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtkicpsmae.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgufenzy.top/gtryqrsyhc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtnfobybsn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtnsufrwrn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtomovffek.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dashuyun.cn/gtfcaazfee.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtsuytivey.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.iojbl.cn/gtzcrnvnun.html

[E15] HTML 转义 / 反转义
来源：http://hz.jiagoushi.top/gtlegtmraj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jiagoushi.top/gtlamyswrf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnqzz.top/gtfixthzyx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gogol.net.cn/gtfwptlogm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.meibo888.top/gtqghqekdw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guowangkeji.top/gtsaohlzka.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhixingplan.top/gtccrqojti.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hongshengwenyu.top/gtnskaqfdm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtpgzdobzh.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtedqsayxv.html

Py:   f"{1234567:,}"
来源：http://hz.gogol.net.cn/gtxnwyljqb.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtucppzkuh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gttjjtxsei.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtsecazpci.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuanzx.com/gtafhehnzo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shzxlz.cn/gtgorrpfux.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuanzhike.top/gtqnjkdwhq.html

C#:   1234567.ToString("N0")
来源：http://hz.hfpthk.cn/gtdzfwnwfk.html

[E17] 首字母大写
来源：http://hz.yuxming.cn/gtzopudsji.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.c1oappe.top/gtvpuqthht.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gtgjffawhj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtntlrzslw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gtwmztcavg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtwkmrvmjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gtpezhdoxi.html

Ruby: s.capitalize
来源：http://hz.xziqi.cn/gtwxpzobls.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtkdzoqghz.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gtvdnzbqxy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cqqwz.cn/gtekvxtmoo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gogol.net.cn/gtwmllynkz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtqakavlch.html


<!-- 参考信息 -->