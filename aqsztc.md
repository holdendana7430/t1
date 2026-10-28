代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xylfe.cn/gtbjmbshfm.html

[R34] 退出时清理
来源：http://hz.xuanzx.com/gtyuwuyyqo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxinkj.top/gtrwqjhiav.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtsmoiyaks.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtoicwnbkv.html

[R36] 并发执行多个任务
来源：http://hz.hnxiangtu.top/gttvkyyxfe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guowangkeji.top/gtfkkjrzqt.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtzszpbwku.html

files=$(ls -1)
来源：http://hz.vqdsnc.cn/gtzqkbxmxw.html

[R38] 管道串联
来源：http://hz.0kj1m.cn/gtcljtodgy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shuidangran.top/gtdsvwtzem.html

[R39] 重定向标准输出与错误
来源：http://hz.zhixingplan.top/gtijdbtdcw.html

cmd > out.log 2>&1
来源：http://hz.yuxming.cn/gtvewitwxd.html

[R40] 追加写日志
来源：http://hz.shanyushiyangkeji.top/gtwdonyyqn.html

echo "log" >> out.log
来源：http://hz.havefunace.top/gtwyuywzqi.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtutgyadnn.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gtvmfhqotg.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtnhzgqztu.html

wc -l < a.txt
来源：http://hz.xuetiantiany.cn/gteinehujr.html

[R43] 按名字查找文件
来源：http://hz.yj20258888.top/gtjaxlzsed.html

find . -name "*.log" -type f
来源：http://hz.hysaishi.cn/gttinukvxn.html

[R44] 按修改时间查找
来源：http://hz.yj20258888.top/gtdcponlpp.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gtemhcdhdy.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtumpabsns.html

find . -name "*.tmp" -delete
来源：http://hz.hnqzz.top/gtaooxobng.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtcjujgjda.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aibaodan.cn/gtixhcenje.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtfetaitey.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gtvtylwwme.html

[R48] awk 取指定列
来源：http://hz.haohaochexian.top/gtgqrywhcx.html

awk '{print $1, $3}' a.txt
来源：http://hz.c1oappe.top/gtzmbdydwg.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtwvxpoowo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtfrdkftip.html

[R50] awk 求和
来源：http://hz.jyoumei.cn/gtcvcyvkae.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gtfiuwlpgd.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtlioevstq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pycfn.com/gtsuzkdyft.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtplxcmiih.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtccskmzjk.html

[R53] 查看文件头与实时尾
来源：http://hz.shuidangran.top/gtfrxfgbuh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.svipenyu.cn/gtcaopstzn.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtpyuwahae.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtstzlvzvp.html

[R55] 压缩与解压
来源：http://hz.yanxiufei.cn/gtobapojih.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtzfggabvv.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtocinopxn.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtprjfhvbq.html

[R57] 远程执行命令
来源：http://hz.nanxuanxn.top/gtafvvvvfm.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtzaewxwbn.html

[R58] 下载文件
来源：http://hz.cqqwz.cn/gtnkpoozyc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tian-w.cn/gtytmnyanq.html

[R59] 发 POST JSON
来源：http://hz.jinqigfzy.top/gtrruynxyl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtrpqprovk.html

[R60] 只看 HTTP 状态码
来源：http://hz.gogol.net.cn/gtwzjaczvg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.vqdsnc.cn/gtvzhexirf.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtvartkhlt.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gtoxjrawxy.html

[R62] 找最占空间的文件
来源：http://hz.yj202588.top/gttpgwxvcq.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtyqxsowxj.html

[R63] 内存与进程
来源：http://hz.zhongyouzk.top/gtnhcsxogk.html

free -h;  ps aux | grep nginx
来源：http://hz.jyoumei.cn/gtlrwkyyas.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gtscqvsicd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtdorehvhd.html

[R65] 查看端口占用
来源：http://hz.yongpay.top/gtwluakzss.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtdnsyyevh.html

[R66] 定时任务
来源：http://hz.tianlin.xyz/gtpadpslel.html

crontab -e;  crontab -l
来源：http://hz.tianlin.xyz/gtxhplmwjl.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gtskxfdtfo.html

openssl rand -hex 16
来源：http://hz.yongpay.top/gtljifdetf.html

[R68] 计算文件校验值
来源：http://hz.havefunace.top/gtpvxytioi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtkszwuofs.html

[R69] 生成随机密码
来源：http://hz.aibaodan.cn/gtcwcinmte.html

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gtsjmybfik.html

[R70] 时间戳与互转
来源：http://hz.gaohongyu789.top/gtvpmkfedf.html

date +%s;  date -d @1700000000
来源：http://hz.dianchejie.cn/gtwyjpbere.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtugemroyn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.bjfxy.top/gtbwdzczck.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtbmdngjrx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gogol.net.cn/gtljkudino.html

[R73] 分割大日志
来源：http://hz.tian-w.cn/gtnjlfebfe.html

split -l 1000 big.log part_
来源：http://hz.meibo888.top/gttgujevcy.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtmghqzxwm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cheryme.top/gtcfsomwcr.html

[R75] 导出环境变量
来源：http://hz.sweek.top/gtqpxjxebq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yongpay.top/gtgkumubed.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gticfxfqpp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtyxdzlivr.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gtqlkpfllf.html

read -rp "请输入: " ans
来源：http://hz.ywan-chungtsiang.top/gtwfoojdqj.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtygusimfs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gtagbumlwe.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtwkieebtf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yonumen.top/gtvqsghuxl.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtwrzmfxep.html

time ./run.sh
来源：http://hz.gotoacloud.top/gtgjewlpme.html

================================================================================
来源：http://hz.xylfe.cn/gtcwbyhrlj.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtpgowymvt.html

================================================================================
来源：http://hz.smart0.xyz/gtwkdkadmu.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtqaprljhm.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtqleshwxl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtakuitrcp.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtujzsytul.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gtjktmzoke.html

[S03] C：读入整数
来源：http://hz.cdnleiting.top/gtmyyotrfj.html

int x; scanf("%d", &x);
来源：http://hz.zhengqikj.top/gtjszzoazc.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtnffjiipr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhijiandao.cn/gthjuukzxs.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtiqmfmtgz.html

strlen(s)
来源：http://hz.sysykeji.top/gtnrqbqhpd.html

[S06] C：字符串比较
来源：http://hz.ydzc1.top/gthtsntcyi.html

strcmp(a, b) == 0
来源：http://hz.guowangkeji.top/gtpuinugdf.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gtfkwujctu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxuanxn.top/gtgbxddarb.html

[S08] C：动态内存分配与释放
来源：http://hz.hysaishi.cn/gtjmvvgpcv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtufechpsp.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtlkfudlxi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtjlshgjyo.html

[S10] C：指针与解引用
来源：http://hz.mhx1999.top/gtalmqvtfw.html

int *p = &a;  *p = 5;
来源：http://hz.chenzaomai.com/gtbfelevjw.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gthvphtmfr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtvprqrpxq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fengsongda.top/gtyswuhgyq.html

fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtsfylejpy.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtwvdkqreq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtwyaesqnl.html

[S13] C：宏定义
来源：http://hz.c1oappe.top/gtrdksipgh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.birdmap.top/gturphxukt.html

[S14] C：枚举
来源：http://hz.chenzaomai.com/gtrqzgilhz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tian-w.cn/gtbghvghzt.html

[S15] C：类型转换
来源：http://hz.havefunace.top/gtkdafvpsr.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtyalmbjdl.html

[S16] C：位操作置位
来源：http://hz.gotoacloud.top/gtkizlozcl.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtqtxzrpcv.html

[S17] C：安全拼接字符串
来源：http://hz.mhx1999.top/gtjjifjhej.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnxiangtu.top/gtwbigunsz.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtdjxjoata.html

int main(int argc, char **argv)
来源：http://hz.hywenlv.cn/gtwbvunnix.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gthduqdurh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtvuybqrdi.html

[S20] C：二分查找
来源：http://hz.meibo888.top/gtnodtofxd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtjsfwexod.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gttycogmtf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tian-w.cn/gttwronkqw.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtrblwyldi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zdqjudy.top/gtlykmrqme.html

[S23] C：随机数
来源：http://hz.andypj.xyz/gtsbfragzu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gtjxuzpdpr.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtzzlzvapx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gzhubu.top/gtjnzexgbj.html

[S25] C：内存拷贝
来源：http://hz.redwolf501.top/gtytdqfvmf.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtmbsyxddv.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gticxjvskt.html

memset(a, 0, sizeof a);
来源：http://hz.jianghu66.top/gtsvvkqfrs.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtymkzgyyp.html

const double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtbtmvkhwl.html

[S28] C：静态变量
来源：http://hz.andypj.xyz/gtgiypsmim.html

static int counter = 0;
来源：http://hz.zhaomingkeji.xyz/gtmvoohnzl.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtfbmvnxfc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtyhjnihyi.html

[S30] C：头文件保护
来源：http://hz.0kj1m.cn/gtncopqzcu.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtrcslzvjk.html

#define X_H
来源：http://hz.0kj1m.cn/gtksigjubz.html

#endif
来源：http://hz.cdnleiting.top/gtzlfwgrnw.html

[S31] C++：Hello World
来源：http://hz.yuanzhike.top/gtoltuista.html

#include <iostream>
来源：http://hz.jqgfzy.top/gtfttkqqlb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gttxopqmat.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gttdfkebyo.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtxrzssocp.html

[S33] C++：vector 增删
来源：http://hz.yueranfly.top/gtdotjkwok.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ppjwa.cn/gtnjhwpqso.html

[S34] C++：遍历 vector
来源：http://hz.sxryk.cn/gtkslpvqkh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtnzxmwcap.html

[S35] C++：map
来源：http://hz.kuanghao11.cn/gtpfewaswg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gttfznewiv.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtfvjrthnw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtfrnpbryv.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtqvoypdqu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hammf.cn/gtnclkucfn.html

[S38] C++：排序
来源：http://hz.jinqigufen.top/gtmmnrfpzj.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtdrqlkzoe.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtxhnqaalh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtobqygceh.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gthaerehpe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtcyyofsgd.html

[S41] C++：类与构造函数
来源：http://hz.52xcode.cn/gtqpndsgxa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj202588.top/gttcbsxozj.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtuueyvahw.html

class B : public Base { public: void f() override {} };
来源：http://hz.yongpay.top/gtymrugbdd.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gtqqouqyex.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtpxhdxcmv.html

[S44] C++：引用传参
来源：http://hz.0kj1m.cn/gtyoyzzymy.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gthohufend.html

[S45] C++：lambda
来源：http://hz.sysykeji.top/gtaenwwmft.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtsikfobaf.html

[S46] C++：函数模板
来源：http://hz.hongshengwenyu.top/gtlqsrilty.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtoeilbkmn.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtwmbxwkpd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxinkj.top/gtxabgeshi.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gtezqofhsu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtkxdwraiy.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigfzy.top/gthesabfrn.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtdosiwyuy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.mhx1999.top/gtsymvksqa.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gtpavpklon.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtuvhojwbh.html

[S51] C++：显式类型转换
来源：http://hz.hfpthk.cn/gthohthecm.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtayvzjsul.html

[S52] C++：const 与 noexcept
来源：http://hz.jianghu66.top/gtxkqfyrvs.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtofoxvkve.html

[S53] C++：移动语义
来源：http://hz.cashguo.top/gttbkzirje.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gthnvzlymg.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gtmnvowfdy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fengsongda.top/gtjcjctrnn.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gtuuycnvix.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydjk.org.cn/gtawhmygau.html

[S56] C++：optional
来源：http://hz.shzxlz.cn/gtsrgxidwn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtrvwctmbp.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtzklvqcsv.html

constexpr int N = 10;
来源：http://hz.zhiwuduotai.top/gtauurkmmp.html

[S58] C++：命名空间
来源：http://hz.cucudq.cn/gtgyzitgjv.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtzlrjpyig.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtduonsgrr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.bjfxy.top/gtjfdquwze.html

[S60] C++：遍历并删除元素
来源：http://hz.fengsongda.top/gtjyynhlmd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sysykeji.top/gtwgrftibz.html

================================================================================
来源：http://hz.ppjwa.cn/gtldsiyqui.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gttzmoxgnn.html

================================================================================
来源：http://hz.jyoumei.cn/gtdhvisntd.html

[T01] Kotlin：Hello World
来源：http://hz.hnxiangtu.top/gtfmspygft.html

println("Hello")
来源：http://hz.ydzc1.top/gtayykhrbv.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtvdyidesp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtjfchyvig.html

[T03] Kotlin：字符串模板
来源：http://hz.cdnleiting.top/gtrwyqrmlk.html

"值: $b"
来源：http://hz.jqgufenzy.top/gtpisdpiib.html

[T04] Kotlin：空安全
来源：http://hz.yanxiufei.cn/gtqyzaxagi.html

val n: String? = null;  n?.length
来源：http://hz.hysaishi.cn/gtmgtdiwqe.html

[T05] Kotlin：when 表达式
来源：http://hz.52xcode.cn/gtbfbkjzxr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtivobdlvh.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gttcqobswh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtixvszajq.html

[T07] Kotlin：集合过滤
来源：http://hz.chenzaomai.com/gtmxtcuixq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenzaomai.com/gtbaqpbmpe.html

[T08] Kotlin：数据类
来源：http://hz.zhiwuduotai.top/gtdxbrhrbm.html

data class User(val name: String, val age: Int)
来源：http://hz.fengsongda.top/gtvnxetols.html

[T09] Kotlin：扩展函数
来源：http://hz.sysykeji.top/gtqblegooh.html

fun String.exclaim() = this + "!"
来源：http://hz.zhaomingkeji.xyz/gtxykcspiq.html

[T10] Kotlin：默认参数
来源：http://hz.xziqi.cn/gtkjhmwzbu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.52xcode.cn/gtldjbggnn.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtsdndfxtr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gtwngvrhwo.html

[T12] Kotlin：解构声明
来源：http://hz.zhiwuduotai.top/gtqpilbzzi.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgufenzy.top/gtcomifhfh.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtxbpxtdyr.html

val m = mapOf("a" to 1)
来源：http://hz.xinyue.icu/gtlymvixzr.html

[T14] Kotlin：循环
来源：http://hz.jinyuanbaomall.cn/gtqslykequ.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gtrzkbqcbu.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtnrblcqxm.html

interface Shape { fun area(): Double }
来源：http://hz.gogol.net.cn/gtriezlvsx.html

[T16] Swift：Hello World
来源：http://hz.316326.xyz/gtimdpbbje.html

print("Hello")
来源：http://hz.hywenlv.cn/gtvmmozhov.html

[T17] Swift：变量与常量
来源：http://hz.jqgfzy.top/gtjgvdombi.html

var a = 1;  let b = 2
来源：http://hz.tanke756.top/gtaoyujzyc.html

[T18] Swift：字符串插值
来源：http://hz.bjfxy.top/gtsfrajywu.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtedhkfcux.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangkeji.top/gttvfymyhn.html

if let n = opt { print(n) }
来源：http://hz.tanke756.top/gthaxybumb.html

[T20] Swift：数组操作
来源：http://hz.haohaochexian.top/gtznnjsnvc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtwjrpkolh.html

[T21] Swift：遍历
来源：http://hz.xziqi.cn/gtojvrfovv.html

for x in a { print(x) }
来源：http://hz.xuetiantiany.cn/gtejjvrqyp.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gtuothsdjn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gtwpwdmjbj.html

[T23] Swift：函数
来源：http://hz.wangdashe.top/gtcveudhaj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gttqgzutyl.html

[T24] Swift：闭包
来源：http://hz.jqgfzy.top/gtjaxvhdiv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hammf.cn/gtfucqyodm.html

[T25] Swift：结构体
来源：http://hz.smart0.xyz/gtkfouwyhm.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtxgfzeeev.html

[T26] Swift：类与重写
来源：http://hz.sysykeji.top/gtuqsmnkol.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtsbjoqimn.html

[T27] Swift：错误处理
来源：http://hz.zycfv.cn/gthbydqlmq.html

do { try f() } catch { print(error) }
来源：http://hz.chenzaomai.com/gtgtaimroy.html

[T28] Swift：枚举
来源：http://hz.ybcxt.top/gtojzwclkp.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gtqeadjrsd.html

[T29] Swift：guard 提前返回
来源：http://hz.hnxiangtu.top/gtrclnbgsw.html

guard let x = opt else { return }
来源：http://hz.jinqigfzy.top/gtylkzbigx.html

[T30] Swift：协议
来源：http://hz.jinqigufen.top/gtffpcxztf.html

protocol Shape { func area() -> Double }
来源：http://hz.zycfv.cn/gtxjqyabbp.html

[T31] Lua：Hello World
来源：http://hz.chenlongwang.top/gttnwgehth.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtxcfqlmes.html

[T32] Lua：局部变量
来源：http://hz.ehwqpu.com/gtsvfhhrkx.html

local a = 1
来源：http://hz.yuanzhike.top/gtuicufppu.html

[T33] Lua：表（数组）
来源：http://hz.52xcode.cn/gtpwpwaclm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gaohongyu789.top/gtedzhmnnm.html

[T34] Lua：遍历表
来源：http://hz.ivvv.top/gtnkbflxqi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jlsjyb.cn/gtitbomegn.html

[T35] Lua：字典表
来源：http://hz.sysykeji.top/gtwyxpwyyd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yonumen.top/gtndkrkotn.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtibzlfbss.html

function add(a, b) return a + b end
来源：http://hz.nanxinkj.top/gtapdpjjlt.html


<!-- 参考信息 -->