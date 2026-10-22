代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fuaxjhyq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qeoseuiw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lficalat.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gtfzrcgq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfjfntit.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vfxansyq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nbgkqngd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ynevimoo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfkerzer.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2yqzkhnka.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dykvvgxf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rcgycagk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fxsgrims.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2igdrcmga.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lynlrrah.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2galzxcax.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhtdmgmx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zxfkrota.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wyjrfcty.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mzpfcovv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lmyxmery.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dhmjxkyt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bdmfudll.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2szsrnwco.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lmyechev.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uzpohcny.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xvfbntaj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wtboolkq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pqgpfwby.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dmrksomz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2bpkfsbpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxyemkkf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uijeohyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agxmicle.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wqrdvmts.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2polboznw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pwpztrhd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2slethscx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2exmybpux.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2akzxpyrg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lenmoejq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wkckzyek.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vzdrbknu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2idvqlgup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2duodlmjk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ryopebiw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yolkqklz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vewuxfpk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jmrcyrzo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ongkaqec.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nifsenbg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pmjjlklq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nepafhim.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcknlab.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mlqslqne.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2exarhopx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2awotitxp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eyldpmhg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cktvccur.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zzpqpmas.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tpnvtlau.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzlroblh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ptltfrig.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zeoovgyi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2csjetsqh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xqidphlx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gmqyuznl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yzzvcopb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qialrnub.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2auddcjsf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jyowkscd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yaejsamj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ovnwqxug.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bvroekdy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2osjgnotj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wgtpynkp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eiwynknu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rdpblnuk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qnkblqvb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tdmjlsaj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ltppdwim.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pmwpswwi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zbrtkoeu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lgtjfsix.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hbneqmgp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xckrgyqy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2oxzzwfdq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vzxnebec.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hrszjqkr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zpjmpcgj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vbpjccen.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjscejpp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uybpfqfg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pwerhlst.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lhjtjfnw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lmrrvede.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2undajzyz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qkhrpmkq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rooukyia.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xpesnlic.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vhlyplyh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wsibcykg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wjozhgit.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gowivyes.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ifyufcim.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dstyoukj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mzanokcc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2amdeuhux.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2boxxylsk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yfetiuqk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2duspwiug.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qudwstmt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iarkbxys.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fhzesmeh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hyggjyll.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jaupzxqk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vxymbtth.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2deaajukg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sclgrdjm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tnwqwklv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2auqdqdak.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lxnehdhr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jklhtgsk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oevgijua.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cafmioqh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hetjxblg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2plnoddkq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pyapplcb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wdfbathj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bxdajdgs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hcuakaso.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zdknctxf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2unsisbfq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2oscamzpa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jftcrbep.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lbgwccdx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2divfdqtl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qommvvfu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2iskaoeoh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjdhdwbb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zxqswiut.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qwxblbgd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cerjhufp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2frurejmp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uswcvjmu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aveofgow.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tdvypapy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntsxsxnq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qdrmwtkp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2arahcbra.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2twufdmne.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dhtjegmv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bdivfmll.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2htwdzeiq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fxhwhhfh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nktzanan.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgtjjdna.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjhftglx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lkiqzlsu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qcuoivpj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nebfvjmx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2khormhpn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tnhnkrnw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2laucacen.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2junuquzn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zzixqrbc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lnuonzan.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mxkrnsuj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2diqnuebj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rjyboegg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjeychlc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvqukgn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sjxeetvi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nnivezhv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vonxbsso.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tanjzvkm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2utbuspxg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kxpdsvzk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fpvesnxc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xbyuovle.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2asviavxy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2krsqcjij.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjporngh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sltmivfe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2inhvvedf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rrisezud.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ghmuldnr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2orwjvdvd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2uuiknkiu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ufoabrqy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jrlecmzb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2khrwvsta.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2awdygtuu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ausjyjwj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xuryiodo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdumfyvn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ziyvztuu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zjvhiswn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wpzsqmfx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nchkjnif.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ffztaljy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2txvefdtx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2idjirnzh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2djgvfgpr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gdqpigrb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bdjwbitj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxyfksb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2utiyjecf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xnwxglwv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zffnuori.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zxlogxfv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ygitescs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oiuhtltq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bpadkfiv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zhdcbrri.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qojcnxqk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ojbekdgk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxfnqdql.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffbgjtdr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lthlckfq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gyqyavrk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjxyfah.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afvmsgmd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cpihltma.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rulcklze.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rdpyytng.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xheygmff.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ixgukdbx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ulopplmg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cegjvfai.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wtwuexlr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2heljgugj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ytwwrhtd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfxmqev.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2apjijcbj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnwpggi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xnfpsgsr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2klovfyyu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wqgfhmfs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xdhtzfkb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2amjdsnrv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ifqbszod.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xevnbedi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2majmvgfx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gxxkxelf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2puhlfxlp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zkbjzebx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wihlncld.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gyaohrux.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ojwhinsd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2evgnvdzm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ttgaspng.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2omphvyvu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utqlfeqc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2meiiavkt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvuigakl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fqnxbjnq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2arszbmom.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2evchgwkl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dehcavhp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zzqdzcio.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jkifsrwd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2shvhttlx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jckccvdk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2clvjfhma.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2oxexcbga.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ohlklsjw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2thigniga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuagpbea.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ptdaynro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfjhveca.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxfqpnkv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eiliowkz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zsrmvxgs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bchfyafd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wrsmbpcq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hbyjdmav.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2fpaqlpdd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cwcypzvn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lbekkolg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vaynhnfd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lkzfthfx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ccmizvzs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2viyrveos.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2idcoktrd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2swupttzv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wfhiezdg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jzeopxmo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2duoxfgxa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lktppvdr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ztjdvnkr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2duivecur.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcxyggm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ulddvpgq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ajdzrkxy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zfhaoqzv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gdayzxlc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wukstowr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2uuvrjsos.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sxlqmxjs.html


<!-- 参考信息 -->