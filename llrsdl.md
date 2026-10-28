代发 wailian999

cmd > out.log 2>&1
来源：http://hz.nwbrower.top/gtenivmmpi.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtgrjqdakg.html

echo "log" >> out.log
来源：http://hz.aibaodan.cn/gtihcstpmi.html

[R41] 丢弃输出
来源：http://hz.ywan-chungtsiang.top/gtugwrhafw.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtptflnfvj.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtwgxqvsds.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtqulgiljv.html

[R43] 按名字查找文件
来源：http://hz.zdqjudy.top/gtmkmjwchi.html

find . -name "*.log" -type f
来源：http://hz.dianchejie.cn/gtmguhcwlh.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtdcwxqgna.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gthdeytfrk.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtkxkrbycq.html

find . -name "*.tmp" -delete
来源：http://hz.hnxiangtu.top/gtluoqzgqr.html

[R46] 递归替换文件内容
来源：http://hz.jyoumei.cn/gteaardfdj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xziqi.cn/gtfslrygtt.html

[R47] sed 单行替换
来源：http://hz.shzxlz.cn/gtwaawzifg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guowangkeji.top/gtjysjfwwt.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtwhwtryvb.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtfmrjvdkg.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gtbcjffsvr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.smart0.xyz/gtqvzdeict.html

[R50] awk 求和
来源：http://hz.cheryme.top/gtjnrvnqiq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tianlin.xyz/gtuzxnckti.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtarspblsq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangdashe.top/gtmonoaivx.html

[R52] 统计行数
来源：http://hz.sysykeji.top/gtbapadmgl.html

wc -l a.txt
来源：http://hz.yuxming.cn/gtfqqezhsc.html

[R53] 查看文件头与实时尾
来源：http://hz.yuxming.cn/gtfztcpwtx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtoihrymts.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtkmlmfrvn.html

diff a.txt b.txt
来源：http://hz.ydzc1.top/gtcanyxsbh.html

[R55] 压缩与解压
来源：http://hz.hnxiangtu.top/gtspqxxhml.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gtvtszfygs.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtskijkudp.html

scp file user@host:/path/
来源：http://hz.chenlongwang.top/gtcvrrxgft.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtenmkgruk.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtshsquicp.html

[R58] 下载文件
来源：http://hz.yvedp.cn/gtqzrvitzb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtjyyjdcso.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtawuimjfz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ppjwa.cn/gtiuhbtagl.html

[R60] 只看 HTTP 状态码
来源：http://hz.daria6918.cn/gtjgrieptg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.0kj1m.cn/gtshunpgyi.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtwtkftjgx.html

df -h;  du -sh *
来源：http://hz.ppjwa.cn/gtyldncams.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtohcxmabd.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gtejaytdgx.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gtqzjvqrzw.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gtcwtrquew.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtbrqkljdw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gogol.net.cn/gtuvlfbckp.html

[R65] 查看端口占用
来源：http://hz.ybcxt.top/gtfupmtjxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daria6918.cn/gtzqsxxtky.html

[R66] 定时任务
来源：http://hz.daria6918.cn/gtfruxserd.html

crontab -e;  crontab -l
来源：http://hz.dashuyun.cn/gtzaahocrf.html

[R67] 生成随机十六进制串
来源：http://hz.quarkkingdee.top/gtyjkhtbda.html

openssl rand -hex 16
来源：http://hz.meibo888.top/gtfegmscsw.html

[R68] 计算文件校验值
来源：http://hz.nanxuanxn.top/gtnjxtbbmb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hywenlv.cn/gtyylywnau.html

[R69] 生成随机密码
来源：http://hz.dianchejie.cn/gtnhzhonpm.html

head -c 16 /dev/urandom | base64
来源：http://hz.ppjwa.cn/gtiizpglpt.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtbhbtuhrj.html

date +%s;  date -d @1700000000
来源：http://hz.cheryme.top/gteaxxcsxi.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtsugivifi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gtttuowjnc.html

[R72] 等待端口就绪
来源：http://hz.daria6918.cn/gtpappdrlu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtmhqtnxml.html

[R73] 分割大日志
来源：http://hz.yanxiufei.cn/gtrhybnonx.html

split -l 1000 big.log part_
来源：http://hz.jlsjyb.cn/gtgrmlajtn.html

[R74] 批量重命名
来源：http://hz.guowangkeji.top/gtcbaaregv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shuidangran.top/gtqgzvrihh.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtjduxccwt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yonumen.top/gthusfozth.html

[R76] 使用临时文件
来源：http://hz.hnqzz.top/gtwtzufskl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtfiiqkmcl.html

[R77] 读取用户输入
来源：http://hz.zhaomingkeji.xyz/gtcidihhgq.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtiyarrzln.html

[R78] 交互式菜单
来源：http://hz.xinyue.icu/gtgymrruan.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtkqzmsbux.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtldlhngze.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xziqi.cn/gtrxloptiy.html

[R80] 查看脚本执行耗时
来源：http://hz.tianlin.xyz/gtzwmjmwdk.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtdbmrkwmq.html

================================================================================
来源：http://hz.chenzaomai.com/gtkeayevxi.html

S. C / C++ 专题
来源：http://hz.yj202588.top/gtawmqisvq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtsdumkqmg.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtcimfhaos.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtvviozoei.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gtptbrzumy.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gtagjlknjf.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gthffydzyt.html

[S03] C：读入整数
来源：http://hz.redwolf501.top/gtgzatjtsr.html

int x; scanf("%d", &x);
来源：http://hz.tianlin.xyz/gtvzigqjjq.html

[S04] C：字符串复制
来源：http://hz.ywan-chungtsiang.top/gtwkzuvxhv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.c1oappe.top/gtdlxxivvn.html

[S05] C：字符串长度
来源：http://hz.xuanzx.com/gtpnmiisxw.html

strlen(s)
来源：http://hz.ehwqpu.com/gtnvjmfmwe.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtrbbpjjpd.html

strcmp(a, b) == 0
来源：http://hz.cheryme.top/gtkdmsjcil.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtlmbygvtm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtmiiczedv.html

[S08] C：动态内存分配与释放
来源：http://hz.jlsjyb.cn/gtipwozhls.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtspojyemt.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtonvtseme.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shuidangran.top/gtycvtryiv.html

[S10] C：指针与解引用
来源：http://hz.ehwqpu.com/gtwckhywml.html

int *p = &a;  *p = 5;
来源：http://hz.pengpengdd.cyou/gthnktgimq.html

[S11] C：逐行读文件
来源：http://hz.pycfn.com/gtehnywtbx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtkjitwrxh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gttyxanzlp.html

fclose(f);
来源：http://hz.yueranfly.top/gtthvjeudu.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtzmzfqqaj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hfpthk.cn/gtukjyzeej.html

[S13] C：宏定义
来源：http://hz.cucudq.cn/gtscedpatc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.9152youxi.cn/gtzvryhhfm.html

[S14] C：枚举
来源：http://hz.snrcjt.cn/gtnibuebbr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cdnleiting.top/gtouqmrhbb.html

[S15] C：类型转换
来源：http://hz.hysaishi.cn/gtcuzrwkyn.html

(double) a / b
来源：http://hz.yangfankeji.com/gtuwozsick.html

[S16] C：位操作置位
来源：http://hz.shzxlz.cn/gtlstmrvkn.html

x |= (1 << 3);
来源：http://hz.316326.xyz/gtoemspcfm.html

[S17] C：安全拼接字符串
来源：http://hz.wangdashe.top/gtkzgvfdma.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.smart0.xyz/gtetzavdaq.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtpmzdplnf.html

int main(int argc, char **argv)
来源：http://hz.xuanzx.com/gtualunaye.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtwyyqioit.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gttknyrati.html

[S20] C：二分查找
来源：http://hz.nanxuanxn.top/gtdgizwlez.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtsybvwzbl.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtkkcuffkg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.birdmap.top/gthmlqjcbs.html

[S22] C：字符串转数字
来源：http://hz.xylfe.cn/gtimmpptlt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtkhwpcrvk.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtlrkddgxx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuetiantiany.cn/gtxyxdwpvd.html

[S24] C：获取本地时间
来源：http://hz.quarkkingdee.top/gtoyewdlgv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtvfnbuiuy.html

[S25] C：内存拷贝
来源：http://hz.yueranfly.top/gtuuhhfzpn.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtoehdubaf.html

[S26] C：内存清零
来源：http://hz.hnqzz.top/gtbguutsvs.html

memset(a, 0, sizeof a);
来源：http://hz.aizwys.cn/gtoeumhzsv.html

[S27] C：定义常量
来源：http://hz.ybcxt.top/gtjeqgzvwd.html

const double PI = 3.14159;
来源：http://hz.wangdashe.top/gtfmdrskal.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gtzeivfoay.html

static int counter = 0;
来源：http://hz.ivvv.top/gteeeczxqd.html

[S29] C：变参函数
来源：http://hz.yanxiufei.cn/gtghocoonz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.0kj1m.cn/gtyvlzwmbr.html

[S30] C：头文件保护
来源：http://hz.ybcxt.top/gtimbefiaf.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gtvokhldqz.html

#define X_H
来源：http://hz.cdnleiting.top/gtggvtkrci.html

#endif
来源：http://hz.snrcjt.cn/gtvawiysoh.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtyifdundj.html

#include <iostream>
来源：http://hz.vqdsnc.cn/gtyurcdyae.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jiagoushi.top/gthutpekxk.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gtwpbhlntx.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangkeji.top/gtmxdpgxlh.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtbrpvcqke.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guannengcc.top/gttavgypuu.html

[S34] C++：遍历 vector
来源：http://hz.hywenlv.cn/gtackqklgo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daria6918.cn/gtnxucvoia.html

[S35] C++：map
来源：http://hz.yongpay.top/gtrkbqjzpu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtjhjqncjv.html

[S36] C++：unordered_map
来源：http://hz.hfpthk.cn/gtnrgqivjj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtmrnnmjtj.html

[S37] C++：set
来源：http://hz.hammf.cn/gtdmwbusur.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenjidiqi.icu/gtsjcqzgyo.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtpxzlswyo.html

std::sort(v.begin(), v.end());
来源：http://hz.meibo888.top/gtqhwhyhgz.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtajlihjsi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yangfankeji.com/gtaqfhixbq.html

[S40] C++：查找元素
来源：http://hz.havefunace.top/gtbllnzngs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cheryme.top/gtzvufdcov.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtwlsketrn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ybcxt.top/gtnpdqymfs.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtfmmkolom.html

class B : public Base { public: void f() override {} };
来源：http://hz.pengpengdd.cyou/gttqqjmqib.html

[S43] C++：智能指针
来源：http://hz.ybcxt.top/gtitomuqlq.html

auto p = std::make_unique<int>(5);
来源：http://hz.hywenlv.cn/gtstqwzvfn.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtwsyvjdub.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtqqkvffht.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gtufabvcwx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pengpengdd.cyou/gtiywlhvqy.html

[S46] C++：函数模板
来源：http://hz.iojbl.cn/gtbirijhii.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenjidiqi.icu/gtcrcbrhyd.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtydjrmltn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258.top/gtcmsyjfvj.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtjubwbfqh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtvsqeayej.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtyrfsfldz.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gtquoltkur.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xziqi.cn/gtgmnvhkrn.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtkmnehdlt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dianchejie.cn/gtzjydvvbi.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtqfkqnccm.html

static_cast<double>(a) / b
来源：http://hz.redwolf501.top/gtkndxmtlq.html

[S52] C++：const 与 noexcept
来源：http://hz.jinyuanbaomall.cn/gtmmedpdid.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gtaqvrynrl.html

[S53] C++：移动语义
来源：http://hz.zhongyouzk.top/gtvhkggwnx.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxinkj.top/gtycdceuic.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtndpvvizn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gtjdakitac.html

[S55] C++：结构化绑定
来源：http://hz.daria6918.cn/gtlavsybux.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zycfv.cn/gteaulkqog.html

[S56] C++：optional
来源：http://hz.yj20258888.top/gtcpjueoqm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.meibo888.top/gtyatugdtv.html

[S57] C++：编译期常量
来源：http://hz.0kj1m.cn/gtqvhgkacx.html

constexpr int N = 10;
来源：http://hz.hongshengwenyu.top/gtjdzwqhxk.html

[S58] C++：命名空间
来源：http://hz.andypj.xyz/gtiiroiyjb.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhaomingkeji.xyz/gtmpywahrw.html

[S59] C++：静态断言
来源：http://hz.cheryme.top/gtozdocckz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigfzy.top/gtuyyrqvwa.html

[S60] C++：遍历并删除元素
来源：http://hz.zhiwuduotai.top/gtyvvxhiqu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gtcvwjqvty.html

================================================================================
来源：http://hz.jianghu66.top/gthmikasrw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtyqaemqug.html

================================================================================
来源：http://hz.ydzc1.top/gtpqwjhbmi.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtzbdwynbo.html

println("Hello")
来源：http://hz.andypj.xyz/gtwceklikx.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtaegdewkv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hammf.cn/gtscaeffaj.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtgyfshuwp.html

"值: $b"
来源：http://hz.smart0.xyz/gtoqgcesif.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gtquskutsv.html

val n: String? = null;  n?.length
来源：http://hz.vqdsnc.cn/gtnblgdybd.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtyrwkqrtk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gttvsgpald.html

[T06] Kotlin：集合映射
来源：http://hz.guannengcc.top/gtvtdpbnwd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtjorafjme.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gtdromjxoq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtaiwgipjj.html

[T08] Kotlin：数据类
来源：http://hz.ywan-chungtsiang.top/gtdubjmmdx.html

data class User(val name: String, val age: Int)
来源：http://hz.hfpthk.cn/gtpwuozpet.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtufktekha.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtexdgvkpl.html

[T10] Kotlin：默认参数
来源：http://hz.shzxlz.cn/gtneqlqsqv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daria6918.cn/gtvnrzlxsz.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtjnqjxzrh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydzc1.top/gtkwhunfjq.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtrfqwwrej.html

val (a, b) = Pair(1, 2)
来源：http://hz.hfpthk.cn/gtpahntzcy.html

[T13] Kotlin：只读 Map
来源：http://hz.tian-w.cn/gtobyeeezs.html

val m = mapOf("a" to 1)
来源：http://hz.hfpthk.cn/gtpassxpxo.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtniuaechc.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtkvjoypst.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gtgqutyaui.html

interface Shape { fun area(): Double }
来源：http://hz.hywenlv.cn/gtkkoipsnr.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gttxelihic.html

print("Hello")
来源：http://hz.jinqigufen.top/gteeeouxxk.html

[T17] Swift：变量与常量
来源：http://hz.guannengcc.top/gtjhxltanr.html

var a = 1;  let b = 2
来源：http://hz.gogol.net.cn/gtiilzbkso.html

[T18] Swift：字符串插值
来源：http://hz.meibo888.top/gtmxbnkvtx.html

"值: \(b)"
来源：http://hz.nanxinkj.top/gtshmltgsc.html

[T19] Swift：可选绑定
来源：http://hz.jyoumei.cn/gtjammzsoe.html

if let n = opt { print(n) }
来源：http://hz.svipenyu.cn/gtxkxnwqiy.html

[T20] Swift：数组操作
来源：http://hz.wangdashe.top/gtowswyqst.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj20258888.top/gtuprvjadg.html

[T21] Swift：遍历
来源：http://hz.hfpthk.cn/gtfilumhws.html

for x in a { print(x) }
来源：http://hz.nwbrower.top/gtnhemhktz.html

[T22] Swift：字典
来源：http://hz.hywenlv.cn/gtadeyyqmd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydjk.org.cn/gtodrjwcki.html

[T23] Swift：函数
来源：http://hz.zhengqikj.top/gtwceuzpqe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtunvqgrcw.html

[T24] Swift：闭包
来源：http://hz.havefunace.top/gtlvyqtsxw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtvrdzjjvz.html

[T25] Swift：结构体
来源：http://hz.andypj.xyz/gtgzngnhax.html

struct P { var x: Int }
来源：http://hz.zdqjudy.top/gtsnnfqtpv.html

[T26] Swift：类与重写
来源：http://hz.cheryme.top/gthvqtlrgv.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtzstjmmqi.html

[T27] Swift：错误处理
来源：http://hz.cucudq.cn/gtqkiwyxed.html

do { try f() } catch { print(error) }
来源：http://hz.feifeiyinyue.top/gtpxnbmqzf.html

[T28] Swift：枚举
来源：http://hz.daxiang520.top/gtvobaakuj.html

enum Color { case red, green }
来源：http://hz.mhx1999.top/gtayvqzuif.html

[T29] Swift：guard 提前返回
来源：http://hz.hfpthk.cn/gtmsgbqxpc.html

guard let x = opt else { return }
来源：http://hz.chenlongwang.top/gtndljbndz.html

[T30] Swift：协议
来源：http://hz.ybcxt.top/gtfnnkhrjx.html

protocol Shape { func area() -> Double }
来源：http://hz.shzxlz.cn/gtdzqzkxnj.html

[T31] Lua：Hello World
来源：http://hz.dianchejie.cn/gtqwvlezuh.html

print("Hello")
来源：http://hz.yonumen.top/gtzjqgxmfn.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangtech.top/gtqvxeotnz.html

local a = 1
来源：http://hz.havefunace.top/gtjqmxadrl.html

[T33] Lua：表（数组）
来源：http://hz.jqgfzy.top/gtmsoetbis.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtpmkahnrp.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtqxngrkpx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinghuilouyu.cn/gtgptpsqdd.html

[T35] Lua：字典表
来源：http://hz.nwbrower.top/gtiepexdkc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cqqwz.cn/gtwphoxhlq.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtjtelnxsc.html

function add(a, b) return a + b end
来源：http://hz.jqgfzy.top/gtyylvzypf.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtjcwbxbnf.html

"a" .. "b"
来源：http://hz.gaohongyu789.top/gtksvpulzr.html

[T38] Lua：条件
来源：http://hz.yuxming.cn/gtleihisfs.html

if x > 0 then print("正") end
来源：http://hz.sufxvd.cn/gtxikvreys.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtycrgfoqa.html

string.find(s, "%d+")
来源：http://hz.ybcxt.top/gtrteupdro.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtrvmjkeqp.html

setmetatable({}, { __index = base })
来源：http://hz.fengsongda.top/gtcgzdcgxh.html

[T41] Perl：Hello World
来源：http://hz.xuanzx.com/gtjqwiuvkj.html

print "Hello\n";
来源：http://hz.nanxuanxn.top/gtcdzjfxmq.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gttmxzntmv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xingfuxueyuan.xyz/gtycukplad.html


<!-- 参考信息 -->