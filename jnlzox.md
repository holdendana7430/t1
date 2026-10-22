代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cddhbial.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2czmvvmof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wduenwdf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2umnbcvll.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hbbbxnxt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ozdjbuty.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jrkhoosk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tgfzxgow.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ofqujfla.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lgxkcnsj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vmkpthfi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gzrjrexx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lzcvwsjb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qmqvcbde.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uoeyrlgg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfxzqecg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lokqwyky.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2eavypkca.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yngxwgqe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yiefoccs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2glhafojd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wxijblxl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hsdiewkk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2asfjnphb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fcktrixc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nftjtazo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vfmfgobq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vxucylgp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kicqvodv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2adpporbj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kebjekoo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2uvislrwn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wtkunnrv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tzcxddeh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rtmsagdw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2dpbywjss.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wrphkjfc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hbxfxdpp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ztqjawhg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jqezxdne.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2acwfwtit.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2htsomknu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xshtfqoi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2eibfaddn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hngpjlhw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ynfhnbuw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qxkfbetq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ppzqimqy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dtxcdofx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zajqlkpn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mkjcrbux.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2etsjgjxs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2moylczzb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyztwkyv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ecdcmvsb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2yknqzfvp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xyotbtuh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hwiddral.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wksssgtk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zgijppmn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cmsidmqc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2plwmtoxw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yfyzwtuv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mxjwljhf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vdhlrsld.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hkihhrdu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qwvobgwb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xqmzetmp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2upaugnhs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2scbhqnwv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bhpxamek.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kayquxpx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2lkzmdqky.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wxretehb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ficszufi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yaljbtgk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kweusilq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2whlsdayk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yucrkddv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xohefwyh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jgadczdq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gczgpowk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2okwjnkan.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2snpvssof.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cqfwyblo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cxkjdoqx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kkgtahaj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bxzjoqtd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wosnbmuj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2slepkzev.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rzjjiygk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygcvxmpj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jznwpsuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hohynccz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qywcciip.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mplkpsxb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2pwlvydme.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rptwctxe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ptwdrdkn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gnngurvk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ebmozkjh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2emmoykpp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bepdhklq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ozyaopsg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxfeqjv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zrymiybw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fkhetiwb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gcnzoopt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mhndmesj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rbtlprfe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2wifuxepl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jwnjybsx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sdyiisdt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dafrbbkv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2srlyvbnr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ndyhvxdc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rbjahoxo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sbjytmmt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mflhbyjw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2namdwmde.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2osdfjwjm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2quidxvnd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fjnjgift.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pxmocvtw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rnznzqzb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qthsdwjv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cpnlrvqi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2niakdipu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nnuvsdqh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uymuvzxy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wwzrotkp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2myxgcdwg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tliqqhtn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vgeihfar.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fuuwqvrj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ytbqawzp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rsrhahvt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2huzmkoah.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xxcnueck.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lldglhop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dohcmkog.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2progiflj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gcwcdcns.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2swpgvpwg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fybvpqjp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xxvgulgi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2faztljlt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rrxmiagu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2satnqrby.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2egddhcsz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yhwctovv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ynbylmft.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hglnthht.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2srxvsxjx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pacfefzh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2edlxuipw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2owqcakvk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2epxtrroq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kzadltin.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wrfuratl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xpmtrptd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2guekbdas.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2crhcofps.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vgtpjqbb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2fchvbbph.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ztnznvqw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zhsskfdq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2eauhgcov.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lsuppfpo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tvopwgxi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lbuhhvwz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2muxywzir.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wguhzmrq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ahvlartr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mbbrioop.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sttuqfre.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gusknjqz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2izzmgdtb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dvjfeqvc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rgiskguu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kzzhxxqm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fvefftlo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2msvwfcki.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cdeyjnqo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sgewznui.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdnswht.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yhvlsscx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vvyevvnp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2skgqqysk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ljbksfio.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2honkomnd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydxeppmk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2btbmcsin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2puzynblh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hlwwdggb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gamohtro.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2skkhbvtv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fkbgtwob.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mcyrmbdy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nunnjpqx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2quguoxfj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kdogcnvk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2regnqfet.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hjamiugu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yjfrqxtv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2swckfdto.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ewjhfmdy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2asrrlswq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wcknoxzm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wgenrngn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2abrtfjim.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2eanfyiev.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hetzobtr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sswfnuld.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2sftcfqef.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lvbqzobr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qmegrpuz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2axaukcto.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lnilfdxz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ecotdppj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qwukqsyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfblmhxy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vxjtikoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmpwxrzt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjzvkhbo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cgtebwmi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2efjwokan.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sruiqxpy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dpadvzkp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cczbqrjb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2njordxvt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kgazvbvb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ntwovrgq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uwzfecjw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wxqnzgow.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vwsoqonw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xugsjjdc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ziqfpipf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zuwjalkf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cvslmeqv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2luoqimwh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2oeledsko.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztefmjoz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2thhoocxj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gmmmqind.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hogogfbj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2oadgylfp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2smcaupws.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2eybwaogq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjmwaobk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2apejnpgr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vinqpcnf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2iabfhxwr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kumhphmq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lqgpjuvk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dhzoyrsx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ftmgnhvp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tsekbvwn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bnicuxcs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hsezpkju.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2puvhbqli.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gyotefrj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zoqxsdsw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xfdzmhey.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2osyckazt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gprnxjby.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hvdfksjp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bfxdgubz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2taazemjy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tlalkied.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2utcjxnhn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jswtitoe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2agjatsfq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2szwtqppk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fzymsygr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2inusbvww.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vijncmku.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2sxjlotdq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nvmvyquo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2abmnbbec.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yxpzdjhz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dnbznvsp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nguqyjte.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oraosjrg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzkzhkue.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ssqerktm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nvzonvuq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sxarjmfb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zpytykie.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wmaznfdv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jppxjpny.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gvqfmlhw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kbnqzemu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mhebyxto.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2giuuuhiu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kqdljzbb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xpcmiixi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2dldmkytx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ecdgwsto.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fevwsdgz.html


<!-- 参考信息 -->