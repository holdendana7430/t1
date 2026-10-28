代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cdnleiting.top/gtoengygzl.html

[R48] awk 取指定列
来源：http://hz.9152youxi.cn/gtplmmiuvx.html

awk '{print $1, $3}' a.txt
来源：http://hz.yongpay.top/gtbexhobnr.html

[R49] awk 带条件
来源：http://hz.jinghuilouyu.cn/gttrgjecdr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtkwtsfekc.html

[R50] awk 求和
来源：http://hz.haohaochexian.top/gtjrnrmvuh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.smart0.xyz/gtnwsbcgzv.html

[R51] 排序去重取前几
来源：http://hz.hfpthk.cn/gtmrrjcxqy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtndivgmdb.html

[R52] 统计行数
来源：http://hz.yongpay.top/gttoxhovvv.html

wc -l a.txt
来源：http://hz.shuidangran.top/gtxgfdvuhx.html

[R53] 查看文件头与实时尾
来源：http://hz.shanyushiyangkeji.top/gtkwetgifu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtiaxvrdzl.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtoxnpiorx.html

diff a.txt b.txt
来源：http://hz.feifeiyinyue.top/gtczushqev.html

[R55] 压缩与解压
来源：http://hz.guowangkeji.top/gtnngkcmbm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhoulong.xyz/gtlsrwzmmw.html

[R56] 远程拷贝
来源：http://hz.zycfv.cn/gtavvlvdch.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gtxwugzmwv.html

[R57] 远程执行命令
来源：http://hz.dianchejie.cn/gtzxfzvzsw.html

ssh user@host 'uptime'
来源：http://hz.hnxiangtu.top/gtfmzmigoz.html

[R58] 下载文件
来源：http://hz.pycfn.com/gtmrfutjgg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinghuilouyu.cn/gttjzbnkul.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gtweynjtkk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenjidiqi.icu/gtochqerjx.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtrtcesssb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.c1oappe.top/gtcqhjyhrp.html

[R61] 磁盘占用
来源：http://hz.xuetiantiany.cn/gtcshqgjbu.html

df -h;  du -sh *
来源：http://hz.tianlin.xyz/gtgvzgapah.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtwfpomjem.html

du -ah . | sort -rh | head -10
来源：http://hz.fzhhl.top/gtxdigkcmh.html

[R63] 内存与进程
来源：http://hz.xuetiantiany.cn/gtiirrppar.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gtrnbrceim.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtrvrtxlqy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtcqxxaukv.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtnqntsfbb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtbcabkrtu.html

[R66] 定时任务
来源：http://hz.daria6918.cn/gtbrgmhsvp.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtsrjxuily.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gthjqrztjk.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtxfaefvox.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtvffumpla.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jlsjyb.cn/gtrzzndstr.html

[R69] 生成随机密码
来源：http://hz.dianchejie.cn/gtrlwltpqy.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydjk.org.cn/gtqpsysiir.html

[R70] 时间戳与互转
来源：http://hz.quarkkingdee.top/gtcuzxkcoa.html

date +%s;  date -d @1700000000
来源：http://hz.jianghu66.top/gtpktppoip.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gtonnaoxgt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuanzx.com/gtugpimryw.html

[R72] 等待端口就绪
来源：http://hz.pengpengdd.cyou/gtgtxwkxgq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zycfv.cn/gtnuccwjcw.html

[R73] 分割大日志
来源：http://hz.sweek.top/gtguupizdd.html

split -l 1000 big.log part_
来源：http://hz.xingfuxueyuan.xyz/gtpisxpdpg.html

[R74] 批量重命名
来源：http://hz.meibo888.top/gtwxesgsis.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jiagoushi.top/gtmghrsjaj.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gtqapgknhn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xziqi.cn/gtntbodiqy.html

[R76] 使用临时文件
来源：http://hz.yueranfly.top/gtweckpqqq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtuhzxgcko.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtbzqbfyld.html

read -rp "请输入: " ans
来源：http://hz.yuxming.cn/gtnrnnzogj.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gtbtglexyq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guannengcc.top/gtrcwnznwo.html

[R79] 解析命令行选项
来源：http://hz.tanke756.top/gtvgozbizl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtnyhccvwp.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258888.top/gtwavbskbf.html

time ./run.sh
来源：http://hz.pengpengdd.cyou/gthoxtdpkj.html

================================================================================
来源：http://hz.yuanzhike.top/gtepjiebfz.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtnohzyjvy.html

================================================================================
来源：http://hz.snrcjt.cn/gtntlprvri.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtvmamhjux.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gtyvvljwzi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hammf.cn/gtspcbgzbt.html

[S02] C：变量与格式化输出
来源：http://hz.cheryme.top/gtbweqommd.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtocmdzjtd.html

[S03] C：读入整数
来源：http://hz.9152youxi.cn/gtbhxyquuw.html

int x; scanf("%d", &x);
来源：http://hz.xziqi.cn/gtcoqhpjes.html

[S04] C：字符串复制
来源：http://hz.kuanghao11.cn/gtxtbaltax.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.316326.xyz/gtrkwwbnfo.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtcvlbihge.html

strlen(s)
来源：http://hz.iojbl.cn/gtjorbfrlr.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtubmrrcnm.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gteshddvja.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gtenzvsqut.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtwemexmne.html

[S08] C：动态内存分配与释放
来源：http://hz.zhijiandao.cn/gtdjxlezko.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtkbpayezw.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtsmipbzwu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangtech.top/gtbnkluvpd.html

[S10] C：指针与解引用
来源：http://hz.sweek.top/gtlesgeack.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtftsrnfbe.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gticlzvnoi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guannengcc.top/gtinizduri.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtbhrukzqy.html

fclose(f);
来源：http://hz.sweek.top/gtpyminhgn.html

[S12] C：写文件
来源：http://hz.wangdashe.top/gtgzaxpltv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hywenlv.cn/gtohafsczs.html

[S13] C：宏定义
来源：http://hz.sxryk.cn/gtlmdlgzgg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhoulong.xyz/gtfupshdnx.html

[S14] C：枚举
来源：http://hz.shanyushiyangkeji.top/gtttbzlknz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gtzdiqmnzp.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gtxfzhbawp.html

(double) a / b
来源：http://hz.jiagoushi.top/gtjfjcatrf.html

[S16] C：位操作置位
来源：http://hz.aibaodan.cn/gtbjdtbpmi.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtvcqqifto.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtxaahqarn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtbqiqcwqe.html

[S18] C：命令行参数
来源：http://hz.xinyue.icu/gtmzzgloif.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtklxcxoqd.html

[S19] C：快速排序
来源：http://hz.svipenyu.cn/gteajrkush.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtfpibeasq.html

[S20] C：二分查找
来源：http://hz.nwbrower.top/gtwsigcsrp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtehaxagmq.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtzulzsdcl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.iojbl.cn/gtgxtdcryu.html

[S22] C：字符串转数字
来源：http://hz.birdmap.top/gtedzdsrfi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xingfuxueyuan.xyz/gtxvwwqokk.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gtqfhekvca.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gtsfywbbgr.html

[S24] C：获取本地时间
来源：http://hz.jinghuilouyu.cn/gtixurmpfk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtbxoxamov.html

[S25] C：内存拷贝
来源：http://hz.smart0.xyz/gtjqkazyap.html

memcpy(dst, src, n);
来源：http://hz.zhaomingkeji.xyz/gtftouzfzy.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtbmqycuna.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258.top/gtgvwfbplw.html

[S27] C：定义常量
来源：http://hz.guannengcc.top/gtdmizbxyc.html

const double PI = 3.14159;
来源：http://hz.yongpay.top/gtedgzvrwd.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtobxvkoqn.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtfjjwpnof.html

[S29] C：变参函数
来源：http://hz.cashguo.top/gtxqqihwjk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nwbrower.top/gtoqnsvjmp.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtpxvjfccv.html

#ifndef X_H
来源：http://hz.chenzaomai.com/gterlvhxcq.html

#define X_H
来源：http://hz.shanyushiyangtech.top/gtezzgkeke.html

#endif
来源：http://hz.snrcjt.cn/gtfpqluqht.html

[S31] C++：Hello World
来源：http://hz.redwolf501.top/gtsawggtjf.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtromnxubg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtbtpoldyq.html

[S32] C++：字符串
来源：http://hz.sweek.top/gtxdctxzsf.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxinkj.top/gtesdlvhsw.html

[S33] C++：vector 增删
来源：http://hz.zhoulong.xyz/gtxlxvelnk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtjorszjvl.html

[S34] C++：遍历 vector
来源：http://hz.zhiwuduotai.top/gtsmygubco.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tianlin.xyz/gtfxprpaqp.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtrqiscmno.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtabnulbpq.html

[S36] C++：unordered_map
来源：http://hz.tanke756.top/gtlphlkyms.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtehhcdkqu.html

[S37] C++：set
来源：http://hz.zhaomingkeji.xyz/gtvllnhwcf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtyzcknyji.html

[S38] C++：排序
来源：http://hz.iojbl.cn/gtkoninkmc.html

std::sort(v.begin(), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtcytdrkna.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtgtazrjfg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtrupvmzfc.html

[S40] C++：查找元素
来源：http://hz.mhx1999.top/gtpmntbhbi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhongyouzk.top/gtxlekgmnz.html

[S41] C++：类与构造函数
来源：http://hz.sxryk.cn/gtxydmwwpj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.birdmap.top/gtvnvaaecg.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258.top/gtsscwnnkn.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtqzsxtudi.html

[S43] C++：智能指针
来源：http://hz.wangdashe.top/gtnbarwtmk.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgufenzy.top/gtwaapfoof.html

[S44] C++：引用传参
来源：http://hz.haohaochexian.top/gtjbkucskn.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtddaqoizu.html

[S45] C++：lambda
来源：http://hz.nanxinkj.top/gtgzbfrlqg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhijiandao.cn/gtelqnhdwr.html

[S46] C++：函数模板
来源：http://hz.ybcxt.top/gtsomkydwo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtkpqvvclt.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258888.top/gtjpxqpcqb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtlyqxqzwk.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gttitgxtbr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gthxeoqhqn.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtgvvenmzy.html

[S49] C++：写文件
来源：http://hz.yanxiufei.cn/gtgriwqyzy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pengpengdd.cyou/gtunbothqu.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtwvnsdcbm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ybcxt.top/gtswsapsmw.html

[S51] C++：显式类型转换
来源：http://hz.jinqigfzy.top/gtfanxahhk.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtgtqgoexd.html

[S52] C++：const 与 noexcept
来源：http://hz.havefunace.top/gtlsdksnlb.html

int size() const noexcept { return n_; }
来源：http://hz.chenzaomai.com/gthzxtjuoi.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtjijkpnzk.html

std::vector<int> w = std::move(v);
来源：http://hz.guowangkeji.top/gtpnammcnr.html

[S54] C++：异常处理
来源：http://hz.shuidangran.top/gtkzrtffpt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gttsnufuhu.html

[S55] C++：结构化绑定
来源：http://hz.iojbl.cn/gtlaploqvv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.iojbl.cn/gtimkocjxj.html

[S56] C++：optional
来源：http://hz.jqgfzy.top/gtphghblns.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dianchejie.cn/gtoqsrmdgy.html

[S57] C++：编译期常量
来源：http://hz.ydjk.org.cn/gtivcotquz.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gtoaunyohc.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtujhbtzzs.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtgnasuhoi.html

[S59] C++：静态断言
来源：http://hz.ydjk.org.cn/gtynwmgckp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.9152youxi.cn/gtvdbntutf.html

[S60] C++：遍历并删除元素
来源：http://hz.ybcxt.top/gtknccuuun.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hongshengwenyu.top/gtpqwpdivy.html

================================================================================
来源：http://hz.daxiang520.top/gtmpkpperx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtbmadygcg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvlzdynop.html

[T01] Kotlin：Hello World
来源：http://hz.pengpengdd.cyou/gtnychlodb.html

println("Hello")
来源：http://hz.cucudq.cn/gtswxyjhss.html

[T02] Kotlin：变量
来源：http://hz.zhaomingkeji.xyz/gtzckqkyse.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gthyyenntc.html

[T03] Kotlin：字符串模板
来源：http://hz.cucudq.cn/gtjifqsgix.html

"值: $b"
来源：http://hz.ydjk.org.cn/gttwdgruiz.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtrbbdylqq.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtsacvkzio.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgufenzy.top/gtxwigstww.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.redwolf501.top/gtpxqjviem.html

[T06] Kotlin：集合映射
来源：http://hz.gotoacloud.top/gtnfbwqcdw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cdnleiting.top/gtuproxcns.html

[T07] Kotlin：集合过滤
来源：http://hz.hammf.cn/gtwkoexyhh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sysykeji.top/gtdwkghmtr.html

[T08] Kotlin：数据类
来源：http://hz.zhongyouzk.top/gteuobufyl.html

data class User(val name: String, val age: Int)
来源：http://hz.chenjidiqi.icu/gtgdgcqbnd.html

[T09] Kotlin：扩展函数
来源：http://hz.xziqi.cn/gtzbrbbewh.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gthjtwedsi.html

[T10] Kotlin：默认参数
来源：http://hz.chenjidiqi.icu/gtzfzfbpsa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yonumen.top/gtjinqprsy.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gtxpfwdprt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hywenlv.cn/gtpfcwrlvd.html

[T12] Kotlin：解构声明
来源：http://hz.hnqzz.top/gtbfpnkoff.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxinkj.top/gtxsumsfrr.html

[T13] Kotlin：只读 Map
来源：http://hz.zhixingplan.top/gtbbrzfsvf.html

val m = mapOf("a" to 1)
来源：http://hz.hammf.cn/gtmlxsrcfv.html

[T14] Kotlin：循环
来源：http://hz.hongshengwenyu.top/gtidmjeqvr.html

for (i in 1..10) println(i)
来源：http://hz.xuetiantiany.cn/gtwpwpbloc.html

[T15] Kotlin：接口
来源：http://hz.yvedp.cn/gtgngypkkv.html

interface Shape { fun area(): Double }
来源：http://hz.cheryme.top/gtldtpenia.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gtmbfddkcx.html

print("Hello")
来源：http://hz.yueranfly.top/gtmtqndyjn.html

[T17] Swift：变量与常量
来源：http://hz.c1oappe.top/gtxsqyucrf.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtqwtrcelg.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtkrupgqif.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gtyfrrnlwz.html

[T19] Swift：可选绑定
来源：http://hz.nanxinkj.top/gtxtduubzu.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtoqqqrvyp.html

[T20] Swift：数组操作
来源：http://hz.ydzc1.top/gtwirvdsnj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.mhx1999.top/gtxutnaubl.html

[T21] Swift：遍历
来源：http://hz.fzhhl.top/gtheyporrp.html

for x in a { print(x) }
来源：http://hz.vqdsnc.cn/gtkgnopzhf.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gtznhrhqwy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daria6918.cn/gtxsdbaofg.html

[T23] Swift：函数
来源：http://hz.redwolf501.top/gtzkpwetgd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtimxrsxeo.html

[T24] Swift：闭包
来源：http://hz.daria6918.cn/gtfmrzvezo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xinyue.icu/gtocfmqflz.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtphwqvdlj.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gtgyacqnyt.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtqweeaizw.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangtech.top/gtqwiwigrj.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtykfbcluj.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtjnuuhhon.html

[T28] Swift：枚举
来源：http://hz.mhx1999.top/gtxhkrzafw.html

enum Color { case red, green }
来源：http://hz.hongshengwenyu.top/gtnezpmoeh.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtbsosugvk.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gtcgrdhoik.html

[T30] Swift：协议
来源：http://hz.chenzaomai.com/gtlvcjkxvp.html

protocol Shape { func area() -> Double }
来源：http://hz.aibaodan.cn/gtcfdqkihv.html

[T31] Lua：Hello World
来源：http://hz.tian-w.cn/gtmprzkyqg.html

print("Hello")
来源：http://hz.wangdashe.top/gtepuvwfhx.html

[T32] Lua：局部变量
来源：http://hz.aibaodan.cn/gtnudrjqdj.html

local a = 1
来源：http://hz.xinyue.icu/gtlifsksoe.html

[T33] Lua：表（数组）
来源：http://hz.guannengcc.top/gtvcmvfdpk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zdqjudy.top/gtdgwvweyg.html

[T34] Lua：遍历表
来源：http://hz.316326.xyz/gtoqbthrtn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuxming.cn/gtkrdfdatq.html

[T35] Lua：字典表
来源：http://hz.meibo888.top/gtybkhivze.html

local d = { a = 1 };  d.b = 2
来源：http://hz.quarkkingdee.top/gtwcpelqjl.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gtncissmqo.html

function add(a, b) return a + b end
来源：http://hz.ppjwa.cn/gtenlzzrnf.html

[T37] Lua：字符串拼接
来源：http://hz.c1oappe.top/gtmcykozid.html

"a" .. "b"
来源：http://hz.shuidangran.top/gtpqevjeas.html

[T38] Lua：条件
来源：http://hz.gogol.net.cn/gtleznnsqh.html

if x > 0 then print("正") end
来源：http://hz.hongshengwenyu.top/gtmmlczauj.html

[T39] Lua：模式匹配
来源：http://hz.chenzaomai.com/gteytcskww.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtywwmywxf.html

[T40] Lua：元表
来源：http://hz.cucudq.cn/gtrrfuyoni.html

setmetatable({}, { __index = base })
来源：http://hz.ehwqpu.com/gtoetnmsbh.html

[T41] Perl：Hello World
来源：http://hz.jinqigfzy.top/gtbzhgdqkw.html

print "Hello\n";
来源：http://hz.ehwqpu.com/gtlecbujau.html

[T42] Perl：变量类型
来源：http://hz.zhixingplan.top/gtswkxadms.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sysykeji.top/gtdzppjpsw.html

[T43] Perl：字符串插值
来源：http://hz.zhijiandao.cn/gtbrydbfef.html

"值: $a"
来源：http://hz.daria6918.cn/gtuspriibu.html

[T44] Perl：条件
来源：http://hz.xingfuxueyuan.xyz/gtzjaheedv.html

if ($a > 0) { print "正"; }
来源：http://hz.xylfe.cn/gtaseofdvn.html

[T45] Perl：数组遍历
来源：http://hz.fengsongda.top/gtpjxzlpxn.html

for my $x (@arr) { print $x; }
来源：http://hz.hysaishi.cn/gtoafnaxls.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtqgmzvppv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuanzx.com/gtblzuwfhc.html

[T47] Perl：正则捕获
来源：http://hz.zhengqikj.top/gtxywtqknk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhaomingkeji.xyz/gtovcvgyaq.html

[T48] Perl：正则替换
来源：http://hz.yueranfly.top/gtyweqkmov.html

$s =~ s/old/new/g;
来源：http://hz.fzhhl.top/gtcorxittq.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtrqctkicn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gaohongyu789.top/gtkpphbzsh.html

[T50] Perl：逐行读文件
来源：http://hz.shangyingyoupin.top/gtwhvdgudl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ywan-chungtsiang.top/gtrjbgljin.html


<!-- 参考信息 -->