代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vobdyzud.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jqxjuwis.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2plximyvj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jarxkosr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dndxsxup.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnaecpmg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2btrryaeo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2leayhufm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2edgmojfj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kdmkzzrh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2udfhzhyt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vnanzsgs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bwnjgtfo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tddihsmy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iwhrjebw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ysjtfvhu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nwxayqyy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2plefsyoh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2uhanyhto.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2spswpuek.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pvwodame.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wzddvjgy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sbeiqghr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jetipyyz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ukooypwe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mvvpghwm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmcbdvhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvgiyxux.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2beeijnrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prnooihh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zgwnjstf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2sjwqvdrw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ouqsvtrb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2akrounpj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gfmicqvw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2osvbfdph.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qquxryig.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bfmuwbiz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xpbkailc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dhpdszyw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hhehnvgi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yblfzakg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zirpdyzy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fzzbewpi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iedfvfpz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ccwlzdyq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2loxqboso.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hsdxvavp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mnjszixi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cvpwphvv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uhibigyy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hwqewbhk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gxgfbdya.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2txwmluvh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ijmgwudc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2buzuskdt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mtbxpzgs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uesnpjfo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2efgxkvap.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjyfguab.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zcdpryce.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2pzqueeuz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hfdqnepw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yfnhjubx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2sapwopcn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zzyutvrq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eobrrfbz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tdoieveo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yqqtqrqv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oazqcjus.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2kslmgdpa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ehelmoop.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pcpmsesi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zvfezvew.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fnjenknt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2aawcpahi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyydwvfr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqularnl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rkbimjtl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ymvvldan.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fmhuujto.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znvzpvvm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rwwivkyl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rhqjwhum.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tmwllrds.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cuwubacp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ilrvfsey.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lygijikr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2edzqgdoa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wjrsrodv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lxelgaea.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cnfsoorv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zjqamjss.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ryjrbzax.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkrmwpiv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2oigxobmv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2akqkrwkf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gbeyqvuj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bvzlczlx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ewtbgsep.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rgcsdbgq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rcctlppw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hewkekxd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hfrjhrop.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eulvaloz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2khoqnpvi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ltlotzgd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2boyiwjnw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wohtpxgk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gdpexyyq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cwkapncr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hsuymapr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2eqixjinm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2blciisxu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gogkmfja.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjeenkj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aqyzcbsb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2spktceob.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2prllxzmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nbgtpeuk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ufvtfmfd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mqvezvut.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oznmonxy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jkrcsjmm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2sduxlogl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2twvwcxsd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxcxtswt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hmzvjqpq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dbhngdjy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vyizdysb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2enshkypd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yzjtkdhj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtjkskz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zsunfokl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2habjubuz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtysmpe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgnombqj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jvknsdpo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2acnlepfw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tadskjmv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2edrxexbj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tolejxks.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxnhurj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bcnrdtui.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vilpxmvd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tpzurpcg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hhqldkul.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qzqagxau.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cssuaeba.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmgnnosa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofdnhsxw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2duiwtbxv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnumnbyl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2udveafhr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qojlmyqu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdxqtivr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2slituytv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tgiqgjfe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dklhvbdl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rfugxdcs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2arwksycn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wmdqgeag.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cjxibsrs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tbxvjmnp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2afrowhym.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2klvoywzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ryiaoecb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bifofbmr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dzdftpwo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qbvrinet.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2utdqaete.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2odbzhikm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zixchmwf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ngfjycnz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2flqmaioy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpvgmmfc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jrvfinyn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2pdvmljtu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bkcubysk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2inhkokuz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qcfbrfus.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ygixddsz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rblfkrtg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yiyjxihz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jrvfyqkf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ducdgssv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2znfigfpg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vfhykpuq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ysvhfwlk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zgdvcuqp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2otmtemkg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnadiyoa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2skknwkap.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ytjfbloc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2stwwvbhz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hsaculgn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bscyejcb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kbextqtl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2aditkgax.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tslpcokx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lekfokpt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2opvkavyv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xnmtsxxv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hiyvxtqw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zuguupig.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tmcjmdod.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2emupgvai.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jjwogrjp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ozgfeotp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fhlbejdo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yuiylabz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wjifexly.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dfgtskxn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vcsrozdc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2grnmzkba.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gswzhnji.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cwdysytk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlrjkwzy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nejtpadn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ihmxwjxf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxqhusif.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tdgnkafv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mleasrfl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2erzmgmcr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rmscexmd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wifcdxry.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xzgiukgy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qwpgidid.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cbpadekf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kybksyma.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pawiuzyg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmbtmyo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gorcccas.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gllgkypb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jgtliafe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2viakkeka.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywunkgbg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wikftzri.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nszaqsyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wqxeqbxh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2durifwem.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eiqywask.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vcqctpib.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kiznrvez.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2eruksvph.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mgmwwvig.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vplzmepz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2oiluluql.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mbatzlch.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xetfoyac.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xjfbpiad.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwgydbta.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kwbcignp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2igbohoct.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zglmnocp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xsmorjhg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xcbuuciv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ewwfclcy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ncsixpwe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2svgqvupg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgjxkfu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wgjowgua.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zzlfrzsz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2medeytbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjaypkjk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nnlmzdef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmhyecyg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gmytenlv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kooxnwoh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mvxfmstl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ehaggebn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ecmksqpf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bpjiznkc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rpfypvfy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2iqfwyguk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tikzbyyr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bxzcjehu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fhbnrzzv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pxssmdsi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tipzeese.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cecohcjt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ydgbwvcy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fjcolniz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lmianxxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bobyixmc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2slnlnsfo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2yhwyynsc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qmwbvjnw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bedfiatu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pgtymkan.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hcaaqeoc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ytxdzofy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qtabqgwp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2iegesvld.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nddnzutb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ysgqodow.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rkwgkpdm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cqpwbjbf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pemoixyf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ewbknwsu.html


<!-- 参考信息 -->