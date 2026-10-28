代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.svipenyu.cn/gtwinbxfrf.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtvuusbnmm.html

Go:   slices.Reverse(arr)
来源：http://hz.svipenyu.cn/gtiqhgumtk.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtjowlqaqe.html

C#:   list.Reverse();
来源：http://hz.hysaishi.cn/gtzkxcdipn.html

[D12] 查找元素下标
来源：http://hz.pengpengdd.cyou/gttikrieep.html

Py:   arr.index(x);  x in arr
来源：http://hz.haohaochexian.top/gtdbcblcgg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sxryk.cn/gtfqpbdbwq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtrsvywxka.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtozjulcsm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yvedp.cn/gtqlxgrshe.html

Go:   slices.Index(arr, x)
来源：http://hz.jinqigufen.top/gtlqvzhwzf.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtoyyrqdhe.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtljxbuzyt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.c1oappe.top/gtkupznhvw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gtowvtojml.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuetiantiany.cn/gttaevvuki.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtqjwqrumr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hammf.cn/gtgiivooda.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gtzszvhtzp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cucudq.cn/gtevnqwgaw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtzojvrsys.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtinjxbcgl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yonumen.top/gtnmrgoqtp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtrpdwypwr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nwbrower.top/gtgwzlzpzw.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtjnbltdnl.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gttklrnnqe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tian-w.cn/gtuwselocw.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gthklzyxzd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtaqrdvhqj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yueranfly.top/gtwifpfwer.html

[D15] 去重
来源：http://hz.feifeiyinyue.top/gtlgpolvip.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtxkmgcaui.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtpondlebf.html

JS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtqspwjaze.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtnnkxpboh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shangyingyoupin.top/gtzexifbry.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yongpay.top/gtftjsnuzn.html

Ruby: arr.uniq
来源：http://hz.quarkkingdee.top/gtyxgrbcpe.html

C#:   list.Distinct().ToList()
来源：http://hz.zhijiandao.cn/gtcgwedige.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gtfianekpy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.svipenyu.cn/gtwsrzutya.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtvzaozumo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtvewyqdhk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gtyuyyotwt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jianghu66.top/gtrstaezxj.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtmsrbrfxt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtxjyowavg.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxinkj.top/gtgmqeqyee.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtwwxwbiwf.html

Py:   max(arr);  min(arr)
来源：http://hz.chenjidiqi.icu/gthomghbdk.html

PHP:  max($arr);  min($arr);
来源：http://hz.gotoacloud.top/gtzhajtjiv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtvrzkskzr.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtkzsitjqg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gtnohawyjc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jyoumei.cn/gtnbosyhnb.html

Ruby: arr.max;  arr.min
来源：http://hz.chenlongwang.top/gtbfzfsevu.html

C#:   list.Max();  list.Min()
来源：http://hz.dianchejie.cn/gtyftydtva.html

[D18] 扁平化嵌套数组
来源：http://hz.guowangkeji.top/gtsktjbdzt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhaomingkeji.xyz/gtbelpokpc.html

PHP:  array_merge(...$nested);
来源：http://hz.zhixingplan.top/gtvaicnohj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.c1oappe.top/gtpdosntnn.html

TS:   nested.flat();
来源：http://hz.aizwys.cn/gtfdefhwec.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hammf.cn/gtklwisrvh.html

Go:   // 手写双层循环
来源：http://hz.feifeiyinyue.top/gtgiupqwub.html

Ruby: nested.flatten
来源：http://hz.haohaochexian.top/gtpxyjpwmq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj202588.top/gtkhxvgunq.html

[D19] 按字段分组
来源：http://hz.gaohongyu789.top/gtztkhefzp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sufxvd.cn/gtvdxvtvmv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydzc1.top/gtxmthpkac.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yanxiufei.cn/gtxygjvcxd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtgfaumpyz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenjidiqi.icu/gtqprvddlo.html

Go:   // 手写 map[string][]T
来源：http://hz.sufxvd.cn/gtbkfmxfrw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daxiang520.top/gtkjkrkstk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtdvkmdqvo.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtqfcxbvdk.html

Py:   Counter(arr)
来源：http://hz.yj20258.top/gtcrvaigqy.html

PHP:  array_count_values($arr);
来源：http://hz.mhx1999.top/gtqpqjjyfr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gteqoozlfg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtohpjhdls.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cqqwz.cn/gtycrndgiw.html

Go:   // 手写 map[T]int
来源：http://hz.yuxming.cn/gtdjyiekqk.html

Ruby: arr.tally
来源：http://hz.ppjwa.cn/gtkppkshxk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.haohaochexian.top/gttfbmkokc.html

[D21] 判断是否包含某元素
来源：http://hz.0kj1m.cn/gtvcbuwyom.html

Py:   x in arr
来源：http://hz.hnqzz.top/gtuuzlyxib.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gthunwqjuu.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtvyhdspvw.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtskfjghlm.html

Java: list.contains(x)
来源：http://hz.zhengqikj.top/gtggmwmjzo.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenlongwang.top/gthqglpczm.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtdsffnibs.html

C#:   list.Contains(x)
来源：http://hz.shzxlz.cn/gtvoquryzw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.quarkkingdee.top/gtxewvejal.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guannengcc.top/gtpiiftulg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cucudq.cn/gtsoohqtcz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daria6918.cn/gtbjvzacts.html

TS:   [...arr];
来源：http://hz.zdqjudy.top/gtvkgcqtof.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gtumnguclv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.svipenyu.cn/gtzpmclmlt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtstokdjme.html

C#:   new List<int>(list);
来源：http://hz.zdqjudy.top/gtypsvtkea.html

[D23] reduce 累积计算
来源：http://hz.sweek.top/gtgfowkkke.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtbvphiopn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ivvv.top/gthdirhjgo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtcouqiuss.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.bjfxy.top/gtmdcugtjy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jiagoushi.top/gtqeifspbg.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtvczocurn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhijiandao.cn/gtdshyhlpt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtwiixcibz.html

[D24] 字典 / Map 基本操作
来源：http://hz.haohaochexian.top/gtposlaxsc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.andypj.xyz/gtsvqtkmnb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtctjkcldd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtpiskybdh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cdnleiting.top/gtdabvyedl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hysaishi.cn/gthoiqlklv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhoulong.xyz/gtidgpazdq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.iojbl.cn/gtxlacnqbp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gthfsguyyt.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtdtiojwrw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gtkhvnjfoj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tian-w.cn/gtljwylokh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shuidangran.top/gtolodnmmz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuanzx.com/gthnmattmv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.bjfxy.top/gtencvlxgx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.kuanghao11.cn/gtcxsozxbo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gtjhhitwqs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtzlsvpqnk.html

[D26] 数组转字符串
来源：http://hz.wangdashe.top/gtcnspvcfr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xinyue.icu/gtccadpsrc.html

PHP:  implode(", ", $arr);
来源：http://hz.hfpthk.cn/gtmmfddoyf.html

JS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtfemqcyms.html

TS:   arr.join(", ")
来源：http://hz.hammf.cn/gtfqjfxxcg.html

Java: String.join(", ", list)
来源：http://hz.fengsongda.top/gtxdppmmbq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.pengpengdd.cyou/gtdpegaidc.html

Ruby: arr.join(", ")
来源：http://hz.ybcxt.top/gtfflqegui.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gttzklulav.html

================================================================================
来源：http://hz.xylfe.cn/gtzachtotj.html

E. 字符串处理
来源：http://hz.vqdsnc.cn/gtlzcccnnv.html

================================================================================
来源：http://hz.yuanzhike.top/gtchziqgrt.html

[E01] 拼接字符串
来源：http://hz.zhongyouzk.top/gtswjznyfw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ppjwa.cn/gtoppzcrvb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.snrcjt.cn/gtszqkstqy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtchryhxqi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtacwsfbdb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydjk.org.cn/gtthvtezzu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daria6918.cn/gtcgobtkmy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ehwqpu.com/gtcvahmkrl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnqzz.top/gtgexcoemd.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gtarrhtllj.html

Py:   "ab" * 3
来源：http://hz.daria6918.cn/gtimxwkuhc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gtorpzktez.html

JS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtugfnmeji.html

TS:   "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtbexvwnax.html

Java: "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtqrjpcfbm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtitdgvgcu.html

Ruby: "ab" * 3
来源：http://hz.snrcjt.cn/gtvwvxjurh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhongyouzk.top/gtxgrnslzt.html

[E03] 截取子串
来源：http://hz.fengsongda.top/gtonllmbcm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangshuangyany.cn/gtcpmzijru.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xylfe.cn/gtoyocugdb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sxryk.cn/gtazalhalb.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtjgbgcebz.html

Java: s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtehncwexs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtssrnkbfb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.kuanghao11.cn/gtzjkzxipn.html

C#:   s.Substring(1, 3)
来源：http://hz.sufxvd.cn/gtypqomwap.html

[E04] 查找子串位置
来源：http://hz.shuidangran.top/gtoxmfbcta.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtjcdinysy.html

PHP:  strpos($s, "x");
来源：http://hz.aibaodan.cn/gtpfkigjqn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtlcgqvjwq.html

TS:   s.indexOf("x")
来源：http://hz.ppjwa.cn/gtuvqiofst.html

Java: s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtqlrmovgh.html

Go:   strings.Index(s, "x")
来源：http://hz.hammf.cn/gtcaczqjwf.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gtqzplzdvu.html

C#:   s.IndexOf("x")
来源：http://hz.haohaochexian.top/gtbqeyzqdl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gzhubu.top/gtrnrhlnkp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aibaodan.cn/gtwflpsbak.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtbemygzcc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtlpvzukni.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shangyingyoupin.top/gtgodlijxg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gtcsyxzfnx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.bjfxy.top/gtonzjiynl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tian-w.cn/gtjbvndbsb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhoulong.xyz/gtcobciwbi.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtegctvzjo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xylfe.cn/gtwggyzijj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hywenlv.cn/gtqhldklff.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtwrxszfyk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtuqlfvfwm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtyjwirxxy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gtqnziqmuc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hywenlv.cn/gtdmiyrqto.html

C#:   s.Replace("a", "b")
来源：http://hz.xylfe.cn/gtyohiwief.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gtsjwdqjrz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guowangkeji.top/gtegyzhdqr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shangyingyoupin.top/gtzgyoewfl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aibaodan.cn/gtydtozwlf.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtdengrilc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nwbrower.top/gtswzzqpnp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxuanxn.top/gtlahzitti.html

Ruby: s.split(",");  s.split
来源：http://hz.pengpengdd.cyou/gtilqzmhmd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gtabumgqpr.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtlwwtnfra.html

Py:   ",".join(items)
来源：http://hz.iojbl.cn/gtibhudgiy.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtckzgjwrx.html

JS:   items.join(",")
来源：http://hz.yj202588.top/gtbrhdfhcj.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtcprzawon.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtmeayagdx.html

Go:   strings.Join(items, ",")
来源：http://hz.ivvv.top/gtrcfqrbhs.html

Ruby: items.join(",")
来源：http://hz.9152youxi.cn/gtsvjvpwby.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gttqwdurjf.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtwquuxlmy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gtkisqnpzf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtizjplscq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yvedp.cn/gtgoprdcao.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.smart0.xyz/gtoawxyclz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ehwqpu.com/gtlqmccsxw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dianchejie.cn/gtwtrxlfeb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.quarkkingdee.top/gtfeepxtnv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhongyouzk.top/gtxjtxleqq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.iojbl.cn/gtojjhxyjd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtpawbmqoq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cucudq.cn/gtkcxrzhhy.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtmbkkokgm.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtjtiwnsgk.html

Java: String.format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtfhgdxhml.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gtyeeumrfp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtbiiwkbcf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sweek.top/gtwnnniplp.html

[E11] 反转字符串
来源：http://hz.c1oappe.top/gtencopmik.html

Py:   s[::-1]
来源：http://hz.andypj.xyz/gtmocdjlwk.html

PHP:  strrev($s);
来源：http://hz.andypj.xyz/gttesibstt.html

JS:   [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtyexojuaj.html

TS:   [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtkvqthoou.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yueranfly.top/gtaucvndnz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jyoumei.cn/gtwmlqrgsd.html

Ruby: s.reverse
来源：http://hz.nanxuanxn.top/gttzsewinc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtptonoshc.html

[E12] 统计某字符出现次数
来源：http://hz.zdqjudy.top/gtwypnhpcb.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gthjhxvvfn.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtwsvxvxhf.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtxfftdpjl.html

TS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtsgwtkjjl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.0kj1m.cn/gtdnxhhtno.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtdwljenha.html

Ruby: s.count("a")
来源：http://hz.yvedp.cn/gtynfdixxc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gtddyzsgdu.html

[E13] 逐字符遍历
来源：http://hz.jinqigufen.top/gtufhebonw.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gtpwqtdxrg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yonumen.top/gtmtinzcep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtabvqrnbk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtjwzdjdxv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtegovgeuh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtzttcazlb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gttjprksao.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gtaxzzaysa.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtsfyysdyo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtcyrloqgf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dianchejie.cn/gtuloulglq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.bjfxy.top/gtsvizcjbz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.wangdashe.top/gttndilkmk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtrtmydklb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtwxmnfmii.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuanzx.com/gtxcclxlon.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtlbprkjrp.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuxming.cn/gtsxqmrzmi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtkknjuxua.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhengqikj.top/gtndeafgxy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xziqi.cn/gtzzagvshl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gzhubu.top/gtvemmxncv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zdqjudy.top/gtucfrnfqq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtwypkspvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtkqaauxho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cucudq.cn/gttksyocxe.html

[E16] 数字千分位
来源：http://hz.zhongyouzk.top/gtpsmuuhrn.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtcluesxwp.html

PHP:  number_format(1234567);
来源：http://hz.yueranfly.top/gtkdtsfpbd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtvflbxrfb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtxxmrukam.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtdizuirzz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sweek.top/gtzulrkgkh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.vqdsnc.cn/gtuealggei.html

C#:   1234567.ToString("N0")
来源：http://hz.yuxming.cn/gtfwxgcafk.html

[E17] 首字母大写
来源：http://hz.pycfn.com/gtxrlrvmtm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxuanxn.top/gtwjciljqv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtpjcjcudt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gttiikqqtz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtoivkozlo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yanxiufei.cn/gtohvxclcc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtvfplxbkd.html

Ruby: s.capitalize
来源：http://hz.fengsongda.top/gtyjklqrae.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zycfv.cn/gtobobavaj.html

[E18] 模板占位符替换
来源：http://hz.zhixingplan.top/gtdzdvqnkz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtozuwlapz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gttmsbyvgq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtowlicjgw.html


<!-- 参考信息 -->