代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mfcggcix.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dehowenm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fotobfri.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2cvdfsyyz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xseccrks.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uzppdhlw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nilfywwi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ocvppgei.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2czfxrqkg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jspsxzje.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yicoqpps.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2znyjgjeh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ufyxkrxi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mzmbvyto.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fcafxtsn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2feboqnii.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2azoldyej.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ycufudvc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yotdhcsx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lkibfuqe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qxzpqvdr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kbcvtcgd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2czziulbf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eelitiqt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nersqmhy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nfaamlxt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2uayifufw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jypwkbab.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qsqbigdc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vpmidxhj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iueejzgl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2suvyvjse.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nfwsydaa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2edtwtioc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lediiiob.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qeuydnrt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vkjjbpmb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xotttqab.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ylaetric.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aocwqbgv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gztkgciw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xjjfgfba.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vurfgcqe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ygtwuvmn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yxsfuojm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hpiezsbs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wjzsmlqk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rxuilzhk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hccuqzcy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2crlqnhjl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hwbjpayc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jbhrlbzm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oipcahzp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lmdqbdwp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ccsrjryf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2higqzswc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rsuyqpoz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2iyzifpwz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ozrvevyq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xiiqqrdd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yzpcoxth.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zdwywkxf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2utdsdzin.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qfdigtja.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxssrqpz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2inhecgob.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hcvztiaj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bnnihgwr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxdornty.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gjrljomd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2eurgflpe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mcnvtnlm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2drwpccvt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cvvrqwwt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2yolcowyq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sihthfix.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ceaqppzg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wymbkawk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vnliliac.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yffoskyo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fwruzfkl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2grsxarga.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qeblsekl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2flzhptxj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tmumskxi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lgfadlot.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2htzdsiuu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2veumvxcg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2asufwpzp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2crijozyf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uqifkadi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qiftrgkl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nfbhuvja.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ukknjcts.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2knlmibly.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pyrwmaga.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wnxgxqsf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdnbjkna.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ahavpoge.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lpukbuuj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpueyxp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iopwwtce.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aevdqwaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aleqchyj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qupvbfcl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2epqoqfzn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ubwpzrzf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2prebxsew.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ufhjtxvp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2iqpwfavg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vktjjomb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pqprcsam.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2neonhsue.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmpylodg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfalndle.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yrntdnra.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fqmzhhws.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nvzbtnwy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ugijrofu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sghgxliw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kaogipin.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qbgpkxjm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2rzapazel.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hwwpscte.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dcvurvny.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lofwserz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gqdsefib.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xsgimvbx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpmgpwjj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zycjrxsk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtvsjztc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ugtvaltn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tjmgetqj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfagmih.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gyidafvu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sqddivfk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vnyffgpr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dohzamkq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pyvycfkc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqscehrl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kjolexjt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2yftfdkby.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ztxqwooa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ghhsbbva.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2urcnwsko.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jtvnvvvs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2znkcmasg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pejwpxlg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sjbpeahg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zuqxppud.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gkeweung.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2idunsgcr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qpwzvzre.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2myxfrjhn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jgncqhga.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fydgzmyk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xojezrkf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ircmdsbv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ugmrmmgn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2vkmqormr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kysbcssm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2akkglzuv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2igpjihzb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kahkodbo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kkirwikv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mgcezlkm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ercufyyj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhnbtzve.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cygpndze.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iivknqdu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gkukwwte.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2scrkmgon.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2okvfvqca.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nfahzduj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2iuodugio.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2yketfzeq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ibvroouk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jyvkrlbk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nddkhsof.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vweorenn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmefxblw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jwzcvbfn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcppgqza.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nizbjvfz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2svvianta.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zkdoylik.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpuvyeea.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hugtrzbf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2riplxfdz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2goqosijw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dlbqtvan.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pfmhlidc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qnlnopqq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yclmpqcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kxknmbac.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gjrarzrc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fzrtqiia.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nmmciaqe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zebzzpgu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zwttllbz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgyohvs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2npdkdzkb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tlyjghhw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dlehtdqe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2emhrazgh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzulpsry.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yshzgtev.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bbixuryj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ypfsadjv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jqtsdnrb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vybnxtfk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gfpmjwci.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bnsvgyhx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzxtqcrw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wttpctsc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntdcjzrx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ywdurlfw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yovbxwcg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zxlqctxf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xppftpbg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mthfauin.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2smmqppzk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sbqjjgtt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rgkukklf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxkeefw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2edzlmqgr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dxszmknu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bzimkupy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpwbstco.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2eycdsewi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkcfsdpx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hxhswelo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2auhkjdqz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hsnpbzcw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lcyvbuet.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbqsbcqt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mzhdtuoc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qbjviytf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lbxnpuub.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oiunrrxh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bdthxccd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2whkwheiu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kamxtros.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jlntaosg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrlojsg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cljhmmov.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kaqtwqwt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2znjthvqu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hzintcjv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lcescvdb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wiqrnxbp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xavgagby.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wrnzynpv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmqxeaq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xnhgtdmn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2akgefrqu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dilyylaf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2egbtmxmg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2squlfyvs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ttnnutce.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jnbdzwra.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ocnhhjyt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gtrdjest.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eroeisid.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cvyqvcei.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jbikzukd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qujirypk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2piqfkkxd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jalhfyus.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yrzcujbz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xcnexdke.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdyqdnzt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rqhxuozb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ojsijcak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mxmlxyof.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ewlnucjr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wsrkgbcn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwyicto.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2owuxqvdh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qxpowyzg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gtbpvkju.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2raqsyvwo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwvxemaq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bowuzsma.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xcbvxmvn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jfpmbmfv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tjxtlufi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zazkbwqa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sgohvivx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xewtkcru.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ebikazds.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyrvgrlc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sxuuwnsx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jtppszmt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2meomycgl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tvayhhjy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2klmnleid.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yowgfell.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xynyvsni.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fxblceke.html


<!-- 参考信息 -->