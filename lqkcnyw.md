代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gdikphscs.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gpxnblhrk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gzenptlyn.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gvkkbnwjl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/ggfzfpcav.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmihsgpmr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gnvgmpzgn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gxwkytqsl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gmvdcmifr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gnjatortq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gqxprsvyo.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/ghxyapkjr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gykzjifou.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gintayeyu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gkzonzuuh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/grqtrpxhr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmmiklnmx.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gvipiztdb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/glrrfrtkw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gsiprpwen.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gaogauqaq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gtnwwfcyi.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gdaixjvei.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/guulrlwxw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/giwlilywu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gehzhzbue.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/glrprvnco.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/ghuqfymsc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gdnkjehmy.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gmiuhhbmq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gsvrwvarn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gugxqkbbs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gimkfnvtl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/ghvppcysi.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gyjjzthzs.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gzfuynpwz.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gsczgohqb.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gnuyyyxpo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/ghwdxeidx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/guwouibea.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gepqtvewe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gxdxkadih.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gcftsdpyz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gzwqhyuya.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gajklgclq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gyfogjddk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gitfvtlzo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsqwmball.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gopypxoaq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gelusdkvj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/grufeppzw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/genrmoxzv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gwldrrmfs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gqjwvlorg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/goxjchbbv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gqbefixzs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ghrzxwfyr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/ggbxlbaii.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gxdfcqqrg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gihdmfdhl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gbyclwvct.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gduyvomen.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gznagiago.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gublbwsyd.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gziubchvl.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gjirxqrjt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gfppwcslp.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gxlfcesir.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gfqaofkws.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gtgyiqhom.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gyohjjntw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gcyrpnfmx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gkwiksekq.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsnqwqcug.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gabykgcmz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gxpcwkewh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glaedoqac.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/ghyofgwyt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/grlzldsiu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/ggpgfommx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/ggxjixisz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gtihxayhz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gfamitrqm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhwgwwdv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gvuhbcavy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gcigyrann.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gkxpvgdct.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/giiezdkfx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gwsgqezvw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gmihnpgop.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gpcgzdzpu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gjamozgfu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gytunxkrr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbaqqbsjo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gmnacesev.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gfppabpgo.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gbdiyxayk.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/ggoicmamm.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gzckmgnqi.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/glnekesry.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gsrysznyf.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gesavmyeh.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gwmuczamd.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gaibfpqxt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gavdpjday.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gpakrqcmn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/giicpgjxy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/giczkefon.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxtitjhjc.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gkgugvaxa.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/giqtajdeh.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gszocjhct.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gubrulqwu.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gleoamlqx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsnabmsvw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gytsoxgmn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gzrfgqssp.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gbxkdpexj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gsgwdbpju.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjogjds.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gccktaucw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gasbwsrcc.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/goofquzoj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gioucrjpq.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gbkzpzavs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gjbewaegw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/griwdmjts.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gidllfqzz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/ghnzekwso.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwpsdroem.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gtnjbsxki.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/ghzhucupz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gbbmmgdwl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gdmxbcpjc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gtozbbyjd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gatimcjfd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gptswtydm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gnjfgycqa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gsmldapvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gntgehhib.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gejmhxqpr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gyecdsbxv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gzfotjdaw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gbinuqkom.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gcbkurnzp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/geaozgmtw.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gkbvzpbex.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gbuqdfqth.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gjbbxijlt.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwlfdhhoz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/grhlkvhxm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gbjzfscni.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gokogyzkf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gnkdkkips.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/glcnvofin.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzcqqoldw.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gjvckripp.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gexyrjexn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gdzbdiigc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gdzxcwavp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/grdajaoqc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gkvdmcocs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gdpipmtes.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtawvmnqe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/ggyptccxe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gnjubaegw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gtbsunnqf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gzdrhwpwc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/glvmkjtpj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gwxgfyxxf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/glrrfoibr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gxinufytp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/glalnblqs.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gpovjanqr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/grxipfvjs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gcqxfrugi.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gpakapbay.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gtpilvfad.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/getwbvkkp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gkxckcsmu.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gbnxsqkfv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/grbpwargo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gqyouanvs.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gkrbspvps.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/goeeohzbn.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gnpqhxrjc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gnbwbfggt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gldtddodm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gitbeunls.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gpqhcfudn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gjncqlbpu.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gpkpnctgx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gayngkmmi.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gbiilfktc.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gnlnqvkwq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gretguwtb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/grkwuyfic.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gzlqrxodo.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gaeobiseq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gxjkfjwdf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gglrpyiwg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gsdlgsxri.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gqvylicrl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gassruzdg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gjjwfvdnz.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gdolmrmot.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gwgdbkhfx.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gileznbpx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gajjvyaoo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gsxnhfdrz.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gwdngtbjo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gxlqxvzia.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/goguwflmb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gvclulnxe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gkryjnkwq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gvusjoufk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gjfpvvhdg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gfymobxbi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/goheusvcw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gjwotliyd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gpruhmheb.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gcjytzzuj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqycgqzjr.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnvvjbrnb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gbgrjrbwx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gnhptijtz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/glegnlfbh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gazixgqpz.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gzanhgdyy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gdivdwjqj.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gctzcmyjr.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gnrxzvmqb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmppsrhoy.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gajbbbjki.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/grwqpvvaw.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmrzvmcu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghpiognco.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gipatksxg.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/grlizitef.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/geyysbnky.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghonsefdj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gqdsporag.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gokskrgeq.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/glomdlclc.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gpgmferzx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gypsqmsro.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gtpozwwbg.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/goivsofao.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gdnsmbpeb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gejppqstp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gtmdaxmzz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gsjfdulvl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gscgkxtid.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gidpkfvbe.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gzoqlbzoh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gqtfusniu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/glpqjwjib.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gdnvvwufl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gwnrovizq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gkhipsjaa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/grriqwvov.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gzdqsgulp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gfknntenx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gqlpcbnqs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gbxhsrkun.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gtdhkvowk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gpcobowld.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gbmpeswso.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/ghqjpylfi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gxqpymbty.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gbsckcfyp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gelvmhncc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/ggolzdbyw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkblulyoj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gdvqffrri.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gibqoeskv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gkbnvxgjr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gjflhnqwz.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/guhyyyevg.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gvzchzbur.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gpueggvde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gwsbolnwh.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ggbncipnx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gcgesjjyi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gduifbilv.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gnkdrgiex.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdfidogko.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/ghcysicah.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gyfpfsxwl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gjayodvgt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/grzfpyfbv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gaoouqyro.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gqnynfsmu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gkwtlyyto.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gfjqwehkh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ggjcifyjo.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gtfvckcpm.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gqulshusc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gjrbdylby.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnipknfqh.sHtML


<!-- 参考信息 -->