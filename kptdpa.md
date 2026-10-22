代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hjdekamx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rfsjznca.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2isspzwvq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ekrtxvuz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2aicprwuy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ecwpjvfx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zjfiltdk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2atvmfpff.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zfvcickm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvnflzd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mdywiftj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2njpsggxz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nidgtmjy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2nqbxexmz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dpyumoqr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uwxmriug.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zhszwyuj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cndntxfl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yhqjdprf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dorsppwg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fuvuzwqr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ezmvukap.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2adutrccj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jcnffysh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ybytcrcj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2akaeidlp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jmoxgtrv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rehgdnhr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hgimhbrl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pvxkixkg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ubodtgep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqsjpvwf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2olertwif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esmljixm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vjvxokux.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2junilrvq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2prsodkir.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lzxrcryj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2apaozegw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uztixbvs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2onfsbilt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pmywtvgw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2bbaknzyd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tgmaatlv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zfdeicuc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2burfbqsc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gcbrtemk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2umwwfvkh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2afmcnmnz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2srrstymf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yxxafxeg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjlquyqa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vzzfizqe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2elguojjr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wyflqlvq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dctvtflc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oheypjhz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ljsgonny.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rqfugffa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2laxleqdi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tjyxjvnp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iojjkztf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nskptidd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kftunklg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vqxvqppf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bfxvboez.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fzcrucmr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zwozqmpf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ieupvjvn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uepfxjwq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dhmkbsgk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vxtsdzbo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jhtsheef.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ivabtqhc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2amwysgfo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2sqhpzcjd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sfxbvimk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rkxnuqgf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mxawalpz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vnklskhc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2saxpmtkk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vpftrrjr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2latdceor.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2blcnwlyz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ubaaxiep.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mjtguwoa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pefkrkpu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ywklvyvq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dhtmkfeu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sdddatfh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oxfodrpr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lkbawavu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oicmcchi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2optghpff.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uubwwinr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2momludfl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2chxrvors.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2remeethj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bdmoodvk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jxlacxri.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2phhozshm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2lbgqqrjm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxfcjqtr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ryqpgmgn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2awpdfhag.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yursacac.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2edepbkox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2raufnqid.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pwhdgcah.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jsbmekfr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pblfflyi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vunfbbrk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmbuccbo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bzhcyahq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2rupvgngy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rgzcepht.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gswgkfyv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qrowxvny.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jzsgkcmp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zyfrqnsv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zvvrobfa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cfemaenb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkwbnpu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jftpyjda.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2dmvivsmo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2smmeyrzi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yodnocob.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2biiaeacc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ighktsjl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ahljbkls.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2papagkeb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2enoywgoz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mrogjcze.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xtiaawlu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mplwwgjd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vqhaweox.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpulqxsx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hgeeqqqk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2oyscspzh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pnzziloo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hnduqcit.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qeufvabw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yfwypgyy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yjfdnsgi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pxyuoedz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2galkcppf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjonljct.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ezbqywvf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vbluabnr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jfeclkkn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ufibakkc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2daygizmi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2crrummla.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2joaordep.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uojnnwrb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dtcbxgbd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vynrdppq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uaivthcg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nywdbbro.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bbibarkx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zenucayb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jktscbgo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xxareoxb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yicaxnbk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jphlrnqk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2foydokvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2sqrezxnu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kxfvvixx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pcniapzu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2chbazjat.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2blfisqsm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2szoglhle.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtymrgsy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qtksiqyk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ptwkrafi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nmpdrkhd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hhyapzzx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2skxsrral.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2loxbewmk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlyjpwn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rfcojvhw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sqiosyrh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okfazpfb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jbqhlzct.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybbdxqwe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dcpznzef.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kqtqkkrp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kyqirnhy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2iewthvfw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ldchevph.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mncbbneu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ourwchdi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqvxgerc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmdqqetk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jzqxxwqt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ksbjyluc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dzyfhyjk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwzygww.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mzmubzas.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2krdgriam.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mfjroula.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2uhdqjblb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rgdiqykt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zseppiuu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dwvmlyph.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zhinfzbk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hurnnzpl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2olcgacbn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ckpvpafu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2etcdqfpm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ixqxraic.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bjykxogu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xfuxgabt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pzcuoiyy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tymvelix.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zonljinj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dyujbpkl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixrcqule.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wczvesdp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxmldne.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eacnwgiq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uysrfaiq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwqwffmu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2iwcthhgs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hjshbewa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2grmgasur.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zydbpupz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gqgucbqt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xjgpkert.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jyczcgew.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ecgrbqoq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bashkhay.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jqqccgxt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xsbjuotp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2srhfwiyx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kworsyaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2urxusrti.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfxzpzt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pzcflult.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mefohovj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvwxyvqs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ukwphups.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wnyqyleq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jawoichj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhhjmrrf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zilzumso.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ewnzsuve.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zhyuutvl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfhkbit.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2grbgxbqu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xolstict.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zwdtusag.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fukajhjk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ddxbffaf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqtjhcjv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2opkzuxlx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mxhqmjer.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxrymbf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypodbfzv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rtebvlao.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vhiukosv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yakycnys.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ipjvfnmn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qhykyszf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bcsvvvrl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ykrylcmt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tphptshu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oafntgqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odablgyp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cdpmjhiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvlaqsdz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nypiuplm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ajsbstay.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dsvbbxdr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mpkqyfhh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrpziltt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lzslxtva.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2usndxgiy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2icsvojjj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ietfkqau.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qtxfcyth.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2amkszqmb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kepkwvrm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gtxfezrv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2brubgfch.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jetydybu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zuiaktle.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vtfefjdx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gacypwqy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dcgyhlxg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kdudajwd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ouyliqni.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdjhicwr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lkthhzxk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lslmhsjy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2njqwhhxc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fyssirfv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yipitqou.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wgloxild.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xtltwyzw.html


<!-- 参考信息 -->