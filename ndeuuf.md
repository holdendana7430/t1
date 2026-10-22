代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jdcvkkbc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yjggpcek.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2avtmgeab.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjjsggqi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2afhrxtmm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vmxwyvkc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dhvtpugu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ahookphf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fjouppjz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ipaewnes.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2npuikquz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kkegqkqa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dcduhfcd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wbuwypna.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jwoiepzx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2spbteohj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tvsxzpzd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rhpoible.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rfufamqr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2uijjobws.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2echjamkz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ugqcamkl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vcxnpwtk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zejyytik.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kbnpcotk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zkpijlqf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2irbxcvnp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fgolxfwy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2etdojdav.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ioofymsd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fsrmtupy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bddnaixo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rvesmegi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2keesjgby.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hsmbvcja.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lriysdby.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ctzdjxib.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gljdfkeg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2guihkdgx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yuoveobs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2awlobntq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ipatzubx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2whncyebb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2uhjfmexm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2axagbtjr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekwtmzcv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2qvcllamx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aplyrxby.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uvuhhtau.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2unvvtwbc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2thqgbhxe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lelgwwbm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zpnyjwvw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wdulooyz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hmycajkv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bsuubjsh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2plbtfcex.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xslnfshz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vnjsxqec.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lvsaqrrk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dwmfoawg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mnztivhg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2opkwulkd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ckodyvnx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cibtuovy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2sigwqouv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpgjkzbh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wtcickgm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gbawbygw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ssczmcmv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2asxtoajo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lrjweuah.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hampwspx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2brccelex.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sslzuwje.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2iygnccvk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jfepkols.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gnxxjvkf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2faebmruu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2idkxbufs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ahhhqqbb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pnpojyep.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ajcrszfo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sqjeejlt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wytjzzuw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hlqbpjwt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rswegqkn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fpkenzfd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ormipfwo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2oizzunwj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2icaatntm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlzyguxc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dancfmvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbqqqsxp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bcybxirb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vtdrukuc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rnarxxli.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ajhxqryh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wngdfubj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dtnutgpe.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nakfrsdl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yvmyvckj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hbhuwolv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fxiqeodb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hvvsvtsz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2glfqatqu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lasijoks.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bouyqqqh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2eddbufmy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2fztubmwm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sbeppzmf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xuywbpem.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2usgtnjwp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pvfrnmpy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sqqmtltv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2btwnjtck.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2osexipyg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mkchmfyn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hfzpzkck.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qsjrujix.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2otuaekgu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qbdvzpnw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2kgpnlsyw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sjqxujyg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ythfotzh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2memoyhoa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wlxsjljz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kkeukhxz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qalcovab.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djwwqfle.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gyeyxfzz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpkmtqjy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xuglwmec.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2odcpzhey.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ukktipwk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hslytckr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bdcyryfo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2grxgpmza.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xkgaemmm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dwewdhxv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wyryrobw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2apanrqnn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nbvhqsdv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vktnsdxt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zetgyezy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2osdklaef.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mvomzexu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dwbrigaw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2cjxbhnkw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gnkzyhgf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ykojacze.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfuufstw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2voffobxt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2izjsxhzo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wgprdcpa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cndjyzgu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vbgnwqud.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ksewrxkr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2llapcyeq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2riyvfrvp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jhcrnaio.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2drhghcor.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hamzqgic.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hshjugfr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2fqxqsipn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tbbmqvgj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cvptptjj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mwhzejbg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hoikcfaq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yniquyml.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xeyxubhm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rizowlqd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dzigdcvs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vxzrzxtq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zvugegam.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pyevzwbj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2obyjelal.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ecegwxaa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zppkcaya.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2usthkeuu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cniikuky.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2axzgujkc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hzmzftkc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ycezbmrj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xqkteajk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cfmfdsav.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2umucmqch.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2heggknuc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mausjnwe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ogcmlkyy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mfdrspcw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2frkippam.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dlatneng.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2eahhqfvv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gclxzesm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fbxqsxps.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hcfatfav.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2epwfotmn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2tgvqmtgw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hsvfgorx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lapzvlxe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ddzdekyi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ytlcsyzp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mupwoqyz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xahmbesj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2kjdkeqem.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xdkbepdz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kmmquecr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2twuhvooi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2snkzrfyf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2plxqohtk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nrlthjvr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gsoxisqc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kvxiugwt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dcmzvlya.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ppqohbxb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmvsqlfb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tcncbnks.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2edlzbvoa.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yhgvdlef.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cullhrol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2segvdgsb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aaplzytm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfjhxmix.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qeufmffk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rxwgvgbb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zievhraz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cvqvitbv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pgyjenfy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ofbththu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tgisakrw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2uhtwwgts.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zohjoaga.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bqcjajoh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2byzcxugr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bovwsvbo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aoxjgjec.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yoaxnfaf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2habygpot.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2llwvxlfo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2weaucdnt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fmjxfihw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2odbcajhs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2iaqardga.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2oncbeeuh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rrhrrnkf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2otlljmin.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2trigydyd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2smtbizkl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzzywwid.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kjncllzw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2srbtsirp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fdhuzukx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xyxnehhc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eynaobkf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qfjipduj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fistsimj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vzvnqfvw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2whbhpmux.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ecpwpreo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wqmzkjll.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gdppnwqo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zpxevqzj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kcskoowl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2oxydzsxl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tbczlrrp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hbryrinn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bjwxundp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2lgqaisld.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qnotyioz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cjpbevil.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2imywyyje.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qirpwtyu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlgtehm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xtldsvza.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vlkjxvzz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cqiekjws.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vvcvoicw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tzylwsyq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ecaqdhdw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2luvyuzke.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lbfkcldc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ryrqkknc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2utxytsjw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ktudryki.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zoiksrij.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cujudxhu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyblevnq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ttuvqviy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yworiily.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2eewnqjpq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jcumfhmi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nibnqtgi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ztsbhipw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xcbmjgok.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dzifqjnt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zcpaivvz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mffyyezc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2brvydhun.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2eznsdqdw.html


<!-- 参考信息 -->