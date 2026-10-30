代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gzjtlxend.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gppoqahae.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gjkwdxyqv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gskuifmgd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gpxmykrte.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gwxeodwch.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gfapdbgci.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gnmiilhym.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gamqqqarq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gypvuoqnm.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gxetfvkew.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmclgvsd.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/giohcnmfx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/ggdkbqbic.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gewpyqruy.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gjvjhhkal.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gdqkfqrhe.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gcrkgdcor.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gktztayxq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/glaugltlb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gnqqdmiaa.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtwfzyucx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gqqjfyrvd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gmkcnxbor.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gcrdrjqpm.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gtjhlbutj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gbwpyphbf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gbywyxcet.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gbqiaaqwo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/glkntxifh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gdnhtrdmm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/guvipyddq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gznxoufls.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gpxwpwhzo.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gtzgqwetw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gejmwbhys.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/ghompnamw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gflownlhm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gvajoegul.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gxdemwbsm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gaeivkvyz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gfotnffhp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gtjvppjcy.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gwohzukkk.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbibuxbv.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfvrjvsen.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gvirxhemh.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gcfokwgrv.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gdleezjuz.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gtnevjrxw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gdujeukro.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/grfkavarb.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gszugwbjj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/ggnrnhsbq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gleixndcx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gviipdhdk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/giqfzjdhb.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gxwpbpdkq.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gfdnosdgb.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gxfjcxezn.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/ghpaziuph.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/guwzjpyva.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gfgqotowi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gemizzrgo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/geponjqex.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gcbcqonft.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcmangcds.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/ggomkhxmm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gsmpjpvof.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpabqhxrn.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gjhbecrwy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbskvyuse.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glnfguhgy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gqdjhwfus.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gjgqdegkg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gsxawxgph.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/grlkwnmtw.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gmrguxyfl.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gvtcbqzpj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gwplnliys.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gdiidpdss.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/graysjtfm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gdksbejrq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gsciephpf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gkclshjnp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/grrqgwkpu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ggbfsjroc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gekrlkqft.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gaucrvqlq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gjwcalguu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gdbfsqgod.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gmoguenbc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/ggvvocnbj.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gkbcueqff.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gyzbszhvk.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gfphvoufw.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gatarkfwn.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gjlsccvmf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/ggcbmbzhh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gamlptuvk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gnhgmiecl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtaiemmeh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/givhvsvpt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gvhpavoet.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gauehsqvi.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gkkenrudl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gfubctxef.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gtcgiirea.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/glfvuhujp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gcbwokfnm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gyctohjtc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/glgxkjlxe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gwjtfputw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gzkzdzknr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gkncpfvge.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gkdhucexz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gzjbobtzq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gslftrtcs.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gnyfnovbn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/geclglfyq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gkxmbsfbo.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gphrpnbxm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggryhwkne.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gbbrtnyum.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/ghzrnzuli.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gfpctbqer.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gsdrfvrih.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gbppeaxro.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gszedtycl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gmrimraki.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gpuexabcc.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gjyksfpzj.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzfkxohec.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/genpepznz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gljxpvgts.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gzxmaxbch.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/giphjzipw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gnuwzwjhn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gofarydvd.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gzbdprvkn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/glbtzyeqp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gszzgajul.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gnanniqek.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvczovoqd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gysxdieij.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/givycppeu.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gkpkphayl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gtpuekiwi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gtwoikdzf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/ggkllpcwu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gikqhuunt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gvnlmfwgq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/ggpqmrglb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gcobzxxdc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gmjeaddcw.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gxvwcgwdj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gqtirhsvj.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/grdposzai.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gigjcduhu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/ggzktgjom.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gronimgqw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gkkhmqate.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/ghgjfwhtf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gqdbwjzno.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gexwcfpxi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gzcnzhcrr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/grrsxqzvc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/ghmbinoja.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gwkohwbvm.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gvazkmmax.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goouytxzn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmmciij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/geupcfqbj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gkpjzbjqa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gyvkitywu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gkaohjelj.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gcjzfvrlf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gywbrfimk.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gemozqhzk.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gbmyfdbed.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/ggavadoyz.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gnskihjly.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gfunektmu.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzoefzaeu.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/glnfroiyq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gorcwdkns.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gzyzieutt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/guywsowny.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/ghvmtmoyd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gaoluzloa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/glilgtlpa.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gblnncorb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gwnlrjoss.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gcdfuwezr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gbxdskilc.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gmmltxcxw.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/glaxehsof.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/ghsrgjwtn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/guctgllcb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/grlhwmayw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/girkhkvoy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/grksqapde.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gvmsiocar.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gyfdwslfn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gptmcsmnh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/ggpktjiyp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/guvwmkiqh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gvwuctlcv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gtijeqnoz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glzmjsmtb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/giitehmhw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gqckxglsl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gdlcmgedz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/ghzhfeamx.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gwfcwizse.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/ghzhiinhd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gxwmeyefx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gsjnfvugu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gdecfqhsd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gliczggem.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gepxhjjyt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/glgrrpcne.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gmalgnmjo.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtnghrmra.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gwzmgqbaj.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gsybnsevi.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqvmhyews.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gvwgefyzw.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ggwocgvbj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gtlrcffsr.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gliozlxkr.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gfnflzqxg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gluazqict.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/guijsadei.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghpnkriho.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gizrlhhnq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gvxkadftm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/ggagievmv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gbxlfgqsk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/guwirdoao.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gdpjvmtux.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gfyogiwag.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/guouxvdxr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gluzooyub.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gpdnameka.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/guxpdfxgw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gccsbszsk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/girroqaya.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gozqzvyet.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gehmhsdxy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gptebolvz.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gmhnvbvkp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gaqtxjtuo.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gksfzyymh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/ggqpaudio.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdiktbrwj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghuqsgmeh.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtsaijbei.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ghewirzxp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gbwsqwevz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gqxawmvrp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gmtczlmxl.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/grmyxqcox.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjuuszubm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gchckodky.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/giopkfjex.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gyyznfgfa.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gpxqbhsse.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gbcjieqtt.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gqxetmdcm.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gqyslitnx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gphbgvzsf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gnpgascrd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gnovzqeql.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gsqztahtz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gmzjmvrjn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gkggzinjy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gepyelsnf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gbfcaajwr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gdfjtdorg.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gdwiqonmp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gausgnjww.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gkldigqlr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gyfwtpiap.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gfrftljes.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxpyjrhoi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gecsemayf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glxjluzlv.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfhkfdqar.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/glulkryjy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gdqogaorr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gfklzqlcx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gdcugtdsy.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gqkmqrywi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/grnzdtqjj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/golqdabtu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gldfrxdde.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gustlqtau.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/govhxomew.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/goiuegzax.sHtML


<!-- 参考信息 -->