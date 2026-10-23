代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uclfgvga.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rudmrazl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qedivhfx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ptbbasmi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qocvnnih.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hctozadw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ysyqajlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hzatjupj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mjniifaw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qglybtzz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3plskssdc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wfyaxhlz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wnclulyn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3whnihcwg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxsuaqi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wyefodjg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vlmyeyfh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3lfvieozk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kyptgzes.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lddiobqu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxofhbs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dkhozate.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jlxzkgks.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3muvimotd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ysqzxopt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uzlhifmn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vkbkxauh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mscokuob.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yhqanmgc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ibmqcval.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3alnfekaa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dqwpewje.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytessqtl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aufpvrmz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3recbtmas.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ugxkydco.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zjlhynzr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ajuulmbr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tkkxzbue.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vqdrwxrt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3extnliig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zkgfnzvy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tiyerzur.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wejmezif.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zdyuwaqd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iguzgbfq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3yqvqvsim.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uavykpkt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3buywwaym.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rghgqrsv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zfrglxmp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vaxygoef.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jkfytefr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mdddqche.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ficpmoxd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3spmgzcef.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bxtewzje.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tjlkqxvn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rhooajvd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hahhnbuh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frkmutkg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3znqmkptv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vzopkrjh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nsfsbsdd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rrvqrjas.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vjtkkmcu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hrdknrxn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uwlxejtk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ieibtsjf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qxkkbhue.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cthpxiyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pparryzb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zeklypje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vboyhete.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvlmmbv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qgpjuuqr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zchencrp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hlopuorq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfpxkavr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3gbnqgqjj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qhedyhsu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3eltsghwd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdngudp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rvragwoa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mmtrpeyi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tsomxkyh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3eqkgdvcs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qpnzewpw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fpfmhnnm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3epiwauas.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rlrakeyr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcghsflm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgdcggxb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dbfunine.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mhrehgar.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lajwnslp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ewkbykat.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iljnwcxt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ibsoikxe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqrxctsx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tyfedcmf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ntereljt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dkmsnndn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pjpyfwnu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hrpqtdsa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3inkqaaxx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3amuoqgnw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rnlcaizc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ayovxjby.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aynfunzw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbkqthmy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jhvmpclx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qjegshzg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vfjwjjnn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ygwwpomv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3brzztyrr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kiymivdn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gsywiyyz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3szwocxvn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lpuuikdi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3krowweqv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ndfsyeej.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpblrmoy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eojmlhem.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3buycmhkt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tjdnhuts.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gtpugmft.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dsdlkqba.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ekzbejmj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bofnymul.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ldweguiv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axgvdwpd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fimwwveb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izuxstoo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xpzesonz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zazcvghj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxcybvvo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mqdlkhgr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tboudbzo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3gokjfbyh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bdkfixcn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3iicdlgnd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pemarkcz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bmygjtap.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hqlvajhl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvzouxfv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3suivkwyk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uuewxwba.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gfitoyio.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evxfqmfa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pawnvczq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ivxlmriy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gjqlsawb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3klnbfpbi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uvdroitq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vrmfjjux.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3izkgihjw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3hrzmbzpz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pajdfvkl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oyehclnx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3semcplyt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3scwpseqx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wgcilqjr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3yonqluoe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yisracbp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3adykegcs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zskrvkbb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3upzwnish.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3uqsngrka.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfsustzx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwqbmabj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3obqseckj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wigszywp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwjqwksz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jflkkoee.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gqkmokmx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vutlopfo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3raqjnugt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvtxbmwv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ijzfjhlu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gbunfgpo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jfvnazsu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lxlvrwrz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jxnwyvda.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3atusazmj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hatrqsve.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwiwfwfr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kikprjhv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gfbwaqih.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fbshwfdj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sonzcawv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3azilnwej.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3isbczjli.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bkgjtqvp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lbmkzwof.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpunrvsh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3coyumijs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kvfcfoox.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3quokkabk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bexiowpd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3enbjzxcw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3dtcxfmfb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hnvjhljb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xttoyxrj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hehvqxxm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vowznhyk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xyvhzgoc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtaeoom.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ttrxnuzq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmiqflni.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdhnzxm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3heqagmww.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dcdqxnwf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dwoamofi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3beqddczf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dcaukowy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pyctfmao.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wegofils.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ixttmkyl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yumfksoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhzmlcbn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ftvbtpab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbbmtqdc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vpozedkn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wqzfxmgv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtxxgenw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvpnazg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mwuiuyls.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cbnxdvud.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iupxnrxt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dijayifl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3opqpvist.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvsgqhdu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xxxaaaaw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3umymmdwv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3obfyxicc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bqmbxhtp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3huuwdjau.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmqggxvq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hdcdqeyt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dywnuwph.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kiaskzcv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3niiiscef.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xygckoyy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ezzauzwn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3blwchjxc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3muiubuip.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ldxvajtj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jyfhslwb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykuojsbw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hysxainu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sgztapqg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vhpkkwfy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qqgroqsq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3urwmzztc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mikoptdj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3izfwhbni.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3igalxnzc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ahvsvuqt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dpmvpyqg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rodumvkx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xgaoojhj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3btwjtzap.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zhmvjigm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gfmxuxda.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xskgbvic.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yigjtggt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qpksyrms.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sqgdygop.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvfczvu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jywljake.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wfqcksnd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3spjaapzx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nkrsdzoj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3juxwpcjh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ivwxnfov.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hlepygov.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3izzmiqta.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kzhckwrt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3njvbdnxv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fmnrqpwh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aqkajpsx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dqeurejv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bjhgfxwp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vsppwhcv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xhiainly.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vwjpvbwf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rnwanvqd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xmtbdpyc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ddziejiq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3heysrxwc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3awjrozks.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mcqezxys.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aegjwzxa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wehyhngb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ouenzftf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rufrqbgf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ylbusndd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zkhffhjh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jcaoffeq.html


<!-- 参考信息 -->