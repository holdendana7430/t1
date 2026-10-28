代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtwmdusxga.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhengqikj.top/gtlipmppsl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtkhbmymqj.html

Ruby: arr.uniq
来源：http://hz.sysykeji.top/gtjdhnoaal.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gtucdmghks.html

[D16] 求和与平均值
来源：http://hz.aizwys.cn/gtuzpgslzh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtaekwmwuz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aizwys.cn/gtvxyncbqy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtlfazjrsr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtzebxgfek.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtnwyrdplz.html

Go:   // 手写循环累加
来源：http://hz.gzhubu.top/gtrtsyhazx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aizwys.cn/gtggopqxvk.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gtoslpkfjm.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtvjkbxxni.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtxfnvffod.html

PHP:  max($arr);  min($arr);
来源：http://hz.hfpthk.cn/gtipicpibu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.andypj.xyz/gtvscodrxv.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtudhmoceq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangkeji.top/gtzusjkvpn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jiagoushi.top/gthsbkduho.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gtavfsbtzj.html

C#:   list.Max();  list.Min()
来源：http://hz.wangdashe.top/gtejiqevrj.html

[D18] 扁平化嵌套数组
来源：http://hz.quarkkingdee.top/gtnhuezkip.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yongpay.top/gtffxtwwla.html

PHP:  array_merge(...$nested);
来源：http://hz.guowangkeji.top/gthgcbjgsx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtkaixkkmb.html

TS:   nested.flat();
来源：http://hz.guowangkeji.top/gtmmrflvaf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtkikdscuy.html

Go:   // 手写双层循环
来源：http://hz.chenzaomai.com/gtlzcxjcql.html

Ruby: nested.flatten
来源：http://hz.sysykeji.top/gtdbnqnrvr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtniwlcbjw.html

[D19] 按字段分组
来源：http://hz.xziqi.cn/gtbjfrdmgn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nanxuanxn.top/gtuksrhpna.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fengsongda.top/gtyxasblxe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangkeji.top/gtferqhmaj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.meibo888.top/gtjzdkwemz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuetiantiany.cn/gtwgowgjao.html

Go:   // 手写 map[string][]T
来源：http://hz.sysykeji.top/gtfmesgnyw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ppjwa.cn/gtbeyskgxf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ppjwa.cn/gtfssxppaf.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtjfbaawgc.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtogczjeoc.html

PHP:  array_count_values($arr);
来源：http://hz.ybcxt.top/gtwykcmbxz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtdifvkghh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtafwxmgub.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuanzx.com/gtarrekwbs.html

Go:   // 手写 map[T]int
来源：http://hz.nanxinkj.top/gtetljlkah.html

Ruby: arr.tally
来源：http://hz.pengpengdd.cyou/gtnikwywhh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxinkj.top/gtdesvfgya.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gtqvxpviik.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtcngpoonp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtjnftjumg.html

JS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gttqqzfsma.html

TS:   arr.includes(x)
来源：http://hz.zhijiandao.cn/gttlnnqbee.html

Java: list.contains(x)
来源：http://hz.sxryk.cn/gtatyaxvhx.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gthxhjxhtn.html

Ruby: arr.include?(x)
来源：http://hz.52xcode.cn/gtaubedsao.html

C#:   list.Contains(x)
来源：http://hz.shangyingyoupin.top/gtdcyeaann.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hongshengwenyu.top/gtolmvcwss.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtrkiporme.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtttvbdvgf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.havefunace.top/gtwqzjbyxa.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtobvqqnua.html

Java: new ArrayList<>(list);
来源：http://hz.0kj1m.cn/gtvvuvnxmy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gtvlerskky.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgufenzy.top/gtdbkuvziz.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gtemjmvvfq.html

[D23] reduce 累积计算
来源：http://hz.ydzc1.top/gtwcjcnnno.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.birdmap.top/gtkaycaxhe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtopxdocds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtuzvqrjgz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtpucurgxj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gaohongyu789.top/gtfzfkaajw.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtqljdinkp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gtvrufpybb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gteytwyidr.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuxming.cn/gtmmbnlrza.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuetiantiany.cn/gtdwxypizf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.andypj.xyz/gtiwtnaozn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gthhijwaoz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.guannengcc.top/gtidcaphmw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tianlin.xyz/gtfkitcvdl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daxiang520.top/gtckizhvge.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gttcndmhak.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yvedp.cn/gtrwvquozm.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtlhskzkqs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhongyouzk.top/gtvnqpklvc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhiwuduotai.top/gtdbvrzklw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj20258888.top/gtnyhgwwkq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtlwyaddlq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuetiantiany.cn/gteyeeudms.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gtczvklmgo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtbmstovya.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuanzhike.top/gtivcaxloz.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtcvoolpxk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigfzy.top/gtqjbecday.html

PHP:  implode(", ", $arr);
来源：http://hz.zdqjudy.top/gtjidrswyq.html

JS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtwopumgpq.html

TS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gthlalvenr.html

Java: String.join(", ", list)
来源：http://hz.yj20258888.top/gtqebzzctk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtyrbkisxx.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gtqgiubqyf.html

C#:   string.Join(", ", list)
来源：http://hz.quarkkingdee.top/gtnswwgski.html

================================================================================
来源：http://hz.andypj.xyz/gtajltthsc.html

E. 字符串处理
来源：http://hz.yj202588.top/gtqyqrapju.html

================================================================================
来源：http://hz.havefunace.top/gtvdflsvqw.html

[E01] 拼接字符串
来源：http://hz.aizwys.cn/gtthvugafd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.guannengcc.top/gtjduqpoox.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.iojbl.cn/gtqfzvmpzh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtgisdlbxu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtongkaerm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinyuanbaomall.cn/gtabazmpwf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.kuanghao11.cn/gtjyotkzly.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gaohongyu789.top/gthacoebio.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ybcxt.top/gtdwtkqbbq.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtjfpusdfo.html

Py:   "ab" * 3
来源：http://hz.mhx1999.top/gtnhadxlye.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guowangkeji.top/gtbitopwmb.html

JS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtjkhxgxkw.html

TS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtqanwtnfg.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gteorcpyys.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yangfankeji.com/gteytrnaxt.html

Ruby: "ab" * 3
来源：http://hz.yj20258888.top/gtorhbxamh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fzhhl.top/gthfseiqcb.html

[E03] 截取子串
来源：http://hz.jiagoushi.top/gtihuffnwo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgufenzy.top/gtvnesinbo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sxryk.cn/gtyrniscbm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtynnvlixm.html

TS:   s.slice(1, 4)
来源：http://hz.jianghu66.top/gtkudukixd.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtjwxekdcl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.dashuyun.cn/gtxfrsoxll.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtirtfejxr.html

C#:   s.Substring(1, 3)
来源：http://hz.iojbl.cn/gtlpgmhmce.html

[E04] 查找子串位置
来源：http://hz.hywenlv.cn/gtnhtkmyfd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.birdmap.top/gtbaiidxww.html

PHP:  strpos($s, "x");
来源：http://hz.guannengcc.top/gtojzepjzn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.iojbl.cn/gtyokdimvf.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtpjygivzh.html

Java: s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtfvbwcwmp.html

Go:   strings.Index(s, "x")
来源：http://hz.fzhhl.top/gtdlnuaciq.html

Ruby: s.index("x")
来源：http://hz.jinqigfzy.top/gtaewazhqh.html

C#:   s.IndexOf("x")
来源：http://hz.yonumen.top/gtpsvhlchn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgfzy.top/gtjblenkqn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnxiangtu.top/gtgrjtwydi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gtqtmsuine.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydjk.org.cn/gtxrnrrmdv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtvtfgagdz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtzkxoearf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhengqikj.top/gtuhcvhyjm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258.top/gthwarhhog.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.c1oappe.top/gthnhgrgvk.html

[E06] 替换子串
来源：http://hz.ydjk.org.cn/gtddlevaoq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.andypj.xyz/gthphftqfo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xingfuxueyuan.xyz/gtsyfxvyyy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gthtfxnavx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtwqwuzlkb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtenjwgtkq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.52xcode.cn/gtsefjquxn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jlsjyb.cn/gtvxkppapf.html

C#:   s.Replace("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtwjntiqii.html

[E07] 按分隔符拆分
来源：http://hz.fzhhl.top/gtonnppuwb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtwdogiaes.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sufxvd.cn/gtammgojvk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.feifeiyinyue.top/gthdjxsnny.html

TS:   s.split(",")
来源：http://hz.haohaochexian.top/gtunxqdvie.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.dianchejie.cn/gtlwkuxyli.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.aibaodan.cn/gtggmabwzg.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtjbfkugvw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtuctgdidx.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtzdbbvxxg.html

Py:   ",".join(items)
来源：http://hz.pengpengdd.cyou/gtgxnpjcxa.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gttovpzjee.html

JS:   items.join(",")
来源：http://hz.yj202588.top/gtakvqkjeh.html

TS:   items.join(",")
来源：http://hz.iojbl.cn/gtgwpuekld.html

Java: String.join(",", items)
来源：http://hz.sufxvd.cn/gtcevqszny.html

Go:   strings.Join(items, ",")
来源：http://hz.fzhhl.top/gtrposhece.html

Ruby: items.join(",")
来源：http://hz.aibaodan.cn/gtfywfdplp.html

C#:   string.Join(",", items)
来源：http://hz.jinghuilouyu.cn/gtabobxyto.html

[E09] 去除所有空白字符
来源：http://hz.sweek.top/gtsxhmzart.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cdnleiting.top/gtvwqlykvd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gthxjovgmq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtbjfiwcce.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtciikgfdu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxuanxn.top/gtgvehszbw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtsxsldcjp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhaomingkeji.xyz/gtffhvhaqu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.svipenyu.cn/gtlqbwqitg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.meibo888.top/gtewokvfbt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxinkj.top/gtlnxuhkmo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cqqwz.cn/gtwuwfxmfk.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtiqlgvygf.html

TS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtfvxelqif.html

Java: String.format("%03d", 7)
来源：http://hz.ybcxt.top/gtqtkvegml.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtulnymvdd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtyalnkhkp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigfzy.top/gtbudslnvl.html

[E11] 反转字符串
来源：http://hz.svipenyu.cn/gtugjzxvuk.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtmhqnhokb.html

PHP:  strrev($s);
来源：http://hz.sufxvd.cn/gtxrlgeoah.html

JS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtmkkyswcj.html

TS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtogkksusx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhijiandao.cn/gtteaikgxi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hongshengwenyu.top/gtzjyeaamh.html

Ruby: s.reverse
来源：http://hz.hongshengwenyu.top/gtllsaejwk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gthkseczcj.html

[E12] 统计某字符出现次数
来源：http://hz.aizwys.cn/gtzuvinsez.html

Py:   s.count("a")
来源：http://hz.yj20258.top/gtwxngrgeb.html

PHP:  substr_count($s, "a");
来源：http://hz.gaohongyu789.top/gtxpfswztn.html

JS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gttnrzndsq.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtwiisqait.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnqzz.top/gtgbrisitc.html

Go:   strings.Count(s, "a")
来源：http://hz.yanxiufei.cn/gtyqbtbhmh.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtrsopyhte.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daria6918.cn/gtqlmkbjay.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gticbxufbl.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258888.top/gteebpewes.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.birdmap.top/gtkbsoojdp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtkhsuqcxx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtpqybvxzv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhongyouzk.top/gtwclrulun.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yvedp.cn/gtrfiepjfw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.smart0.xyz/gtqrmzostd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinyuanbaomall.cn/gtcmtlwoad.html

[E14] URL 编码与 Base64
来源：http://hz.ydjk.org.cn/gtfmbwmhlm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yonumen.top/gttniiefap.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtzbijeprr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtdtfnqwsb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pengpengdd.cyou/gtbtyeoruj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zycfv.cn/gtdhxorjnc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.c1oappe.top/gtifxwkklg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinghuilouyu.cn/gtmcpsrfzp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gtaasphxsd.html

[E15] HTML 转义 / 反转义
来源：http://hz.sufxvd.cn/gtvqwueyfy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xziqi.cn/gtffzdkxjq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhijiandao.cn/gtbakhboye.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ybcxt.top/gtbzfbeikq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gthxtzdaaz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guannengcc.top/gtvcufeuhh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtqiepgyyg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhengqikj.top/gthtrievqn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtfptlorry.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtziurpzji.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigufen.top/gtnyhoxxyq.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtiquoxutp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtniqxmgod.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtuhilslrt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gzhubu.top/gtszpmxfbr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hywenlv.cn/gtwxxcscpo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxinkj.top/gtffibllwe.html

C#:   1234567.ToString("N0")
来源：http://hz.yueranfly.top/gtzisrhwol.html

[E17] 首字母大写
来源：http://hz.shanyushiyangtech.top/gtvfbshmys.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ppjwa.cn/gtdnllrzax.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ivvv.top/gtuqyorbsc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gtlhbjpggq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ybcxt.top/gtisjebmqs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gtjdfszvfr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gthtvcbxrn.html

Ruby: s.capitalize
来源：http://hz.hammf.cn/gtlwszytfr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gthgwkidld.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gtssebioze.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.smart0.xyz/gtpuyztyys.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtdgdihrlp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtbgtmurzc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtcziuavxv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shzxlz.cn/gtkhogzheb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtprvmkfrb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tanke756.top/gtlaonrqme.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangdashe.top/gtxaisvact.html

[E19] 多行文本按行拆分
来源：http://hz.gogol.net.cn/gtvxdrjzpu.html

Py:   s.splitlines()
来源：http://hz.redwolf501.top/gtrllnlpsc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtvdemuhan.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtrxwzyixc.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtzjlcagvk.html

Java: s.lines().toList()
来源：http://hz.9152youxi.cn/gtgpieornj.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtagxrcivv.html

Ruby: s.lines
来源：http://hz.xinyue.icu/gtnsfvvggs.html

C#:   s.Split('\n')
来源：http://hz.xuanzx.com/gteqstpjni.html

[E20] 判断字符串是否为空
来源：http://hz.gogol.net.cn/gthbcvfjcs.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtubkziyvr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yanxiufei.cn/gtabdykynn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.andypj.xyz/gtztginikx.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtmikmpwbd.html

Java: if (s.isEmpty()) {}
来源：http://hz.pycfn.com/gtulgbvvoy.html

Go:   if s == "" {}
来源：http://hz.xuanzx.com/gtroruqnwa.html

Ruby: if s.empty?
来源：http://hz.zycfv.cn/gtiifzfins.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gtdufzseqr.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtksxnbeld.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtsvrnswyz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sufxvd.cn/gtxaorscoy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtjboqygjx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtnfyjnlbv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtdhaplpar.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gtmcemmllb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guannengcc.top/gtngxietld.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tian-w.cn/gtqcfcwqdr.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258.top/gtbrkthytt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigufen.top/gtdpwxpvtu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtcpmmclkj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtsoalilwe.html


<!-- 参考信息 -->