代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3glkupbyh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3oquajyaw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zetrtfqd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zcxqvqwx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fzxqzzdw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yxzmumbr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hsuwvpce.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bkrmmkhv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xwtibsiw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uwudbbcn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kjmfskmk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pvpscbtn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wyubpyhz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hahxpxzb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vrvzvmoo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rcomqwyb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kuiipuuk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mnmqzaku.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3juckedtf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fdpcqzhx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qvfysgqx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kmhwaaew.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lninzlyu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmhskhke.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zyoppvez.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qopcbqey.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wrymhrig.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3icugraae.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bxlidflt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fdgezpxs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qhbmfost.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hxkrmxdb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3svkxccrk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pravxqzs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xprfifgg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dewnzocv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xzlegykm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gvcmkkpy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bhjtdawk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3svdwjzjv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dkwditks.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xtvhwoqb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bhtpchgb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3putffqiw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ewgbrebt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbvmcuov.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3npkqtzcr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tfkjzrzp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rpgxctop.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kqrizwqw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ebofzgif.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3snrodvgu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wravhrfi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3errwsvyl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3phiyobxd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xxxmkwyt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lnrthdyr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bozjrrbx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3coscfnob.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3oitqdlih.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pelmxeid.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hlvfnvhf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bhlkmhdd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zjzoqzrh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bsljmgga.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3eyoiwnwq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cqmrsorx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mmelavty.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cuyatcma.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3emugwztm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zhakavjc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3uzorjiwf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wzweicjs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3htiqapak.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bmkmrwot.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ucopsxpc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3exjjgnuu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xtbfebwa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nrgfpezx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3prysgouz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cxolwgvr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aqdkgpfj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3azkquxpi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vxuefbhw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dyicrrbt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cbhrpzhw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fhnbeaxh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3suhyppdq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3icdephcd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cawagvql.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cnbpfmvv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jqpuvtqe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ghpcvzhx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yhzqpcga.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xupssbze.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dxsalnpw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qddjjmhn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jfukabxz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rfceebtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fszozqlj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yuatdbuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alununsy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uuwyslpx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vmbdgevd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3beunmkeu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nlhqfaxb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nnydrrvg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qzznpyjg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mwsqvfcn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pswolegt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dcnxvclh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sojygjdc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmyoyxmu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ljixccek.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jhhehqyl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mepekldc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xjxhjfkf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gcwmkmov.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3htkhqihf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gjxtlldq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3eflagjsj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lijewnbf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3exqqsint.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvpnpags.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hnnzypbr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hcmnlgkw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tqjrohml.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryroezek.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ywqeghtz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mbphnlzt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uiuokwqh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bixobaro.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3icmnfywm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3thgcjish.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wyerzrbt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3svhrstrh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpsixoyx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jdbaiqsn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ylpzkjov.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvdmkalk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xpwfcxmt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3athxtquj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hbqixmrc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xsjnrruw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lsrhcmxj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qlisxacf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3uejelgco.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3khibmipj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dohakukt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lromkvac.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3aduhosnx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zirmvvjo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ufhfzrik.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xrpyqcik.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ttwwozsu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3plozcbln.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3iizbfjai.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tpklcqoo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zvwmgeuz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3awhidapw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vyyeprzi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3fjnwivmg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bvaaxpyi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yjgbtpoq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pkdqhptr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gwjdjzbc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lesharcy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bbzpneav.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bklwgbfe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ohsvmske.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yxuofmta.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yhcoupwu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nnrxpelh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yjifhzkm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xxselihr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3awpomhdx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ifplkkwr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jqpurlpo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3atjehrtr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpnuuytu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uzdxzigg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oyoualni.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nykpfqwz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wqiwgjxm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3drrqfhvn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gvwssqkh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3iitoxkbp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3knpsztot.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wrztjidq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3npvqyqyu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zseknemq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tkonjfvv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qvycyqen.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cffbcbcr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3eojbylgi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqnrixhw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kuzyyrqi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tkabifzb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fnxzbqcg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3frpiwjmn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vaywoqna.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3auareilu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxjcftle.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3krzvrguc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wuxgikiq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnbupzlp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qrezdixi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3baniucmm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imygiqso.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3eefnsuhb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jhjhayeg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hhhgglka.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3cusshbaw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hvvxbgsw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fsiycana.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qrzrzjbj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pjllsruk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ggvfwpui.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gxgwvjqs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wvzlozod.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hbzygpxw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pjrxkqjx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jbsfbhew.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wfwmvlku.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ygppmehz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3musboesq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ntvzkrma.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bheigxjc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kogwhfei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldqzjtmx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hatgezas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybofyjzw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lqwkhfle.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hsirixui.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bcthsopn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3syfahbtc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mdxnbcvb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hsjhwayb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bkshdhcq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xgjtqgaz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xumqxwss.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rpwvqjct.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xxwtmour.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rvwmsqzd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ticllzll.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iweqcnoy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vasvlcla.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qflheavr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqjgjwgh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3vawyoapp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3czwzwkse.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3joqmoowx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3iudyaxpu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ccfdggju.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cbrswamq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovputnin.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rlqkakby.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3blztwbab.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cjlsehpk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oalbpxzz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3laojadje.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnvoywm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fjmnexjj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eiyesyeg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qliqefkn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fgliailx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jagsrvlp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3jfgyetkn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ceeniloa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hryhyxkn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ciwshddb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dapxtduk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kstcjkaz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3neipbcxr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3chbscdbg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xfpslqug.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3syhbegfd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xeulrhgx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ainjcbwl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lsdbojoh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3oqfuryfm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rtisnyzw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vhyqiuhu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vlnwhmpu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ikyjqlff.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bweedern.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jdvfonpr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3nhvjhcsf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wwnhdevk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3njarxxoi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3hfkinkfg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rvelxubq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efywexev.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gcdjosor.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bhiqmwnf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3swozadre.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ctnkanap.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwyhyn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zsqipifx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ersjzfrt.html


<!-- 参考信息 -->