代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daria6918.cn/gtharzuhua.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.316326.xyz/gtkhxisjzw.html

JS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtjnammhnf.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtyaoblbss.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydjk.org.cn/gttjzcxtmd.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtxobzxoiy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xziqi.cn/gtydayhtmi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtureqeago.html

[D15] 去重
来源：http://hz.dashuyun.cn/gtuirrukcz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtebbmbvmw.html

PHP:  array_unique($arr);
来源：http://hz.aizwys.cn/gtrmrbqbyf.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtpogpttgy.html

TS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtzsxdomxg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.quarkkingdee.top/gtshcdxwyq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xinyue.icu/gtmulytnfw.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtaxojvslw.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258888.top/gtwtfzgvwt.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtullbvkyq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xuanzx.com/gtfrdgmrel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.iojbl.cn/gticizrcwv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtrdyhwrhv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtwolfpypn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ehwqpu.com/gttafalfzg.html

Go:   // 手写循环累加
来源：http://hz.feifeiyinyue.top/gtqmpqcmlq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cheryme.top/gtleqwxvcv.html

C#:   list.Sum();  list.Average()
来源：http://hz.52xcode.cn/gtwboxyiet.html

[D17] 最大值与最小值
来源：http://hz.yj20258888.top/gtbxpvllwq.html

Py:   max(arr);  min(arr)
来源：http://hz.ybcxt.top/gtamteuzts.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gtmlgijiuo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.smart0.xyz/gtjlbfkpxs.html

TS:   Math.max(...arr);
来源：http://hz.hysaishi.cn/gtmdhnfhfc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtihisawvr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zdqjudy.top/gtiakmzhvx.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gttetbbkax.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtsacicjcq.html

[D18] 扁平化嵌套数组
来源：http://hz.jiagoushi.top/gtissywogr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hongshengwenyu.top/gtrmedtrmr.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtxhavlcag.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zdqjudy.top/gtgxpeahmi.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gtvmmugzfj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hywenlv.cn/gtpmesbfhr.html

Go:   // 手写双层循环
来源：http://hz.jqgfzy.top/gtiynimrxv.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtgxfzynxg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtbwgihulp.html

[D19] 按字段分组
来源：http://hz.xingfuxueyuan.xyz/gtmfkbcqwf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guowangkeji.top/gtdojbxuyh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ybcxt.top/gttgvmrdzp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tanke756.top/gtzgokueke.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtbjwlpmnb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigfzy.top/gtzorijjbo.html

Go:   // 手写 map[string][]T
来源：http://hz.jinghuilouyu.cn/gtdkybiiie.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnxiangtu.top/gtgpbibpva.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhengqikj.top/gtprprunaa.html

[D20] 统计每个元素出现次数
来源：http://hz.xingfuxueyuan.xyz/gtaxjyhidq.html

Py:   Counter(arr)
来源：http://hz.yongpay.top/gtnpephoel.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtuswbdlps.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nwbrower.top/gtgslxymgl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtegljdssp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ywan-chungtsiang.top/gtigjfiroc.html

Go:   // 手写 map[T]int
来源：http://hz.daxiang520.top/gtmvcsfork.html

Ruby: arr.tally
来源：http://hz.nanxinkj.top/gtarkgyvbi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj202588.top/gtvmksrufl.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gtgejkrafd.html

Py:   x in arr
来源：http://hz.cheryme.top/gtgkgcrdih.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtmgqilrdb.html

JS:   arr.includes(x)
来源：http://hz.tanke756.top/gtoxrzppcc.html

TS:   arr.includes(x)
来源：http://hz.vqdsnc.cn/gtmfimtdjw.html

Java: list.contains(x)
来源：http://hz.zhiwuduotai.top/gtggawlgsp.html

Go:   slices.Contains(arr, x)
来源：http://hz.bjfxy.top/gtvkkezwzf.html

Ruby: arr.include?(x)
来源：http://hz.xziqi.cn/gtpongdvlu.html

C#:   list.Contains(x)
来源：http://hz.yj202588.top/gtralgcnco.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gttnwgysvh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gtfgijetet.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gtaolotzbs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj202588.top/gtimixiaah.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtqaucrjfy.html

Java: new ArrayList<>(list);
来源：http://hz.yvedp.cn/gtamwbjalm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigufen.top/gtpegdeddf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtzshuwexe.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gtwbjfzhmh.html

[D23] reduce 累积计算
来源：http://hz.zycfv.cn/gtklhgdnqc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nwbrower.top/gthngpgdfu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ivvv.top/gtoyxjznar.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtjtonavbi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtnyqycayt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.birdmap.top/gtmytumevv.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtatrbscjd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gtiofxcinf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtwhunndup.html

[D24] 字典 / Map 基本操作
来源：http://hz.sxryk.cn/gtjiqqyzzm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jlsjyb.cn/gtsmhgczlx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hongshengwenyu.top/gtxxhavfyn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yangfankeji.com/gtavxnhfyd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yonumen.top/gtfboatfyk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xinyue.icu/gtwvwgvnyp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtpkgmlazb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj20258888.top/gtncjwtsfp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ywan-chungtsiang.top/gtngjzimlk.html

[D25] Set 集合去重与交并差
来源：http://hz.wangshuangyany.cn/gtjdpfkxov.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hfpthk.cn/gthrexbpgq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.iojbl.cn/gtlhrzrhjm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hnqzz.top/gturxugmvc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gtxlquqggl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gotoacloud.top/gtjuveixno.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xylfe.cn/gtyylumiyi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.guannengcc.top/gtnvezujgg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.bjfxy.top/gtpcawakyd.html

[D26] 数组转字符串
来源：http://hz.chenjidiqi.icu/gtiqztvcof.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258.top/gtcierqczf.html

PHP:  implode(", ", $arr);
来源：http://hz.hnxiangtu.top/gtjqbuqlhq.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtaplsspfp.html

TS:   arr.join(", ")
来源：http://hz.havefunace.top/gtrcpkbnsr.html

Java: String.join(", ", list)
来源：http://hz.yanxiufei.cn/gtaiqakhqt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.smart0.xyz/gthljugvsf.html

Ruby: arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtnsclyyju.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtkylwnnya.html

================================================================================
来源：http://hz.haohaochexian.top/gtjetkrbzq.html

E. 字符串处理
来源：http://hz.zhijiandao.cn/gtkimzmvgx.html

================================================================================
来源：http://hz.cucudq.cn/gtlodljpmt.html

[E01] 拼接字符串
来源：http://hz.tianlin.xyz/gtqmugmwru.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.0kj1m.cn/gtskceuzpn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yongpay.top/gtrfphohad.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtlfpbafnn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtctwjppba.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tianlin.xyz/gtndnkqtxo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.iojbl.cn/gtvzetciqd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sysykeji.top/gtydtrfmdq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xylfe.cn/gtwigjsmjy.html

[E02] 重复字符串
来源：http://hz.zhengqikj.top/gtytvjgfcl.html

Py:   "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtmdnzlvxj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhiwuduotai.top/gtoggxrzft.html

JS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtycevruab.html

TS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtvorspuuo.html

Java: "ab".repeat(3)
来源：http://hz.316326.xyz/gtlxrgxyxq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.316326.xyz/gtmonpmolr.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gtqbgyuirq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.9152youxi.cn/gtqofrvdqf.html

[E03] 截取子串
来源：http://hz.vqdsnc.cn/gtmnylzglp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.guowangkeji.top/gtbixomtvf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aizwys.cn/gtqgizvics.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gtfvotbwbc.html

TS:   s.slice(1, 4)
来源：http://hz.daria6918.cn/gtzcxtwmck.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtisvhjveq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtfozjtovt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yangfankeji.com/gtcainsmst.html

C#:   s.Substring(1, 3)
来源：http://hz.redwolf501.top/gtptgwxwxe.html

[E04] 查找子串位置
来源：http://hz.jiagoushi.top/gtopufhvov.html

Py:   s.find("x");  s.index("x")
来源：http://hz.smart0.xyz/gtpcmzxgxs.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gtmbexalzc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtrqdcuyap.html

TS:   s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtitrzxsls.html

Java: s.indexOf("x")
来源：http://hz.tianlin.xyz/gtirvxjkqk.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258888.top/gtasxigftq.html

Ruby: s.index("x")
来源：http://hz.hysaishi.cn/gtymqaklwu.html

C#:   s.IndexOf("x")
来源：http://hz.zhengqikj.top/gtaplvhnzp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.redwolf501.top/gtzydetnfq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pengpengdd.cyou/gtylzvhvgm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ybcxt.top/gtvqyvcbxn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtbxhigvby.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sxryk.cn/gtofcbwzie.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtlochdtgr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtzlootaoo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gtobkhkbnm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.mhx1999.top/gtuivjsfpl.html

[E06] 替换子串
来源：http://hz.chenzaomai.com/gtvrrrdefe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.haohaochexian.top/gteylzvees.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.feifeiyinyue.top/gtdtqyphna.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtqywnbkie.html

TS:   s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtctamdjfa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gttbooarwn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtzpsnniwj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnqzz.top/gtkftceuel.html

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtwtxunccf.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gtoikdolkm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258.top/gtjovvxckl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ydjk.org.cn/gtrqtlwuqu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.svipenyu.cn/gtdysjaiua.html

TS:   s.split(",")
来源：http://hz.0kj1m.cn/gtcmbwzqcq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.c1oappe.top/gtzemquwcr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gtjyrkoxki.html

Ruby: s.split(",");  s.split
来源：http://hz.hongshengwenyu.top/gtxwzdhank.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhijiandao.cn/gtovnxrczl.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gteickjvli.html

Py:   ",".join(items)
来源：http://hz.jqgfzy.top/gtymzxyyfg.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtsghvxova.html

JS:   items.join(",")
来源：http://hz.birdmap.top/gttkmrcvzn.html

TS:   items.join(",")
来源：http://hz.jianghu66.top/gtrapwsfip.html

Java: String.join(",", items)
来源：http://hz.xuanzx.com/gtwoptqlkz.html

Go:   strings.Join(items, ",")
来源：http://hz.yj202588.top/gtlxftgxzn.html

Ruby: items.join(",")
来源：http://hz.redwolf501.top/gtmilgnwxh.html

C#:   string.Join(",", items)
来源：http://hz.nwbrower.top/gtoobqdugb.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtplywbiee.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydjk.org.cn/gtylkeqdyl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.smart0.xyz/gtcgfgoucy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gteeuohhnb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtiixdybfv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtdgzcfptb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hywenlv.cn/gtoahxzjqa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtpeakaqme.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gtizdcsnsk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.quarkkingdee.top/gtguxeqocx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cashguo.top/gtqyyxmina.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hongshengwenyu.top/gtlrksqgvn.html

JS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtbyzmnxus.html

TS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gttinzfbwe.html

Java: String.format("%03d", 7)
来源：http://hz.fengsongda.top/gtxwkbpway.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.snrcjt.cn/gtisgieunw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.bjfxy.top/gtrdeqvfbe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yuanzhike.top/gtoxoongdy.html

[E11] 反转字符串
来源：http://hz.yanxiufei.cn/gtwtpxgbsf.html

Py:   s[::-1]
来源：http://hz.yvedp.cn/gtqlyqsnpx.html

PHP:  strrev($s);
来源：http://hz.yonumen.top/gtbacbibcc.html

JS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gthjrrwklc.html

TS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtvfoowrbb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.redwolf501.top/gtlmnosbls.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pycfn.com/gtuaimbpna.html

Ruby: s.reverse
来源：http://hz.cucudq.cn/gtqfdumaye.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtuivtfwla.html

[E12] 统计某字符出现次数
来源：http://hz.jqgufenzy.top/gtvblgqwvv.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtjsiribql.html

PHP:  substr_count($s, "a");
来源：http://hz.yueranfly.top/gtugxynhhv.html

JS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtplsfzwdu.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtrhyiwlat.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258.top/gtzgvfhurg.html

Go:   strings.Count(s, "a")
来源：http://hz.cheryme.top/gtlogockcg.html

Ruby: s.count("a")
来源：http://hz.gotoacloud.top/gtxsdpqgwp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tian-w.cn/gtcxkmfmkb.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtemvcnwcd.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtbwyobmyb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cashguo.top/gtlqcblvet.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtxqetwbtj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtnukqfnki.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hfpthk.cn/gtamnrjxsn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangshuangyany.cn/gtqualbzuu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtxqfjccyg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.birdmap.top/gtkoqkbmme.html

[E14] URL 编码与 Base64
来源：http://hz.zhijiandao.cn/gtpbsswxpa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydzc1.top/gtnwhsjodd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinghuilouyu.cn/gtpdsnspug.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tianlin.xyz/gtrfaasynw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gtsaemxrqt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtmanzmzze.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pengpengdd.cyou/gtjkpyjbua.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtpoiehqlo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtcdjqexoh.html

[E15] HTML 转义 / 反转义
来源：http://hz.316326.xyz/gtqpypgmna.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.c1oappe.top/gtxdfcwcbc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.svipenyu.cn/gtticyrcyp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnqzz.top/gtruootxte.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgfzy.top/gtldhkzbcm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenjidiqi.icu/gtxtsxyrdg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigfzy.top/gtrzxspyse.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuxming.cn/gtpyedeqyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cucudq.cn/gtztkwlwtw.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gtiupndxxy.html

Py:   f"{1234567:,}"
来源：http://hz.hongshengwenyu.top/gtpobkrnlj.html

PHP:  number_format(1234567);
来源：http://hz.hammf.cn/gtxpoigspb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtpmwdhwlm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtgohtpvbn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhoulong.xyz/gtdplwkcwf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hysaishi.cn/gtuwgqmnmd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangshuangyany.cn/gtvgrjteby.html

C#:   1234567.ToString("N0")
来源：http://hz.nwbrower.top/gtzpljpmzo.html

[E17] 首字母大写
来源：http://hz.xylfe.cn/gtshnulevd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.52xcode.cn/gtwalirqys.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtbebiqqhp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtfkpaxqvd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtyfjaxqhs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pengpengdd.cyou/gtwrkfdlgp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gtzbdgqrvu.html

Ruby: s.capitalize
来源：http://hz.cheryme.top/gtizhoakly.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yonumen.top/gtzlcmbzjl.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtmacmnibv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhiwuduotai.top/gtqpalfooy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigfzy.top/gtxkoygsed.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtapgogseb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtuhwkkfyc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sweek.top/gtdgicwomu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gtixvvsgbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xinyue.icu/gtlggqkvpz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xingfuxueyuan.xyz/gtomjxokxv.html

[E19] 多行文本按行拆分
来源：http://hz.xinyue.icu/gtiyzeqpzf.html

Py:   s.splitlines()
来源：http://hz.guowangkeji.top/gtzvcfmfbt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtnyfgkhzf.html

JS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gtyaomlwys.html

TS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtlqacuspe.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtpmmijwtd.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtpjdjowxq.html

Ruby: s.lines
来源：http://hz.hywenlv.cn/gtfhwykxfk.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtyvjfuybi.html

[E20] 判断字符串是否为空
来源：http://hz.ywan-chungtsiang.top/gtjdgkiqjd.html

Py:   if not s:
来源：http://hz.aizwys.cn/gtdsmgsjna.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gzhubu.top/gtkktdikhz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gtrnggcgcf.html

TS:   if (s === "") {}
来源：http://hz.yuanzhike.top/gtgzyzcucj.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtsjxzqzfa.html

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtdrngfenw.html

Ruby: if s.empty?
来源：http://hz.pengpengdd.cyou/gtstndtyoi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nwbrower.top/gtapopmjbq.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtibzpohyn.html


<!-- 参考信息 -->