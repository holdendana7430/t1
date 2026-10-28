代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtklgcnapx.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtmfocdhku.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtofitrukt.html

[R55] 压缩与解压
来源：http://hz.sxryk.cn/gtdjofhowz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtiyyplwbg.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtbtaeyyzi.html

scp file user@host:/path/
来源：http://hz.xylfe.cn/gtdiadydlq.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtzjsdojvz.html

ssh user@host 'uptime'
来源：http://hz.hywenlv.cn/gtvuvqliyv.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gthloslcru.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.smart0.xyz/gtmmoyglax.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangtech.top/gtvzrhstlt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtyauwrxqw.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhengqikj.top/gttngluwpp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxinkj.top/gttdgiuang.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtawtelxse.html

df -h;  du -sh *
来源：http://hz.shuidangran.top/gtntstvmlr.html

[R62] 找最占空间的文件
来源：http://hz.sysykeji.top/gtigkhcmvl.html

du -ah . | sort -rh | head -10
来源：http://hz.tianlin.xyz/gtievqqabx.html

[R63] 内存与进程
来源：http://hz.xuetiantiany.cn/gtnnnccfjq.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtjgjpcebk.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtfpassslz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtmatushhh.html

[R65] 查看端口占用
来源：http://hz.cucudq.cn/gtuupomvnw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtmpqppneh.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtubjtlihc.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gtwypralfs.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtdnocckar.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gthiboewtg.html

[R68] 计算文件校验值
来源：http://hz.xuanzx.com/gttxdukigu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ybcxt.top/gtqqwytbrb.html

[R69] 生成随机密码
来源：http://hz.daria6918.cn/gteyppytji.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuanzx.com/gtfdqqykpv.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtdiqecbjw.html

date +%s;  date -d @1700000000
来源：http://hz.sufxvd.cn/gtgsjabbvd.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtglhualfy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtembijngy.html

[R72] 等待端口就绪
来源：http://hz.dianchejie.cn/gtnkrfcdti.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shuidangran.top/gtdjuzkwrw.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtozftxbht.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtzqqqawzr.html

[R74] 批量重命名
来源：http://hz.yuxming.cn/gtiqvgyvqq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.havefunace.top/gtvvtrunyr.html

[R75] 导出环境变量
来源：http://hz.ybcxt.top/gtkqaglvap.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtqqczifup.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtbeqckxwm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtwibkmflp.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtsnokngqd.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtkuidcjjc.html

[R78] 交互式菜单
来源：http://hz.jianghu66.top/gtiwnjxojr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtsqcaupdu.html

[R79] 解析命令行选项
来源：http://hz.gotoacloud.top/gtuqbiybkp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gtgwzmfgqi.html

[R80] 查看脚本执行耗时
来源：http://hz.jiagoushi.top/gthjwaigsr.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtebuaxwrn.html

================================================================================
来源：http://hz.quarkkingdee.top/gthbvtuvps.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gttppxnzmt.html

================================================================================
来源：http://hz.sxryk.cn/gtzgwlkvvn.html

[S01] C：Hello World
来源：http://hz.xziqi.cn/gtwifdsuyr.html

#include <stdio.h>
来源：http://hz.zhongyouzk.top/gtzuddgrgx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtbkzrasnc.html

[S02] C：变量与格式化输出
来源：http://hz.c1oappe.top/gtqkbbdqlc.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhoulong.xyz/gtlmiugwlm.html

[S03] C：读入整数
来源：http://hz.haohaochexian.top/gtatyoctws.html

int x; scanf("%d", &x);
来源：http://hz.fengsongda.top/gtnjljundu.html

[S04] C：字符串复制
来源：http://hz.ywan-chungtsiang.top/gtsdgvhvgp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jlsjyb.cn/gtpkisuwrc.html

[S05] C：字符串长度
来源：http://hz.fengsongda.top/gtvhkqbkff.html

strlen(s)
来源：http://hz.0kj1m.cn/gttgkbugkp.html

[S06] C：字符串比较
来源：http://hz.zhoulong.xyz/gtiucnckbf.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtfrzyiowz.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtnuvbhryi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cucudq.cn/gtsaxmavir.html

[S08] C：动态内存分配与释放
来源：http://hz.fzhhl.top/gthdfyolrn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nwbrower.top/gtkpskqrrs.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gtxrdsntiy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shuidangran.top/gtbflxsdow.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gtvoaulyki.html

int *p = &a;  *p = 5;
来源：http://hz.xuetiantiany.cn/gtxsltnzmr.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtadxfiqus.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gturzdzlyu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhixingplan.top/gtpeysxyjh.html

fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtqmjmzwxe.html

[S12] C：写文件
来源：http://hz.kuanghao11.cn/gtymedmojz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnxiangtu.top/gttgajdltp.html

[S13] C：宏定义
来源：http://hz.52xcode.cn/gthxdikwon.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hammf.cn/gtkieqgvlj.html

[S14] C：枚举
来源：http://hz.pycfn.com/gtrzuaqfmx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gtuhgqbzei.html

[S15] C：类型转换
来源：http://hz.birdmap.top/gtibclnhkr.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtrjcikaap.html

[S16] C：位操作置位
来源：http://hz.yueranfly.top/gtjijymvgp.html

x |= (1 << 3);
来源：http://hz.iojbl.cn/gtzmuymbzo.html

[S17] C：安全拼接字符串
来源：http://hz.sufxvd.cn/gtssbrokbv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtuznnnmtt.html

[S18] C：命令行参数
来源：http://hz.jqgufenzy.top/gtauhhrmbz.html

int main(int argc, char **argv)
来源：http://hz.0kj1m.cn/gtrafoabfp.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtxlgzmktf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtoogytojw.html

[S20] C：二分查找
来源：http://hz.yueranfly.top/gtecwgfshq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtavvdzsih.html

[S21] C：字符类别判断
来源：http://hz.jlsjyb.cn/gthboeismg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuanzhike.top/gtvmtyzktl.html

[S22] C：字符串转数字
来源：http://hz.xuetiantiany.cn/gtdnirzjug.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daria6918.cn/gtujaemmhk.html

[S23] C：随机数
来源：http://hz.hongshengwenyu.top/gtotjwjqlt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.quarkkingdee.top/gtdaganlah.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtdgveatwi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtephzkuqc.html

[S25] C：内存拷贝
来源：http://hz.ivvv.top/gtoubwcati.html

memcpy(dst, src, n);
来源：http://hz.redwolf501.top/gtpdvvdowc.html

[S26] C：内存清零
来源：http://hz.snrcjt.cn/gtjcwlhefb.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtvwiqpifd.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gtnwzvcczc.html

const double PI = 3.14159;
来源：http://hz.yj202588.top/gtkijniqbc.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtexvwpbud.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtnriubyhz.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtesnslcur.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gtrgrldseb.html

[S30] C：头文件保护
来源：http://hz.feifeiyinyue.top/gttlhvwkph.html

#ifndef X_H
来源：http://hz.xuanzx.com/gtihwwiake.html

#define X_H
来源：http://hz.yj20258.top/gtjgdatobj.html

#endif
来源：http://hz.tanke756.top/gtwhfyezuo.html

[S31] C++：Hello World
来源：http://hz.316326.xyz/gtxegezskr.html

#include <iostream>
来源：http://hz.tian-w.cn/gtcmyaleum.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sufxvd.cn/gtgijkvtfp.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtxomdlwhl.html

std::string s = "hi";  s += "!";
来源：http://hz.hywenlv.cn/gtpzvaaprt.html

[S33] C++：vector 增删
来源：http://hz.shuidangran.top/gtestwrgxt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigfzy.top/gtedxhmfsp.html

[S34] C++：遍历 vector
来源：http://hz.chenlongwang.top/gtemxwjctm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gtkabwhcor.html

[S35] C++：map
来源：http://hz.hnqzz.top/gtcpkkbvlf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtwgpiefsq.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtngijtlzh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtyjiehidi.html

[S37] C++：set
来源：http://hz.iojbl.cn/gtahozxdvf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangdashe.top/gthowjmimx.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtndejgags.html

std::sort(v.begin(), v.end());
来源：http://hz.yanxiufei.cn/gtdrsoqvcu.html

[S39] C++：自定义比较器排序
来源：http://hz.jianghu66.top/gtnuuxtrtw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtmdggmrwl.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtmsdpqoev.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtnthhuztn.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtovndxavi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yvedp.cn/gtniudtmsv.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtljwxkszr.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtubquwkks.html

[S43] C++：智能指针
来源：http://hz.aibaodan.cn/gtoazjpmjr.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gtbgixbcrx.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtucrcxiot.html

void inc(int &x) { ++x; }
来源：http://hz.chenjidiqi.icu/gtcfexgcwu.html

[S45] C++：lambda
来源：http://hz.mhx1999.top/gtbwjgfpyr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtjcwguswk.html

[S46] C++：函数模板
来源：http://hz.316326.xyz/gtfnztiail.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtpxndotat.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtmhjldnmb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jyoumei.cn/gtsbjzoydx.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gttcuwrxrr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtwjoqrpgy.html

while (std::getline(in, line)) { }
来源：http://hz.gogol.net.cn/gtqsrwixvy.html

[S49] C++：写文件
来源：http://hz.zhoulong.xyz/gttuzsjnaz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shzxlz.cn/gtaucqksom.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtsirycbbu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtntdkmbak.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtxponvure.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtcimtofjj.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtctpyyliv.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtavlheyue.html

[S53] C++：移动语义
来源：http://hz.zhiwuduotai.top/gtcxwrfsjh.html

std::vector<int> w = std::move(v);
来源：http://hz.ydjk.org.cn/gtnonwimdo.html

[S54] C++：异常处理
来源：http://hz.kuanghao11.cn/gtqbvttpbm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuanzx.com/gtduxixmpt.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtzqzqtgrk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenlongwang.top/gtgfuqxwwv.html

[S56] C++：optional
来源：http://hz.cqqwz.cn/gtpgamryyr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhoulong.xyz/gtdinzpfmm.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gthkjcrlcf.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gtgsjhccfv.html

[S58] C++：命名空间
来源：http://hz.jinghuilouyu.cn/gtzazvsnjw.html

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gtfytbmbdm.html

[S59] C++：静态断言
来源：http://hz.zdqjudy.top/gthahlxxrz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guowangkeji.top/gtdylscoke.html

[S60] C++：遍历并删除元素
来源：http://hz.fzhhl.top/gtlyhwblmr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258888.top/gtjhcuagoj.html

================================================================================
来源：http://hz.dashuyun.cn/gtowfpnoaj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gteezvsgkd.html

================================================================================
来源：http://hz.jianghu66.top/gtfxxvjymw.html

[T01] Kotlin：Hello World
来源：http://hz.redwolf501.top/gtpktyknfe.html

println("Hello")
来源：http://hz.snrcjt.cn/gtbgotwtpw.html

[T02] Kotlin：变量
来源：http://hz.zhengqikj.top/gtbayxonuh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xylfe.cn/gtqpjghbnp.html

[T03] Kotlin：字符串模板
来源：http://hz.zhijiandao.cn/gtdqfeovme.html

"值: $b"
来源：http://hz.jinqigufen.top/gtihnreant.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gthkawmmbj.html

val n: String? = null;  n?.length
来源：http://hz.0kj1m.cn/gtykfwjiln.html

[T05] Kotlin：when 表达式
来源：http://hz.zhixingplan.top/gtudbefuer.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shuidangran.top/gtocfuxjhf.html

[T06] Kotlin：集合映射
来源：http://hz.vqdsnc.cn/gtlkhjsgnl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.9152youxi.cn/gtqlqpnrtt.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gtdoavamfj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtsngxeyyx.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtbiskgqfn.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gtakwvpczn.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtlylcidjv.html

fun String.exclaim() = this + "!"
来源：http://hz.ydzc1.top/gtnrmtbyhr.html

[T10] Kotlin：默认参数
来源：http://hz.shzxlz.cn/gttqlllaad.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenzaomai.com/gtsuwxovsr.html

[T11] Kotlin：协程
来源：http://hz.gogol.net.cn/gtghtkgkty.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gtpzvdxdks.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtifksbebz.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgfzy.top/gtrkjbytqg.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtdosmovey.html

val m = mapOf("a" to 1)
来源：http://hz.zhixingplan.top/gtgtgzvaet.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gthktmpkok.html

for (i in 1..10) println(i)
来源：http://hz.fengsongda.top/gtfrittkmm.html

[T15] Kotlin：接口
来源：http://hz.ppjwa.cn/gtukkakauo.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gtjforhibq.html

[T16] Swift：Hello World
来源：http://hz.chenlongwang.top/gttafcffsi.html

print("Hello")
来源：http://hz.jiagoushi.top/gtkptdfgno.html

[T17] Swift：变量与常量
来源：http://hz.feifeiyinyue.top/gtvqxashlc.html

var a = 1;  let b = 2
来源：http://hz.feifeiyinyue.top/gtnkyzbykr.html

[T18] Swift：字符串插值
来源：http://hz.zhongyouzk.top/gtlzbktbez.html

"值: \(b)"
来源：http://hz.xuanzx.com/gtfinxuexj.html

[T19] Swift：可选绑定
来源：http://hz.xylfe.cn/gtieiyqypl.html

if let n = opt { print(n) }
来源：http://hz.jinyuanbaomall.cn/gtxyclkxui.html

[T20] Swift：数组操作
来源：http://hz.zhijiandao.cn/gtllujnifq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.feifeiyinyue.top/gtfdbcraaq.html

[T21] Swift：遍历
来源：http://hz.cucudq.cn/gtngvmkvvw.html

for x in a { print(x) }
来源：http://hz.jiagoushi.top/gtrrlvjwvy.html

[T22] Swift：字典
来源：http://hz.havefunace.top/gtlldiwrls.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtgmuejvdk.html

[T23] Swift：函数
来源：http://hz.andypj.xyz/gtjuqljdsd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtsmggekcl.html

[T24] Swift：闭包
来源：http://hz.tianlin.xyz/gtqyvkizcz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guannengcc.top/gtpwscllsa.html

[T25] Swift：结构体
来源：http://hz.zhengqikj.top/gttcjnlqsk.html

struct P { var x: Int }
来源：http://hz.jinyuanbaomall.cn/gtfjgqufcq.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangkeji.top/gtlseaotic.html

class A: Base { override func f() {} }
来源：http://hz.nwbrower.top/gtxswcafle.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gttmxcahss.html

do { try f() } catch { print(error) }
来源：http://hz.jianghu66.top/gtuoajjvgy.html

[T28] Swift：枚举
来源：http://hz.dashuyun.cn/gtgjgqcsyx.html

enum Color { case red, green }
来源：http://hz.jinghuilouyu.cn/gtinlbhbff.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtvnwijtdo.html

guard let x = opt else { return }
来源：http://hz.vqdsnc.cn/gtfhcjwiud.html

[T30] Swift：协议
来源：http://hz.havefunace.top/gthmdpzobc.html

protocol Shape { func area() -> Double }
来源：http://hz.haohaochexian.top/gtrpeqqizp.html

[T31] Lua：Hello World
来源：http://hz.zhijiandao.cn/gtndikggys.html

print("Hello")
来源：http://hz.chenzaomai.com/gtuogdmoif.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtrjjufpop.html

local a = 1
来源：http://hz.ydzc1.top/gttsobparm.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtrqcmosrm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.bjfxy.top/gtzteqnkaw.html

[T34] Lua：遍历表
来源：http://hz.yonumen.top/gtdkptlzpv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gaohongyu789.top/gtuftdjofl.html

[T35] Lua：字典表
来源：http://hz.dianchejie.cn/gtcigduajw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hysaishi.cn/gtfzxyurzk.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gtxmvsweha.html

function add(a, b) return a + b end
来源：http://hz.hongshengwenyu.top/gtvafcnfuf.html

[T37] Lua：字符串拼接
来源：http://hz.sysykeji.top/gtvihymagp.html

"a" .. "b"
来源：http://hz.wangdashe.top/gtscdcucoh.html

[T38] Lua：条件
来源：http://hz.0kj1m.cn/gtonvkmprd.html

if x > 0 then print("正") end
来源：http://hz.dianchejie.cn/gtxzbkmkry.html

[T39] Lua：模式匹配
来源：http://hz.hnxiangtu.top/gtdcrtbxdi.html

string.find(s, "%d+")
来源：http://hz.cucudq.cn/gtaehgbngk.html

[T40] Lua：元表
来源：http://hz.mhx1999.top/gtzpmxloty.html

setmetatable({}, { __index = base })
来源：http://hz.shanyushiyangkeji.top/gtkevklosk.html

[T41] Perl：Hello World
来源：http://hz.ivvv.top/gttiwhgjbt.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtwtaueodx.html

[T42] Perl：变量类型
来源：http://hz.haohaochexian.top/gtiyuyewum.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinyuanbaomall.cn/gtfbffbamf.html

[T43] Perl：字符串插值
来源：http://hz.jinqigfzy.top/gtkfoolzae.html

"值: $a"
来源：http://hz.jinghuilouyu.cn/gttybhyjdi.html

[T44] Perl：条件
来源：http://hz.bjfxy.top/gtyqzoauyj.html

if ($a > 0) { print "正"; }
来源：http://hz.aibaodan.cn/gturlxdzcu.html

[T45] Perl：数组遍历
来源：http://hz.cqqwz.cn/gtojgmkpbc.html

for my $x (@arr) { print $x; }
来源：http://hz.ydzc1.top/gtetxnzmth.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gtddevupjt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.snrcjt.cn/gtkhwbavcs.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangkeji.top/gtunerkdln.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ywan-chungtsiang.top/gtsyixbjoz.html

[T48] Perl：正则替换
来源：http://hz.nanxinkj.top/gthzpnslsz.html

$s =~ s/old/new/g;
来源：http://hz.jyoumei.cn/gtxnkrrtxu.html

[T49] Perl：函数
来源：http://hz.yanxiufei.cn/gtvtugdcpy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daxiang520.top/gtzsznymbu.html

[T50] Perl：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtfsltfdae.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yangfankeji.com/gtrcicykqi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj202588.top/gtpsfsajgw.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gtfzvpuxuu.html

println("Hello")
来源：http://hz.xziqi.cn/gtwvrqizoy.html

[T52] Scala：变量
来源：http://hz.yuanzhike.top/gtqfxhspeu.html

val a = 1;  var b = 2
来源：http://hz.zhijiandao.cn/gtgtwulqdj.html

[T53] Scala：字符串插值
来源：http://hz.316326.xyz/gtqngntswg.html

s"值: $b"
来源：http://hz.hnqzz.top/gtpqbdvogk.html

[T54] Scala：集合映射
来源：http://hz.cucudq.cn/gttbnpmeyc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yangfankeji.com/gtsqjsolbq.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtjvunrzjt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xylfe.cn/gtnzvomexh.html

[T56] Scala：样例类
来源：http://hz.chenzaomai.com/gtqtgsophf.html


<!-- 参考信息 -->