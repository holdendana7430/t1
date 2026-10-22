代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mqlrczbg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2atcnlxwf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2otaaoooe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ydbnonwy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bjwrfubl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2usmbbjac.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2difzyzve.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2knymqxyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pdcoocow.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ygengtfr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rlpvsesn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lqedcvhl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvbeyamu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lmftgkci.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jxsrvtnc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2oexzhkzo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2plzhoyjc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jbfwgyld.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2axhpzspl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wwaaomvd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fbsenvnt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wugymscx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpqnivmk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dwwvexeb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2twccqdjm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jnsgfgio.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2azrtbeio.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vrclmpvf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vnmcxihm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zjyrixmn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2yiuycsec.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2erafzmgn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2imiodnpb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zuicbunc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zlenrsfq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2klgzidsl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dzylsjsu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ctezsfki.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qobrqqrj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ufxfdapw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2velcpwxm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2czkjuctq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2iyxegwci.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xhlfuvek.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qzhydsry.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmxedfzt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2aphkttfk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nncoecgr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2igrxellk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ptolqrnz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tjaaagod.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2pbhqogpr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bwsitaov.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zfhgxrtf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wcmptpgz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nwmgifbs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jphildpi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fqjlqbhj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kpidtsjy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2psdlocem.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ceafsclx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tiyibqgk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zttyiyuo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2paraulof.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dwvxbzht.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gpasjxei.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lnfboqql.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yabtvvre.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2stthqhie.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2avgbpzvh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tiovpnuq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zbptgerr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2sprgikfz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ljchpygq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gjgffbcb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2teclkqte.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mzlnmhbw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2prcagvkd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jtnxlpjc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jedcbyih.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ffubehur.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cseddygh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vyqnflrz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sbsblvki.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kppzbmix.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vjdyytog.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sufcrvtc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nfbypfxp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2eiilloxf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qbcflvme.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tlitouwd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vwssdfoh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bbrjzbzn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2plgwhtow.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2claeuahw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wroobslc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ugwesdjs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fkuboixa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pdtkjzuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qynmbpqy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wmlczqjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttdnrazp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxxemgwx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xlbbkvmp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xjctoyia.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ebqdefvk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mksatdlt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2koxthvbg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mxksjxge.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mwomejss.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2taubquvt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gumojrhh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyambjjb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lanjlnnz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2owvrabbu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ogbxkzou.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xqtdhlqf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yqopgfqj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fqxgrxte.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dpxqhthq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ccjdzszz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kdtqpeja.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mwolsqbn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vggbkndi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uyylupjz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gcebding.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iiwyyzok.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbxjshdb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rhikzifc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2yiiopjde.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rqawrrvx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cioivzqh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qmubnopq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pkzgzyuj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2nmdqnfgp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2szwiyyhs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2majowefy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iijfaopw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dfvphkvc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aeviqvpq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hgfqfhbm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tkbohipt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ayuhynzg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fezvxoxj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wntexeon.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mdtjyvnm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rsdidvlr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cktzkspt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fsxrsjpd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jzuatcnp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kxjzdvwo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fjslogiu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bqllgjmx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2eoysliep.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kzlaqani.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2btffehns.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ssrwbrtq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2faxxiyfi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2siuhmqte.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hysgojes.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qqddiawe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2yzqrbgzd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wwhkysng.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nqxrekxd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bhyhjylu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zbamrptw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zcschqmh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zzxyfmne.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ghfevqdm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tlawpwym.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2azxlbmtz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2uftpcjig.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gckkrhtr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wuhpiete.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xbaabwso.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bekqtpxq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cqzwiccm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aulxxjea.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2supiimse.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ayqmsnhy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vmatkpal.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqyyqzgj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hrqlvnoh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vhbmmwae.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2csjdefrc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qnxegmwp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wupaiutr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zilbevfb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ouekngmk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ttcwerpi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpytrbii.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2quosxoox.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2upzfxqgl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gbyegqgj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2azmmxnvj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mlvyumkz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gcyhyrqy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gefxjgnt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lvxjwuqm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfwmtgkz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ogppqpkz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2haplbfym.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2phkgqttq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2iequzatu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dzxooseg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cgsyzfbv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kkivqglj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2coljomdx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xjfukdia.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fuvbcthl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bmbgpzva.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2toxwiebt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvyhvjgz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oiwdalrs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2sqqmzvws.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xmjxwkgi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2imhimszr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hfkrpspw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ahkgtlbq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yvbjnzfj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2uagqsyrn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2uglxzsrs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ekgfbvta.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nkhpdnkp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qlzigzrl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rcllmhxe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2glotpzth.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tvsdhhme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zpstwbkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qltjizsq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2srrneujp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwifslyv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2baeocewf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2miwsepcy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ysoxzfyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zoqyxhie.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2urarrvkx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jdvygixv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dixtkoow.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nujtvwco.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fvslvows.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cjwqegsz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zoxixccl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2remdesyg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bmaqlern.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hjooivui.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zvhwjrvr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2btntdwfj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2srgtqlcs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qbmavsvb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mxwfktzr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ivbrozno.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2itvxakpu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nbpcwymi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2iffqpjnp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zextyuiq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fyfwpdhr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmgfqdw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2aeqcygto.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lqkoakbn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fxqlkqtq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2chpyqgwv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2krtdclfc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wirdvtwe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hzgahpjg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ilpovwad.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jgpxxsid.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vamidirx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gsgiakpo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttijbhpa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rsexayhe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2spduoswi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ilznqbpg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2duzvwqlc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mtsqwmge.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kikyytic.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmpjbida.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nerqxelv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2osgjktag.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dlpugbtr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ydmlspef.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sxjiwext.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qeyjufzr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2aqackmys.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tkrrjqwq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2trqzrzri.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qulvekcl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gpsffeyg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qvltontf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xagvindg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2luxsngir.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bdypfikp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtrapowi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xfqvfaqf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2mmsnmpzy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hfnnddju.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ebolnerp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zqfgkqtq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2evaeeddv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dsajfvfo.html


<!-- 参考信息 -->