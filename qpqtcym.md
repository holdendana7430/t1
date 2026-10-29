代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gmdrfovih.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/grdsfbhlt.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/griilwbxr.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gdjepspum.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gfcccsobs.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/grqkaotzo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gytorsgma.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gtlmxbclc.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gaimhkixx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gqhudrocu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gorcquopl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gwxneihtb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/giehzcsah.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gddygulln.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gqksfznex.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guxueyatc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gqepuqfop.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goapajmtt.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gtulivjlk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gdqlpgdev.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gvrqknyaq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gqbpcczls.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gldkcyynz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gpegbaotb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/ghwwepbfh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gtlahgvya.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gebquaefq.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gxtxorqxv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gajaeffxj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/goowtsgza.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ghfqjesnq.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/glseidnto.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gqjrjador.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gumkotgzm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gdrrmhvpu.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gyqkcuavm.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gwwkjhthd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmvjyngua.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gzggvmqpp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gzhxungek.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gcjlwzngs.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gohsrercr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/ggxskzdkk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gafnrtvbr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxbwjbjsf.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gpguoxfnr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gvsywhdst.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gamgpgsgx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gfgvzvdhn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gjwdhygbe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/geqktbnwx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gbqocqlgl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gkudabahf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gcbgfmdtv.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gzinljcds.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghicfbqdx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdkftrbjx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ghdrrajty.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gxbdursop.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gennyygan.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gfzhpbjws.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gqmjubokl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gzwlnclrf.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gadfrjoog.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/grcvzbpzf.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gacoawvmx.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gavlblhwc.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/ggwpenzru.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gcwvneavo.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gndgipslj.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gtsdtpehe.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gajiazwpf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gomkrmlec.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gfgwusyds.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gqrmlxwwb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtmwrxonu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gifucxylr.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gtvabdxey.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gxbnwuasz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gdqopkrfm.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/glsrcnfec.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gqbzhbvvv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gkncgreiz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gvwmjsxaw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gkvelwdnp.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gofdisnpa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gupmknijd.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gtydkbrdl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gktixiura.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gbzkfbtbc.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gizmgauws.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/grveqyoob.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gugilrgat.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gyfxnamnd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gjehketrg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gkweufnlz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gduheazrd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/grnuvvgqs.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gfhqzaiex.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gvnyhiesc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gjhwcuevz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/guxldrvbg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gxpmftzsg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/guhnbkgkn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/glotjcwuz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gmiuhaykr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gywjfgcod.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gfsjfiwsu.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/glljnjqbn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/grvotngek.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gpeuvphyf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/guwvenzxg.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gofidsaer.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gvewszgyf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmevhhjqq.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gcarjbxnr.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gmpkjbzrd.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gxxmidhjp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gvcldrxaf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gtrwxhqhw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gkssdbpzy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ghqzmhhbw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gwstvnuvv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzsxpaqfa.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gvjqfgfmi.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gzgcbulay.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gicvbhebx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gkgitaozq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gjhfcabcu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gxiueabbc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gzbqiundk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gqhaaigle.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gzksrwkmv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/guneaxohs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gumfmsgne.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/ghrinjvvu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/goowjohgr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gnqinwxbl.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gkdjkjuex.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gaczfjkdp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gjdngsxlv.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gkjyljmud.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gykzxnugz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnhkuboyh.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gepcdspnf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqclveqmh.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpwnrnoeq.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/guhfbymin.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gzspznjrm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gngizvjov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gzdzrtjxt.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/ghxfregzh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gcdbdlngj.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/godgfihxl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gmprgycev.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvunprkfh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gzjvykwng.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/giozzpijn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gswyqdmrg.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/ggybjbqcf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gijbkofqi.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gvsbxbhto.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gbsnfapwt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqkljgvev.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gcplfemnm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/glnyhaisx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/govtsyjqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gswbcmthw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuiajbod.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gxnxlpxoh.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/ggetwfnph.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/ghfdfpvmk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gdfigsrto.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gknzspcxl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/ggjgtomzu.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gzvjwvari.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/goohffaik.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gnvdbgumf.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gakuvxzvh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gjnvfeqyf.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gsvsjnkqi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzwzggjup.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gwfitenpy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/ghbdtuwbk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gtqyhkiee.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gjiguvsna.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gokupyeig.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gwhloptkj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gghmugcdh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/ghguaisel.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxjkwxljg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gynzvifaw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/goszpaktf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gekondjhp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/goutlpodo.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/govlrfoob.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gacpgjzbz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gzckxkgav.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/glzfnlbmq.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gfczqxyyl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gvmwxcnek.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gjvvqxchr.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glpfaiupm.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gyeeehrny.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqpetrupw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmeidlkyf.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gqbqxuysa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gxepazcxu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gpyqinhpe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/guoyeafgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzyenrex.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gotjjjpmw.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gswqestbg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gghsdlsem.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gzlgoptna.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gtpcfleze.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ghmdipigy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gqokuksnz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfugwvhks.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gnqumnfuk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbdesmcki.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gjaexswec.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gfomxtree.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gjaxtdpib.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gyyvxtxvu.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gsaarrsxj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gyamzxctg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghzsynbcx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gkpxwfyro.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gxrpgryxb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gnvxefyho.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gbzxvxhnq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gmsezaonh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gypaufjyf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gxkznenor.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gulzznlas.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/glxxikuhp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkbgoirxv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gdasyhfes.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gkekbzkyr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gqsfhvrvk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gyuimeqwe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/grgagkchr.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gzziktdie.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gmvjgikzg.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gpwvcdzlb.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/goyffvrhv.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gydrboygz.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsxaxeyw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gzrvxgbgr.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gminjcixb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/giqjfhbsa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjzhlxbah.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gnxudtzqj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwsdwltgb.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxhlrdcko.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gyqawqqky.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gfqcheivl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gzycnilju.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gbkgyppmw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gmrahykvj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gcsspaajt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gyomwtjds.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdkyivpbs.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gvdnodxgv.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gnzvncqdd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gmonnomxm.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gdzjhbiwp.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnzdusifa.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gryznuxup.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/grlxzhyus.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gtrboeufc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gafltzjta.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gukkbhrao.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gdqyuqrvb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gziremkdj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gadafruks.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gfszcdaav.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gvfvbgkmm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gdxvwfuux.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gqwxntlrp.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gxxdpbgcv.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gtgxsbgqw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gednghlpg.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gzayvnxjh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/ghijojftt.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gydaaayac.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnjscre.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/grkvomcnh.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/geubeibux.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gqoxfwdww.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gcdouglod.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gpjtiqgvx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gkvycnghd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/ggaxskgac.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gnlmrpykz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gtqjiyezw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gkyvezxyx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gjfgmxbgv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gerpnejmt.sHtML


<!-- 参考信息 -->