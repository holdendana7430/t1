代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtsthygacf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtkluahjuq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtgyoczxvw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhoulong.xyz/gtlgwnwshc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.meibo888.top/gtmjuxaoyj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nwbrower.top/gtfwzrrius.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.9152youxi.cn/gtqotvdqtm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangshuangyany.cn/gtjagndsyo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.iojbl.cn/gtzmgtynpm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yangfankeji.com/gtrtmeckwa.html

JS:   arr.map(x => x * 2)
来源：http://hz.cqqwz.cn/gtcfyygozl.html

TS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtewquvoen.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fengsongda.top/gtqkqywauf.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gtrotmyswy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtmvimwqfx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hongshengwenyu.top/gtokmsdknb.html

[D15] 去重
来源：http://hz.hammf.cn/gtjquhiyya.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gtvudzjsts.html

PHP:  array_unique($arr);
来源：http://hz.yj202588.top/gtvjoicxxv.html

JS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtlryhpsvp.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtiudijdbc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.havefunace.top/gtbipjbdcd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangshuangyany.cn/gtpconzeyb.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtvmzspkwl.html

C#:   list.Distinct().ToList()
来源：http://hz.ppjwa.cn/gtydbbqvia.html

[D16] 求和与平均值
来源：http://hz.bjfxy.top/gtypvazubi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hysaishi.cn/gtyrkyobfw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cheryme.top/gtqgyvppog.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtwjkfphrm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtcxpbvhbl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtfmgocnec.html

Go:   // 手写循环累加
来源：http://hz.yuanzhike.top/gtrmuiezuf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtiapihpmv.html

C#:   list.Sum();  list.Average()
来源：http://hz.tian-w.cn/gtufwwzflo.html

[D17] 最大值与最小值
来源：http://hz.yj20258.top/gtyrvfqavu.html

Py:   max(arr);  min(arr)
来源：http://hz.pengpengdd.cyou/gtetjtdypz.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtdtzgczys.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ivvv.top/gtsrgkgeyi.html

TS:   Math.max(...arr);
来源：http://hz.shuidangran.top/gteuypbrog.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenjidiqi.icu/gtzdrplsix.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenjidiqi.icu/gthfjncpdu.html

Ruby: arr.max;  arr.min
来源：http://hz.fzhhl.top/gtmyrjnegi.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtsobmamra.html

[D18] 扁平化嵌套数组
来源：http://hz.guannengcc.top/gthbntajcb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.vqdsnc.cn/gtloldsyjk.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtrqqpfxoz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yvedp.cn/gtylrkomhg.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtbgnsbwoq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangtech.top/gtglpugjwn.html

Go:   // 手写双层循环
来源：http://hz.yangfankeji.com/gtrvlyakmb.html

Ruby: nested.flatten
来源：http://hz.guannengcc.top/gthntudavr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.redwolf501.top/gtyqoqtllm.html

[D19] 按字段分组
来源：http://hz.zhixingplan.top/gtwonqakdm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.smart0.xyz/gtnqfwbvbt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.52xcode.cn/gtihzoileg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtlpqjxdyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dashuyun.cn/gtulvvsyxm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gtlvtfrzos.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gtplcebwrb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daxiang520.top/gtkfjeuuxt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shzxlz.cn/gtosjswzmu.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gtlyvkpsib.html

Py:   Counter(arr)
来源：http://hz.shzxlz.cn/gttnfgcnne.html

PHP:  array_count_values($arr);
来源：http://hz.cucudq.cn/gtpnbrikkf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtjpylxrgi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtoajrtpmo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yueranfly.top/gtvkezagzt.html

Go:   // 手写 map[T]int
来源：http://hz.aizwys.cn/gtazlsttru.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gtyjsbsrll.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnqzz.top/gtcusreyia.html

[D21] 判断是否包含某元素
来源：http://hz.zhongyouzk.top/gtxsfahfrn.html

Py:   x in arr
来源：http://hz.yuanzhike.top/gtiliqdvkx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yvedp.cn/gtydnrbhon.html

JS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtygcuyids.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtggmnclzk.html

Java: list.contains(x)
来源：http://hz.zhoulong.xyz/gtjzmvfrta.html

Go:   slices.Contains(arr, x)
来源：http://hz.hysaishi.cn/gtqouzpcvf.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gthtjgacpt.html

C#:   list.Contains(x)
来源：http://hz.aizwys.cn/gtxsgiuyaa.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtukbpzhwz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenjidiqi.icu/gtsasxeinj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fengsongda.top/gtmntnaezk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtkqecvgtt.html

TS:   [...arr];
来源：http://hz.guannengcc.top/gtdacuaedw.html

Java: new ArrayList<>(list);
来源：http://hz.xylfe.cn/gtpzvnlvuf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gtrdlqxwvb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtyxqkjhuh.html

C#:   new List<int>(list);
来源：http://hz.ybcxt.top/gtauegzyfv.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtukbbmdip.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtvbakdqtf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xylfe.cn/gtszlkbdus.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtosvtglwi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtszkizdmd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhijiandao.cn/gtnrskvepz.html

Go:   // 手写循环
来源：http://hz.316326.xyz/gtiqtpfllm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ybcxt.top/gtkbxapyev.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gtoluqlret.html

[D24] 字典 / Map 基本操作
来源：http://hz.havefunace.top/gtkrudizse.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xylfe.cn/gtuhddxtri.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gtjmkipbrm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xylfe.cn/gtgkfhaevn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gaohongyu789.top/gthflebnmm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.52xcode.cn/gtathsfxyj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gogol.net.cn/gtdwvmoanj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangshuangyany.cn/gtckhdqrww.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.kuanghao11.cn/gtpxjktymk.html

[D25] Set 集合去重与交并差
来源：http://hz.hnqzz.top/gtkinssnpu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sweek.top/gtyuzaxtdc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gttkdebxwn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shuidangran.top/gtyxuiopdj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gotoacloud.top/gttrqdsujp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yonumen.top/gtqmujfdtb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtiiapdofv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhengqikj.top/gtmhfhmjwr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtmjbtsvwd.html

[D26] 数组转字符串
来源：http://hz.jinqigfzy.top/gtwruytcdo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.316326.xyz/gtdtinerqu.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtuqpsdlga.html

JS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtmjfnkenk.html

TS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtaacimeaq.html

Java: String.join(", ", list)
来源：http://hz.iojbl.cn/gtlujsyrhq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtnjokvjnv.html

Ruby: arr.join(", ")
来源：http://hz.zhongyouzk.top/gtoqtludvm.html

C#:   string.Join(", ", list)
来源：http://hz.dashuyun.cn/gtajzazame.html

================================================================================
来源：http://hz.nanxinkj.top/gtrocwvswb.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gtqwhpwxwt.html

================================================================================
来源：http://hz.9152youxi.cn/gtqxurqptk.html

[E01] 拼接字符串
来源：http://hz.aizwys.cn/gtiffyycnc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtdkmujllt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.svipenyu.cn/gthctasbgf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtvaxpqebu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xylfe.cn/gturzucvox.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shzxlz.cn/gtwutxxdqr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fzhhl.top/gtwqjzhgce.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.svipenyu.cn/gttlksaykp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.0kj1m.cn/gttcqgaprc.html

[E02] 重复字符串
来源：http://hz.gaohongyu789.top/gtwlohdfwe.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtyhnzkrsi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.0kj1m.cn/gtdjqwxohi.html

JS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtgldpdknp.html

TS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtlqckjvpc.html

Java: "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtogzbeqzw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tianlin.xyz/gtqmzrhzit.html

Ruby: "ab" * 3
来源：http://hz.ybcxt.top/gtcaxyhcqg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtewzmbeav.html

[E03] 截取子串
来源：http://hz.zdqjudy.top/gtfavtcdet.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.vqdsnc.cn/gteworxqlz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.svipenyu.cn/gtazbubmeu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.andypj.xyz/gtddodizio.html

TS:   s.slice(1, 4)
来源：http://hz.shzxlz.cn/gtclcvkihq.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gttsqrtvww.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gtinkowxdj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cqqwz.cn/gtnezpcnfu.html

C#:   s.Substring(1, 3)
来源：http://hz.fengsongda.top/gtgclhhfkm.html

[E04] 查找子串位置
来源：http://hz.andypj.xyz/gtfdwkegzb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtnciwkfjh.html

PHP:  strpos($s, "x");
来源：http://hz.c1oappe.top/gtlilenyqg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.dianchejie.cn/gtghwulfla.html

TS:   s.indexOf("x")
来源：http://hz.mhx1999.top/gtrakouitz.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtpayvjkcj.html

Go:   strings.Index(s, "x")
来源：http://hz.ybcxt.top/gtyklgzqzv.html

Ruby: s.index("x")
来源：http://hz.zycfv.cn/gtuvyrnorj.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtkpcmzgwt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hywenlv.cn/gtuocyscoy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xinyue.icu/gtfdpwcbmt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pycfn.com/gteqvindhm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtzwrhuicl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.daxiang520.top/gtuzdptzfx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtitdfgaht.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258888.top/gtuwfcjsar.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhijiandao.cn/gtagaqbali.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cucudq.cn/gtzspuzobt.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gtovnifftq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.aizwys.cn/gtztrkpcbq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xingfuxueyuan.xyz/gtkpaavnwh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtktvzvnuj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gthdilkcvh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtdyfaeyot.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtzgvpjrmn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guannengcc.top/gtuifnojbv.html

C#:   s.Replace("a", "b")
来源：http://hz.gotoacloud.top/gtybbiipmh.html

[E07] 按分隔符拆分
来源：http://hz.jqgufenzy.top/gtdtvxyztk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guowangkeji.top/gtqkvmxeyt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guannengcc.top/gtczwknvqt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yongpay.top/gtrmqnokpe.html

TS:   s.split(",")
来源：http://hz.jinyuanbaomall.cn/gthswvsetv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtbtcntfnu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtcsnehywh.html

Ruby: s.split(",");  s.split
来源：http://hz.meibo888.top/gtlsujsixn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuanzhike.top/gtzfqsnxpe.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtgozvvbwy.html

Py:   ",".join(items)
来源：http://hz.zhijiandao.cn/gtujdebbvm.html

PHP:  implode(",", $items);
来源：http://hz.ywan-chungtsiang.top/gtaayxaxdd.html

JS:   items.join(",")
来源：http://hz.ybcxt.top/gtmdrndgba.html

TS:   items.join(",")
来源：http://hz.gzhubu.top/gtiyprvosm.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gtpvocrwxd.html

Go:   strings.Join(items, ",")
来源：http://hz.daxiang520.top/gtrdakwgbl.html

Ruby: items.join(",")
来源：http://hz.svipenyu.cn/gtogipfayx.html

C#:   string.Join(",", items)
来源：http://hz.guowangkeji.top/gtddauyftz.html

[E09] 去除所有空白字符
来源：http://hz.mhx1999.top/gtvvcbzdxw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.vqdsnc.cn/gtojyqjpou.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cucudq.cn/gtsxwrheow.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtrkpogpuv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtouyxgvib.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuetiantiany.cn/gtiorbtlwx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yvedp.cn/gtkberyyir.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuanzhike.top/gtxbatpnja.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gtizkpplxf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.vqdsnc.cn/gtwsluegif.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.aizwys.cn/gtxvdruuye.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hammf.cn/gtgwfoaigr.html

JS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtpiyyssxk.html

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtysqsmekq.html

Java: String.format("%03d", 7)
来源：http://hz.yonumen.top/gtvszsrueb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gtgvolodka.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tianlin.xyz/gttlzjqpaa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pycfn.com/gtkwrxgebb.html

[E11] 反转字符串
来源：http://hz.jlsjyb.cn/gtgxdfzcex.html

Py:   s[::-1]
来源：http://hz.havefunace.top/gtcduuwtul.html

PHP:  strrev($s);
来源：http://hz.xziqi.cn/gtycffbipp.html

JS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtotpuxqie.html

TS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtenkfmhmq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtztyjclqq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ivvv.top/gtudcgqgvm.html

Ruby: s.reverse
来源：http://hz.ppjwa.cn/gtkhbcpnaz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gttgoxzxug.html

[E12] 统计某字符出现次数
来源：http://hz.shuidangran.top/gtiargnqcm.html

Py:   s.count("a")
来源：http://hz.zhoulong.xyz/gtsfsczgoj.html

PHP:  substr_count($s, "a");
来源：http://hz.yuanzhike.top/gtqfxzjnta.html

JS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtqsyadbnr.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtvftgjmht.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenjidiqi.icu/gtffjuwvyz.html

Go:   strings.Count(s, "a")
来源：http://hz.dashuyun.cn/gthrgnsqpm.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gthldxiopw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenjidiqi.icu/gtqsmexawq.html

[E13] 逐字符遍历
来源：http://hz.quarkkingdee.top/gtbgrhbkmk.html

Py:   for ch in s: print(ch)
来源：http://hz.hywenlv.cn/gtwxxigzjz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jianghu66.top/gtisgjthut.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtkgbkkgyn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtrlequggl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nwbrower.top/gtptyeejks.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtmmubcfyn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ywan-chungtsiang.top/gtlxfnsivf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydjk.org.cn/gtmvjktilk.html

[E14] URL 编码与 Base64
来源：http://hz.316326.xyz/gtemoyrkkx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yonumen.top/gtwgvrdfii.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtvourqhtt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ehwqpu.com/gterljeyjl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtbqpmryle.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtfqpipqpz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtrqspnusz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtrvljwdqo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtosxofkcz.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuxming.cn/gtpmzmhret.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gtehiblcsq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hammf.cn/gtezisznjo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtgamrojdu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hfpthk.cn/gtfeevinzy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ivvv.top/gtanlkespg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtndcdhopb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtfmdlrboo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hfpthk.cn/gtotmjptwa.html

[E16] 数字千分位
来源：http://hz.yonumen.top/gtkmlrqgyu.html

Py:   f"{1234567:,}"
来源：http://hz.tian-w.cn/gtweqecyqk.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtsnhnpmib.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtbdooiglt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtxskdvoda.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jianghu66.top/gthrjshjul.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zdqjudy.top/gtlunfysso.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hammf.cn/gtivwupzim.html

C#:   1234567.ToString("N0")
来源：http://hz.0kj1m.cn/gtawlhjjzs.html

[E17] 首字母大写
来源：http://hz.ehwqpu.com/gtvpoumxwk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtuafijspp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.9152youxi.cn/gtpzokcrfa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtjbhbkiya.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtygwqokoe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtytfhounm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ivvv.top/gtsxbiivus.html

Ruby: s.capitalize
来源：http://hz.andypj.xyz/gtjrgmocuo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tianlin.xyz/gtweudkwpj.html

[E18] 模板占位符替换
来源：http://hz.yuanzhike.top/gtaghnuhhl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhengqikj.top/gtkogahjmy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xziqi.cn/gticnzvvuy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtualgmnul.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gthhwfdtui.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.316326.xyz/gtmdteiutw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.9152youxi.cn/gtoigafpsr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cdnleiting.top/gtyafpcnia.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.c1oappe.top/gtsxajckky.html

[E19] 多行文本按行拆分
来源：http://hz.gaohongyu789.top/gtganvjbmw.html

Py:   s.splitlines()
来源：http://hz.daria6918.cn/gtgjapfpjx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgfzy.top/gtikbdvmut.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtpdfbxosb.html

TS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtembjnpsf.html

Java: s.lines().toList()
来源：http://hz.chenzaomai.com/gtvqeombmj.html

Go:   strings.Split(s, "\n")
来源：http://hz.yanxiufei.cn/gtyrdealqh.html

Ruby: s.lines
来源：http://hz.smart0.xyz/gthptusmsv.html

C#:   s.Split('\n')
来源：http://hz.hammf.cn/gtfdhwvsda.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gtjyymfqrq.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtdoyqncpl.html


<!-- 参考信息 -->