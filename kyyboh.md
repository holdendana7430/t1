代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.52xcode.cn/gtlnlzzcng.html

[R50] awk 求和
来源：http://hz.fengsongda.top/gtrpfsbomk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydjk.org.cn/gtrkylsbbu.html

[R51] 排序去重取前几
来源：http://hz.smart0.xyz/gtvklqidyt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gthbhssunk.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gtyyijdvam.html

wc -l a.txt
来源：http://hz.redwolf501.top/gtytphnesk.html

[R53] 查看文件头与实时尾
来源：http://hz.chenjidiqi.icu/gtkbdiqkqu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yanxiufei.cn/gtorbahcqa.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtikobmket.html

diff a.txt b.txt
来源：http://hz.zycfv.cn/gtmcmmrhep.html

[R55] 压缩与解压
来源：http://hz.yonumen.top/gtjtwszgvd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangdashe.top/gtwiqitcck.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtimhyljit.html

scp file user@host:/path/
来源：http://hz.cucudq.cn/gtyxvxxksl.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtrxavueio.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtueucsedk.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtpwmvyqum.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtytxlhaog.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtzlpdhzvk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangtech.top/gtqnjtajtz.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtzoeiudci.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnqzz.top/gtfypedbab.html

[R61] 磁盘占用
来源：http://hz.iojbl.cn/gtprgghtgz.html

df -h;  du -sh *
来源：http://hz.sweek.top/gtbnsxrluh.html

[R62] 找最占空间的文件
来源：http://hz.daria6918.cn/gtjgjtnoqu.html

du -ah . | sort -rh | head -10
来源：http://hz.quarkkingdee.top/gtiexrulbw.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gtikjhqnmz.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtworklohy.html

[R64] 结束进程
来源：http://hz.xuetiantiany.cn/gtsvuogjuv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydjk.org.cn/gtxqkemhfy.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangtech.top/gthnjvykim.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ehwqpu.com/gtgyseswwz.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtloduonnz.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtlhgcgjuo.html

[R67] 生成随机十六进制串
来源：http://hz.ppjwa.cn/gtqqvwsihi.html

openssl rand -hex 16
来源：http://hz.andypj.xyz/gtxmrnnhfa.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtaphpmkcg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nwbrower.top/gtvvfnvhrq.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtytmxouvf.html

head -c 16 /dev/urandom | base64
来源：http://hz.sweek.top/gtsfheyrgr.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtsysyfhcy.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtywdfizgf.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtckfhoycu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtnaregxpd.html

[R72] 等待端口就绪
来源：http://hz.iojbl.cn/gtltdbsirl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.havefunace.top/gtldjdjimt.html

[R73] 分割大日志
来源：http://hz.pengpengdd.cyou/gtygmajxmg.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtuwsxbmhx.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtpigisjke.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nwbrower.top/gtfijkablv.html

[R75] 导出环境变量
来源：http://hz.gogol.net.cn/gtebryqjxv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtnymxteim.html

[R76] 使用临时文件
来源：http://hz.sysykeji.top/gtxqqgnfin.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtwwjnwvsk.html

[R77] 读取用户输入
来源：http://hz.tianlin.xyz/gtbelfxndl.html

read -rp "请输入: " ans
来源：http://hz.cheryme.top/gtumwhffdl.html

[R78] 交互式菜单
来源：http://hz.yonumen.top/gtvsbkckxe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtfvfahlra.html

[R79] 解析命令行选项
来源：http://hz.tian-w.cn/gtqulbeesh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangtech.top/gtgylybgpg.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtexovsomu.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gtsjvhdhrl.html

================================================================================
来源：http://hz.yj20258.top/gtwrxsbvlg.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtrlmduuun.html

================================================================================
来源：http://hz.sysykeji.top/gtxrinbljc.html

[S01] C：Hello World
来源：http://hz.ydjk.org.cn/gtvrsumpso.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtbzdkxjut.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnqzz.top/gtxkltzibn.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtqhhutnys.html

int a = 10; printf("%d\n", a);
来源：http://hz.ywan-chungtsiang.top/gtrmrcferc.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtadrrevvm.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtkdrflxue.html

[S04] C：字符串复制
来源：http://hz.yvedp.cn/gtbjxyyuro.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtahibwazr.html

[S05] C：字符串长度
来源：http://hz.andypj.xyz/gtaovmmnnp.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtjgctkoxg.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gtbzbahfrn.html

strcmp(a, b) == 0
来源：http://hz.316326.xyz/gtfswwcdoo.html

[S07] C：数组遍历求和
来源：http://hz.yj202588.top/gtsqfdpsle.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.quarkkingdee.top/gtguvbtigo.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtfpwbvsvs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.c1oappe.top/gtewwdooml.html

[S09] C：结构体定义与初始化
来源：http://hz.gzhubu.top/gtbkyvsfjp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zycfv.cn/gtidwgcctj.html

[S10] C：指针与解引用
来源：http://hz.zhengqikj.top/gtuqhgbhsf.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtaxftzroc.html

[S11] C：逐行读文件
来源：http://hz.yj20258.top/gtdpnhniom.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gtelsgvlhv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gtplcsqxvd.html

fclose(f);
来源：http://hz.yongpay.top/gtztilotgy.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtzpqquiss.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtmqonqwhq.html

[S13] C：宏定义
来源：http://hz.ivvv.top/gtuumhikkc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yanxiufei.cn/gtydkoamua.html

[S14] C：枚举
来源：http://hz.ehwqpu.com/gtxlighenm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.meibo888.top/gtutflchpo.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtdyjgdpjs.html

(double) a / b
来源：http://hz.ivvv.top/gtkgzjzmow.html

[S16] C：位操作置位
来源：http://hz.yangfankeji.com/gtsmogtanc.html

x |= (1 << 3);
来源：http://hz.zycfv.cn/gtuuyojqma.html

[S17] C：安全拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtmyfhhvxx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhengqikj.top/gtkokxjwpe.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gtpkqbmgtk.html

int main(int argc, char **argv)
来源：http://hz.hfpthk.cn/gtyivdlewj.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtjnavhsgk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gthiwmoxax.html

[S20] C：二分查找
来源：http://hz.wangshuangyany.cn/gtmztzthgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gticnmexyt.html

[S21] C：字符类别判断
来源：http://hz.hammf.cn/gtjcskpsan.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtufwfujnc.html

[S22] C：字符串转数字
来源：http://hz.pycfn.com/gtupghjcfk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtuajwecuv.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtammezofm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhiwuduotai.top/gtmriwguog.html

[S24] C：获取本地时间
来源：http://hz.sweek.top/gtazypzsbn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.havefunace.top/gtxophjjdj.html

[S25] C：内存拷贝
来源：http://hz.daria6918.cn/gtivjddggn.html

memcpy(dst, src, n);
来源：http://hz.nanxinkj.top/gtiidrirxx.html

[S26] C：内存清零
来源：http://hz.9152youxi.cn/gtclfddlll.html

memset(a, 0, sizeof a);
来源：http://hz.jiagoushi.top/gthcyyjuba.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtvxizwhal.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gtkauqslnt.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtyedjfaak.html

static int counter = 0;
来源：http://hz.jinqigfzy.top/gtlckfydxp.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtgegaeydv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gtwonjwcgj.html

[S30] C：头文件保护
来源：http://hz.jyoumei.cn/gtswyhnqla.html

#ifndef X_H
来源：http://hz.jinghuilouyu.cn/gtxmftcqbt.html

#define X_H
来源：http://hz.tanke756.top/gtdqisyvnf.html

#endif
来源：http://hz.jinqigufen.top/gtrbcnrvyh.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtyjvbgbuy.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtvyzmgxos.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ybcxt.top/gtktnmdzns.html

[S32] C++：字符串
来源：http://hz.chenlongwang.top/gtfcxsepvn.html

std::string s = "hi";  s += "!";
来源：http://hz.daxiang520.top/gtddgkkcsx.html

[S33] C++：vector 增删
来源：http://hz.daxiang520.top/gtxfkbrqjg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtfvpkyyjv.html

[S34] C++：遍历 vector
来源：http://hz.52xcode.cn/gtblbqqzza.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gtjkxgiyiu.html

[S35] C++：map
来源：http://hz.havefunace.top/gtureysuae.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtimgxzsvx.html

[S36] C++：unordered_map
来源：http://hz.aibaodan.cn/gtfscmtcad.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtmjfoacal.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtfkdngykd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tian-w.cn/gtsjqarpti.html

[S38] C++：排序
来源：http://hz.cdnleiting.top/gtdbtrpcsg.html

std::sort(v.begin(), v.end());
来源：http://hz.hammf.cn/gtjdglriez.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gticforhwb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtmbiyddmh.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtmihocaal.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtbmcwcbly.html

[S41] C++：类与构造函数
来源：http://hz.cheryme.top/gtxkvljdoe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtldruvnpw.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtknvwwuqo.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtudldvtyy.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtrddiqmun.html

auto p = std::make_unique<int>(5);
来源：http://hz.shuidangran.top/gtxikwvfnc.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gtfhqmbyxh.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtzjabeufz.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gthmppjtfc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tanke756.top/gtdndwgmmh.html

[S46] C++：函数模板
来源：http://hz.zycfv.cn/gtuuahlzkm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinghuilouyu.cn/gtxtvzradf.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtqfhmlngh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangtech.top/gtledesbno.html

[S48] C++：逐行读文件
来源：http://hz.cucudq.cn/gtnppplbjk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sysykeji.top/gtbdeufydd.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gtkbktqyiz.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gttbzmhiry.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cheryme.top/gtmcvwicfb.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtxphibajq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gttribuzua.html

[S51] C++：显式类型转换
来源：http://hz.havefunace.top/gtxsuqtubp.html

static_cast<double>(a) / b
来源：http://hz.guowangkeji.top/gtkjatbfka.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtykihfkme.html

int size() const noexcept { return n_; }
来源：http://hz.tian-w.cn/gtjjprnfaa.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtyoiljmwy.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gtjyxiofuk.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gtdkvkxmuz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.52xcode.cn/gtdxdmordr.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gtpifwfndh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gtmxjiyskw.html

[S56] C++：optional
来源：http://hz.hysaishi.cn/gtfhnhscbh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gtdfkoehrz.html

[S57] C++：编译期常量
来源：http://hz.wangshuangyany.cn/gtlkmoouob.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gtonpidhht.html

[S58] C++：命名空间
来源：http://hz.52xcode.cn/gtnbzogcqi.html

namespace ns { int f() { return 1; } }
来源：http://hz.shuidangran.top/gthpinhcff.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gtezwfpebj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.52xcode.cn/gtzergovmo.html

[S60] C++：遍历并删除元素
来源：http://hz.cucudq.cn/gtqrfbrmfz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtizapvrqs.html

================================================================================
来源：http://hz.cheryme.top/gtcpcswdto.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gtjkfnlkte.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwkzbippr.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtxybhekme.html

println("Hello")
来源：http://hz.xinyue.icu/gtlovctzms.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtfgytztbe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.bjfxy.top/gtmijiswcs.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtvunoqmmk.html

"值: $b"
来源：http://hz.zycfv.cn/gtgrwnkyrg.html

[T04] Kotlin：空安全
来源：http://hz.xuanzx.com/gtqvcjkkzz.html

val n: String? = null;  n?.length
来源：http://hz.daria6918.cn/gtosbrvehk.html

[T05] Kotlin：when 表达式
来源：http://hz.zhixingplan.top/gtkdyjwpcb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pengpengdd.cyou/gtagdbojis.html

[T06] Kotlin：集合映射
来源：http://hz.birdmap.top/gttapfjtgg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtwhhmrtnw.html

[T07] Kotlin：集合过滤
来源：http://hz.sufxvd.cn/gtfuwryftv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtzufquboi.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtgpsiotgb.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtaimaduko.html

[T09] Kotlin：扩展函数
来源：http://hz.sweek.top/gtwadfrkoj.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gtxukoijms.html

[T10] Kotlin：默认参数
来源：http://hz.hammf.cn/gtzhjthpei.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.quarkkingdee.top/gtyrtoract.html

[T11] Kotlin：协程
来源：http://hz.sweek.top/gtpmvrkuvg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtziklnaum.html

[T12] Kotlin：解构声明
来源：http://hz.ydjk.org.cn/gtofmiivpi.html

val (a, b) = Pair(1, 2)
来源：http://hz.guannengcc.top/gtkzduvfkj.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtwthwssit.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gtzxqxpdlk.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtmodpmiow.html

for (i in 1..10) println(i)
来源：http://hz.wangdashe.top/gtbnyjlrkc.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtybbbeojt.html

interface Shape { fun area(): Double }
来源：http://hz.redwolf501.top/gtqjfyhfwp.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gtmzfyfybq.html

print("Hello")
来源：http://hz.zhixingplan.top/gtsljofryk.html

[T17] Swift：变量与常量
来源：http://hz.guannengcc.top/gtowzgbetf.html

var a = 1;  let b = 2
来源：http://hz.ivvv.top/gtcyhzzcin.html

[T18] Swift：字符串插值
来源：http://hz.hnqzz.top/gtvbybcdgv.html

"值: \(b)"
来源：http://hz.feifeiyinyue.top/gtpxptukqa.html

[T19] Swift：可选绑定
来源：http://hz.tianlin.xyz/gtbrbhwgoz.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtcbudihre.html

[T20] Swift：数组操作
来源：http://hz.havefunace.top/gtttsydzqz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtnmjqlzzg.html

[T21] Swift：遍历
来源：http://hz.mhx1999.top/gtwajcvzoj.html

for x in a { print(x) }
来源：http://hz.quarkkingdee.top/gtapazquuc.html

[T22] Swift：字典
来源：http://hz.yangfankeji.com/gtlmoaprfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gtuiwwilwk.html

[T23] Swift：函数
来源：http://hz.xingfuxueyuan.xyz/gtwrmvzeer.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jqgufenzy.top/gtzodruzmi.html

[T24] Swift：闭包
来源：http://hz.xinyue.icu/gtqdlrfqxq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.svipenyu.cn/gtnejfzsct.html

[T25] Swift：结构体
来源：http://hz.cqqwz.cn/gthkcqfquf.html

struct P { var x: Int }
来源：http://hz.shanyushiyangtech.top/gteurqgjex.html

[T26] Swift：类与重写
来源：http://hz.jqgufenzy.top/gtwvpsoksz.html

class A: Base { override func f() {} }
来源：http://hz.hywenlv.cn/gtybsfkcjm.html

[T27] Swift：错误处理
来源：http://hz.gzhubu.top/gtiawcddwz.html

do { try f() } catch { print(error) }
来源：http://hz.jlsjyb.cn/gticscosjn.html

[T28] Swift：枚举
来源：http://hz.xuanzx.com/gtplccxate.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtpyrjadlm.html

[T29] Swift：guard 提前返回
来源：http://hz.zhongyouzk.top/gtcmwsxeoy.html

guard let x = opt else { return }
来源：http://hz.jiagoushi.top/gtqbxmwqah.html

[T30] Swift：协议
来源：http://hz.hammf.cn/gtuomusotg.html

protocol Shape { func area() -> Double }
来源：http://hz.316326.xyz/gtbsctmpxo.html

[T31] Lua：Hello World
来源：http://hz.ehwqpu.com/gtwwojipeq.html

print("Hello")
来源：http://hz.gzhubu.top/gtkgwnnxbu.html

[T32] Lua：局部变量
来源：http://hz.guannengcc.top/gtjhdmlrhw.html

local a = 1
来源：http://hz.gotoacloud.top/gtkwrvymbp.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangtech.top/gtyyuokqyx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xziqi.cn/gtxbfqksol.html

[T34] Lua：遍历表
来源：http://hz.hywenlv.cn/gttakbsijx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhijiandao.cn/gtwkzxbtuh.html

[T35] Lua：字典表
来源：http://hz.cdnleiting.top/gtlzcuerle.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gthkmapiav.html

[T36] Lua：函数
来源：http://hz.havefunace.top/gtkfunwaiw.html

function add(a, b) return a + b end
来源：http://hz.guowangkeji.top/gtcdxigaiq.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtzhhrpoon.html

"a" .. "b"
来源：http://hz.yj202588.top/gttceyfjfa.html

[T38] Lua：条件
来源：http://hz.shanyushiyangtech.top/gttekhppsd.html

if x > 0 then print("正") end
来源：http://hz.yuanzhike.top/gtzejsrzwk.html

[T39] Lua：模式匹配
来源：http://hz.xinyue.icu/gtfqjimlif.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gttvyjrfwz.html

[T40] Lua：元表
来源：http://hz.shzxlz.cn/gtekwhlyhg.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtmdmzgdus.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtcbfagzrt.html

print "Hello\n";
来源：http://hz.gogol.net.cn/gthieizzyi.html

[T42] Perl：变量类型
来源：http://hz.tanke756.top/gtzevmugzq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.meibo888.top/gtnwgunqmh.html

[T43] Perl：字符串插值
来源：http://hz.aibaodan.cn/gtynovrgbd.html

"值: $a"
来源：http://hz.nanxinkj.top/gtfxlcbivn.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtptjwfmov.html

if ($a > 0) { print "正"; }
来源：http://hz.hnxiangtu.top/gtpcgxwdpc.html

[T45] Perl：数组遍历
来源：http://hz.birdmap.top/gtczxwfovz.html

for my $x (@arr) { print $x; }
来源：http://hz.hysaishi.cn/gtujxyzgte.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtblsgvyob.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigfzy.top/gtupzghgwz.html

[T47] Perl：正则捕获
来源：http://hz.havefunace.top/gtoefljasm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dashuyun.cn/gttcfjfadi.html

[T48] Perl：正则替换
来源：http://hz.vqdsnc.cn/gtrcmzyvkf.html

$s =~ s/old/new/g;
来源：http://hz.tanke756.top/gtpehutqfk.html

[T49] Perl：函数
来源：http://hz.hywenlv.cn/gtwbiduovs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.birdmap.top/gtzlufvlmh.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtnjiurvny.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aizwys.cn/gtcdhibhov.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hysaishi.cn/gtzndnbscl.html

[T51] Scala：Hello World
来源：http://hz.zhiwuduotai.top/gtyxitlkam.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtmtywsvtn.html

[T52] Scala：变量
来源：http://hz.hysaishi.cn/gtqrcjsqqe.html


<!-- 参考信息 -->