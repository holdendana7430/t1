代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nifaxiyz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lcmcehor.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2aslnrtxc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jpstygdc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xfjaesgc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vywspltp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2uqxrogbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtxzqnfp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gaqfyxea.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fgghusgj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cwyrefjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhoieatd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wqplziva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbiywnbx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uoloffjo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wsdhxpam.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xpgrhqea.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zqgnjenk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2eoadbcrg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zzusbbtf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2spnlhmnd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vzhcirxl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zmmgxogt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lzsvpwgu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mczfzdpd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yjneorki.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uaocmzto.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wiqgamkb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntgwseiz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uayuncmf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ghyymjwh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wkrursqe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvrwstjq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yjupzbyw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xtghvmrs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fzhnnpkz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nlusrepd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mbsctqor.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2njpjzoel.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2eqmvovsq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zoxbttvn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yzvpvflu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhkymdnx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2htlewzqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dkvjkkyb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pwnfdzmt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cvsgyqpt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmckplk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hwcsmxbx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qezcpeet.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ixktnmjy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2atyfzmho.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gtirqdwx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wdtyymvy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ddouvoho.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ebqrkawp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gjahskhy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wqxhcrvl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zhdhnnam.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wlxzijrs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdcyvupf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ftjhuiia.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qbpmrzgx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gbewdazz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cctgjodi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkrlffo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vbnankue.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2htoplbqd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2plngttmm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gylaytvj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2arysopvi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ipnclplo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2blmpkqbe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcxseboj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ntvfzphn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mlcujpdz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kxuqhkox.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yiyywmvg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2nimjdlxw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2evmqrtax.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pclfnylj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2umzmgpmf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qnlukqxx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hcglbgff.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2blpeltzr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oncruahb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vndcvfzk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fuyeocoj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rhvigtuq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dvtkntrf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xfhhvapp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2yvdqzczu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxxaanxk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ixnvrnen.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dvqgccyz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cmumnixi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2emqdazqc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zjvecngm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nrgrovzx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wutrthqu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zclcdmfg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wbxgojin.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kjbcutvu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2spnbmjtl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2efhlxsqv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fewbnhgo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omubdkau.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nkuhovcf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2awlrlfeo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2smipipzs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkuucap.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gzxeocbj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ictrffir.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2aqhscdpm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tunvcrjl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wcwvichm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rzvkjwhd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2egvvowms.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qimwrhaq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2esezdkke.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2freciooj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2inwsarha.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2twdrhopk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pmqiqrky.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mrzsraaw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2filmhwlr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2izbvdwxv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mmpslxer.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hphttntt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zffwvlgg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2engzosed.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2daazsaqb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2iijieijx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dntmlapm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkfwayzb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxpipqeq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2glamjkib.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bdlizdwf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnlpkrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xopkinth.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ugfgbhqi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lircgots.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lzjrwsrr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fayvrajx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fsnluyyj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mvrqtkwy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hxhgvopy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hmvvybvf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2snnhdnci.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2kzqmogvb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2clazblea.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2scikbqnv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ruduigdq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qesursed.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nitxrdqg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ebzyyfog.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fjahdali.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fhnhwsba.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bcjysbxp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rxwqipik.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ctaxzlgk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2johndusz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vvnljrwg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2yttbedjj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fcdxloaj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ixuyupzc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zfefjnac.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2otigaipx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2czlaunqo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cwcaicun.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ypauewio.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mjljeuvv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2spxrlgrd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ycnznkzj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bjmreweh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gopvhrsb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ecdaiudk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hkecnbyi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mgunieqo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2shdpxqpd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fceelwfl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2clnulexr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mwzzxmal.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2amfkxhet.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2apilnusd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sukcqcep.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2twjyvsce.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hzjsdhji.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mavzgzcf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bromtthy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2apbzlqlv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qxysztgi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dfrgbzre.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yqbojppy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dbnkbohq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lexesnrt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xhnuyosi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bdiiyuwz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dzuxydzc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bicxjrsa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkhpwcxm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhnyaxp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfdvqlk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2whosivcv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccoojter.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2iccrrvpm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2myrtlgeo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bvdyvrpw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqdtjwap.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kkviwzun.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ffritycn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bdptkxaf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cgxbntqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xujudqcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vbboqbtu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iwokszys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uoxeqjbj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hdxbmgys.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oqfnvzjq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2sdoecodp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjypjyfp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ljvhvusp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ctgrcazh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jvditcgr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2svfbyunl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mssfwzzq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2btqwmltl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zvbprmqz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wfbgtkhz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pvgqmndp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2skqklzud.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xnfsmcxz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pngsyxdr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qidelmlu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vjihrcvp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2romyyulp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xnwqvaqd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hydsuzvo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlizdley.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hgvpjbnj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cbfxmnnn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmeluspw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uluqfnlx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ptmndylp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fvhesitq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zupkxtjh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vodjcxtd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2grwlfphb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilqtwbtm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xgzslvey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpkaeouc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vtlbsiee.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wczxtxft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yfgcfemh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vtcwitik.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ahaltost.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hqzrotmd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2umdthgzp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xfzpnxfz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2shhzaxcb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntaxqrcr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2irigdpzd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kxcgmopl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwrdfaof.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ktwdkqlv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lgdoxnrn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2giwgkgie.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ivfmukay.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vcxbcrmx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tagcglwy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2brxztuet.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ngjphtja.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2brwscnjn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uldqmybx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qgprbmuf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xupsopql.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2syiuzvuo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2urobidql.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rmigvtbk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2smsniwlf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kddizvyh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2txxqjqig.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2omoesrwq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sjddpxwn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zfbygkli.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pnjuwmog.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ucqshxvp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ylnuganb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2geakuqtj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2naidscgr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dxrtrbiz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jxznshag.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2maorjvot.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2goflnsmi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rollrvse.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2krnqevls.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fkcqjlac.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lfluklur.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dkflttnl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yywjxjwe.html


<!-- 参考信息 -->